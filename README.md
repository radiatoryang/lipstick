# lipstick

## update, 1 Dec 2020: I never actually had time to work on this at all, so I'm just going to archive the repo for now, sorry

Lipstick is an open-source fork of Oculus' OVRLipSync implementation for Unity (under Oculus Audio license) with some additional modifications to make it easier to use out of the box. It is not supported nor endorsed by Oculus in any way.

Currently, I've just imported the [Oculus Lipsync Utility v1.3.0 .unitypackage](https://developer.oculus.com/downloads/package/oculus-lipsync-unity/) from the Oculus site, and haven't done any real work on this yet.

In theory, all of this will work fine on Windows / Mac / Android. (Oculus doesn't ship any lipsync binaries for Linux or iOS.) If you bake out the lip sync data, then it'd work for any platform.

## PLANNED WORKFLOW
- use this in real-time, in-game, to get accurate dynamic lip sync (Windows, Mac, Android)
- OR automatically bake out lipsync data via an AssetPostProcessor / custom EditorWindow interface (any platform)
- either way, use the built-in presets for a Mixamo Fuse Blendshape rig or 2D character portrait, and/or configure visemes for your own face rig

### CONTRIBUTORS
- pull requests are welcome, look at the Roadmap above and feel free to start an Issue to introduce yourself

### LICENSE
Note that this repo, and any forks, must stay licensed under [Oculus Audio License 3.3](https://developer.oculus.com/licenses/audio-3.3/)
- this system relies heavily on some closed-source lip sync libraries from Oculus
- only the Unity integration (and sample assets) are actually open source here
- if that bothers you / if that's a dealbreaker, sorry

I am not a lawyer, but I think the license says:
- you can use this Oculus-derived code / libraries in any project, not necessarily for use in an Oculus device or platform
- Oculus retains ownership over the audio code and sample assets, you retain ownership over the rest of your project
- if you modify the code or assets in the \Oculus\ folder, then Oculus technically has the right to demand access to those modifications
- if you bake out lip sync data, then you own that content

This public open source GitHub repo is hereby my attempt to comply with providing access to Oculus.
