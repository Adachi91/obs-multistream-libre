# obs-multistream-libre
Community fork of [Aitum Multistream](https://github.com/aitum/obs-aitum-multistream) for [OBS Studio](https://github.com/obsproject/obs-studio). Adds multi-streaming capability, supporting Twitch, YouTube, Kick, Rumble, TikTok, Joystick, and more with custom RTMP destination.

>Note: Each additional stream will double the uplink/upload bandwidth required to keep streams stable.  

### Changes/Upstream difference  
1. Removed phone home feature used to pull in advertisements.
2. Added stream health to the dock so you can see if you're dropping frames for other services.
3. Fixed possible memory corruption bug.
4. Fixed possible memory leak bug.

## Build
- In-tree build
    - Build OBS Studio: https://obsproject.com/wiki/Install-Instructions
    - Check out this repository to UI/frontend-plugins/aitum-multistream
    - Add `add_subdirectory(aitum-multistream)` to UI/frontend-plugins/CMakeLists.txt
    - Rebuild OBS Studio
- Stand-alone build
    - Verify that you have development files for OBS
    - Check out this repository and run `cmake -S . -B build -DBUILD_OUT_OF_TREE=On && cmake --build build`

## Translations
Please read [Translations](TRANSLATIONS.md)
