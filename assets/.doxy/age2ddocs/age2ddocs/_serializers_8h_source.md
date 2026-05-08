

# File Serializers.h

[**File List**](files.md) **>** [**AGE**](dir_c1649042ac9dcb65c6181568c305ecb0.md) **>** [**Utils**](dir_2ea46939f511f6144e40e8e7d32aa78e.md) **>** [**Public**](dir_6a98f83a49b4a8e48cceea88fbb59588.md) **>** [**Serializers.h**](_serializers_8h.md)

[Go to the documentation of this file](_serializers_8h.md)


```C++
#pragma once
#include "Scene/Public/Scene.h"
#include "Project/Public/Project.h"

namespace AGE
{
    class SceneSerializer
    {
    public:
        SceneSerializer(const Ref<Scene>& S);

        void Serialize(const std::string& FilePath);

        bool Deserialize(const std::string& FilePath);

    private:
        Ref<Scene> m_Scene;
    };

    class ProjectSerializer
    {
    public:
        ProjectSerializer(Ref<Project> Project);

        bool Serialize(const std::filesystem::path& FilePath);
        void SerializeBinary(const std::filesystem::path& FilePath);
        bool Deserialize(const std::filesystem::path& FilePath);
        bool DeserializeBinary(const std::filesystem::path& FilePath);
    private:

        Ref<Project> m_Project;
    };
}
```


