

# File NodeEditorManager.h

[**File List**](files.md) **>** [**AGE**](dir_c1649042ac9dcb65c6181568c305ecb0.md) **>** [**VisualScripting**](dir_5fd6adde202bfce222fbe02ea3ca8deb.md) **>** [**Public**](dir_1a0a2758c948b853064feab5aefe3feb.md) **>** [**NodeEditorManager.h**](_node_editor_manager_8h.md)

[Go to the documentation of this file](_node_editor_manager_8h.md)


```C++
#pragma once
#include "Core/Public/Core.h"
#include "VisualScripting/Public/NodeEditorWindow.h"
#include <imgui_node_editor.h>

#include <vector>
#include <string>

namespace AGE
{
    class NodeEditorManager
    {
    public:
        NodeEditorManager();
        NodeEditorManager(const NodeEditorManager&) = delete;
        NodeEditorManager(NodeEditorManager&&) = delete;
        virtual ~NodeEditorManager();

        void RegisterFunctions();

        void DeregisterFunctions();
        void CreateContextAndWindow(const std::filesystem::path& Filepath, const std::string& WindowName, void* Target = nullptr);
        void RenderWindows(TimeStep DeltaTime);

        static uint32_t GetNewNodeID() {return ++NodeID;}

    private:
        void CreateNewWindow(const std::string& WindowName, ax::NodeEditor::EditorContext* Context, void* Target = nullptr, bool LoadingExisting = false);

        void RebuildWindow(const std::string& WindowName);

        bool IsConfigFileStored(ax::NodeEditor::Config Config);


    private:

        std::vector<std::pair<Ref<NodeEditorWindow>, ax::NodeEditor::EditorContext* >> m_ActiveWindows;

        std::vector<ax::NodeEditor::Config> m_Configs;

        static uint32_t NodeID;
    };
}
```


