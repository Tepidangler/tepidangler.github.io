

# File EntryPoint.h

[**File List**](files.md) **>** [**AGE**](dir_c1649042ac9dcb65c6181568c305ecb0.md) **>** [**Core**](dir_40f28070a54f843eaf86230230ee6eb2.md) **>** [**Public**](dir_4d1ade32537ccbee8ff5d36b16abbd57.md) **>** [**EntryPoint.h**](_entry_point_8h.md)

[Go to the documentation of this file](_entry_point_8h.md)


```C++
#pragma once
#include"Core/Public/App.h"



//Creates our Game/App for us rather than having to do that inside of the application itself because we don't truly know what anyone might use this for.
// Looking at you here Donald.

extern AGE::App* AGE::CreateApp(ApplicationCommandLineArgs args);

int main(int argc, char** argv)
{
    AGE::Log::Init();
    AGE::CoreLogger::Info("Initialized AGECORE Log");
    AGE::GameLogger::Info("Initialized AGEGame Log"); 
    AGE_PROFILE_BEGIN_SESSION("Startup", "./AGEProfile-Startup.json");
    auto app = AGE::CreateApp({argc, argv});
    AGE_PROFILE_END_SESSION();
    AGE_PROFILE_BEGIN_SESSION("Runtime", "./AGEProfile-Runtime.json");
#if AG_DEBUG
    try
    {
        app->Run();
    }
    catch (std::exception& e)
    {
        AGE::CoreLogger::Error(e.what());
    }
#else
    app->Run();
#endif
    AGE_PROFILE_END_SESSION();
    AGE_PROFILE_BEGIN_SESSION("Shutdown", "./AGEProfile-Shutdown.json");
    delete app;
    AGE_PROFILE_END_SESSION();
}


```


