# Jungle Atmos Android 0.3.0

## Changes
- Previous/Next wrap through all 21 scenes and start the selection immediately.
- Each source follows a continuous 24-second overhead flyover: front approach, rise near the listener's zenith, recede behind, then return on a lower arc, with some original scene motion retained.
- Scene changes stop Wade's intro; live status shows the scene number and title.
- **Binaural 360** renders the app's HRTF elevation cues. The optional Android 5.1 Spatializer input has no height channels.

## Audio engine
- Carries forward the v0.1.0 PCM normalization/clipping fix.
- Offers live Stereo pan and generic measured MIT KEMAR binaural HRTF, with crossfades and output limiting.
- Uses Android's device-managed Spatializer only when the current 5.1 route is eligible; this is not Atmos object-audio decoding.
- Retains all 21 scenes, automatic private local logs, the Wade intro, visualizer, and checksum-verifying updater.

## Limits and testing
This is a sound-effects demo, not a music player. The generic KEMAR HRTF is not personalized and has no head tracking; localization varies by listener and earphones. It does not encode or decode Dolby Atmos or claim AirPods head tracking. No Pixel 11 Pro/AirPods Pro is attached, so listening, routing, and localization still need device testing. The full Android sideload update flow also remains unverified; Android requires approval before installation.
