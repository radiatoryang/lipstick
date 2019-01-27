## research: possible Unity workflow

### baking-out and storing lipsync data
- create custom PostProcessor for Unity Audio files https://docs.unity3d.com/ScriptReference/AssetPostprocessor.OnPostprocessAudio.html
- put lipsync data in https://docs.unity3d.com/ScriptReference/AssetImporter-userData.html
- need custom inspector for AudioFiles to visualize lipsync data though?? (to edit, to correct, to reimport or refresh or delete, etc)

### working with lipsync data in-game
- ``LipstickBehavior.cs`` on a SkinnedMeshRenderer, connect to AudioSource, configure mouth shapes and interpolation speed
- ``LipstickMouthShape`` ScriptableObject with Dictionary<BlendShapeKeyName,BlendShapeValue>
- ``LipStickMouthShape2D`` toggles different sprites or gameObjects?
- build Mixamo blendshape presets (and Character Creator presets?)
