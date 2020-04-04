# BabylonNativeWebAudio Plug-in
For adding WebAudio into BabylonNative Apps

Right now this is just in the planning phase.  Here are all the methods available in the 3 WebAudio contexts, whether they are present in the project being wrappered, [Lab Sound](https://github.com/LabSound/LabSound), if they are planned to be supported, and any relevent notes.

| BaseAudioContext | In Lab Sound | Planned | Notes
| --- | --- | --- | ---
| AudioWorklet  | No | No | Do not need
| currentTime  | Yes | Yes |
| destination  | Yes | Yes |
| listener  | Yes | Yes |
| sampleRate  | Yes | Yes |
| state | No | No  | Do not need
| onstatechange() | No | No | Do not need
| createAnalyser()  | Yes | Yes | Only useful for displaying, not audio editing
| createBiquadFilter() | Yes | Yes | Used to create equalizers
| createBuffer()  | Yes | Yes |
| createBufferSource()   | Yes | Yes |
| createConstantSource()  | No | No | Do not need
| createChannelMerger() | Yes | Yes |
| createChannelSplitter() | Yes | Yes |
| createConvolver() | Yes | Yes | Needed for things like reverb
| createDelay() | Yes | Yes | Needed for feed back loops, more complex stereo
| createDynamicsCompressor() | Yes | Yes | Used to level out gain
| createGain()   | Yes | Yes |
| createIIRFilter() | No | No |  Do not need
| createOscillator()  | Yes | Yes |
| createPanner()  | Yes | Yes |
| createPeriodicWave() | No | No | Do not need
| createScriptProcessor() | Yes | No | Deprecated in API
| createStereoPanner()  | Yes | Yes |
| createWaveShaper() | Yes | Yes |
| decodeAudioData() | Yes | Yes |


| AudioContext | In Lab Sound | Planned | Notes
| --- | --- | --- | ---
| baseLatency | No | No | Do not need
| outputLatency | No | No | Do not need
| close   | Yes | Yes | Not in Offline
| createMediaElementSource()  | Yes | Yes
| createMediaStreamSource()  | Yes | Yes
| createMediaTrackSource()  | Yes | Yes
| getOutputTimestamp() | No | No | Do not need
| resume()   | Yes | Yes
| suspend()   | Yes | Yes


| OfflineAudioContext | In Lab Sound | Planned | Notes
| --- | --- | --- | ---
| / length | Not Sure | Not Sure | calculate-able
| / startRendering | Yes | Yes | No point without having
| resume()  | No | No | Do not need
| suspend()  | No |  No | Do not need

