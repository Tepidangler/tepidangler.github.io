

# File AGEAudio.h

[**File List**](files.md) **>** [**AGE**](dir_c1649042ac9dcb65c6181568c305ecb0.md) **>** [**Audio**](dir_db6938f1ff25f5ebd4fcc50cd8804f79.md) **>** [**AGESound**](dir_74e7b55d8738892ae451b103e367b12d.md) **>** [**Public**](dir_da409af63540810d65578dc2200e9eaa.md) **>** [**AGEAudio.h**](_a_g_e_audio_8h.md)

[Go to the documentation of this file](_a_g_e_audio_8h.md)


```C++
#pragma once
#include "Core/Public/Core.h"
#include "Audio/AudioEngine/Public/AudioEngine.h"
#include "AL/al.h"
#include "AL/alext.h"


namespace AGE
{
    class AudioSource;

    class AGESound : public AudioEngine
    {
    public:
        AGESound();
        ~AGESound() override = default;
        virtual void Init() override;
        virtual void Start() override;
        virtual void Update() override;
        virtual void Stop() override;

        virtual void LoadBanks(const std::vector<Ref<SoundBank>>& Banks) override;
        virtual void LoadBank(Ref<SoundBank> Bank) override;

        virtual std::string& GetCurrentEventName() override;
        virtual void SetCurrentEventName(const std::string& Name) override;
        virtual void LoadEvents() override{};
        virtual void Shutdown() override;
        virtual bool IsEventValid(const std::string& EventName) override;

        virtual void SetParameterByName(const std::string& Name, float Value) override;
        virtual void Set3DAttributes(void* Attributes) override;
        static AudioSource LoadAudioSource(const std::string& FileName);
        void Play(const Ref<AudioSource>& Source);
        void Stop(const Ref<AudioSource>& Source);
        void Stop(const std::vector<Ref<AudioSource>>& Sources);




        static void SetDebugLogging(bool Log);

    private:

        static int32_t ConvertToInt(char* Buffer, size_t Length);
        static AudioSource LoadAudioSourceMP3(const std::string& FileName);
        static AudioSource LoadWav(const std::string& FileName);
        static bool LoadWavFileHeader(std::ifstream& File, uint8_t& Channels, int32_t& SampleRate, uint8_t& BitsPerSample, ALsizei& Size);


        void StopSound();
        static void UnloadSound(const Ref<AudioSource>& Source);

        //void UpdateStream(const uint32_t SourceID, const ALenum& Format, const int32_t SampleRate, std::vector<char> SoundData, size_t& Cursor);

        //void AttachBufferToSource(uint32_t SourceID, ALsizei n, uint32_t* Buffer);
        //void DetachBuffersFromSource(uint32_t SourceID, ALsizei n, uint32_t& Buffers);
        std::vector<std::string> GetAvailableSoundDevices() { return m_AvailableSoundDevices; }

        static bool DisplayErrorCode(const std::string& FN, const uint32_t line, ALenum Error);

    private:
        bool FindAvailableDevices(std::vector<std::string>& DevicesArray, ALCdevice* Device);
    private:

        [[maybe_unused]] ALCdevice* m_Device;

        [[maybe_unused]] ALCcontext* m_Context;

        std::vector<std::string> m_AvailableSoundDevices;

        std::string m_EventName = "NONE";
    };
}
```


