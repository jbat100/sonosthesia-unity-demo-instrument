# sonosthesia-unity-demo-instrument

This demo showcases the instrument building and MIDI/MPE control capabilities of the sonosthesia framework. In particular the following packages:

- [com.sonosthesia.touch](https://github.com/jbat100/sonosthesia-unity-packages/tree/main/packages/com.sonosthesia.touch)
- [com.sonosthesia.instrument](https://github.com/jbat100/sonosthesia-unity-packages/tree/main/packages/com.sonosthesia.instrument)
- [com.sonosthesia.midi](https://github.com/jbat100/sonosthesia-unity-packages/tree/main/packages/com.sonosthesia.midi)

Note the raw MIDI functionality is presented in a separate [demo project](https://github.com/jbat100/sonosthesia-unity-demo-midi).


## Installation

Note that to add those packages to your Unity project you will need to add the following [scoped registeries](https://docs.unity3d.com/Manual/upm-scoped.html) to your `Packages/package.json` file (`Keijiro` only necessary for the [com.sonosthesia.rtmidi](https://github.com/jbat100/sonosthesia-unity-packages/tree/main/packages/com.sonosthesia.rtmidi) backend). 


```
"scopedRegistries": [
    {
      "name": "Neuecc",
      "url": "https://package.openupm.com",
      "scopes": [
        "com.neuecc.unirx",
        "com.cysharp.unitask"
      ]
    },
    {
      "name": "Keijiro",
      "url": "https://registry.npmjs.com",
      "scopes": [
        "jp.keijiro"
      ]
    },
    {
      "name": "Sonosthesia",
      "url": "https://registry.npmjs.com",
      "scopes": [
        "com.sonosthesia"
      ]
    }
  ]
```

## Procedural Instrument Builders

Note these builders can be used both in play mode or in edit mode.

### Keyboard

A highly configurable keyboard builder. 

<p align="center">
    <img alt="Keyboard Builder" src="https://github.com/jbat100/sonosthesia-unity-demo-instrument/assets/1318918/2a9622b9-c820-4f28-991e-22df35698778" width="75%">
</p>


### Experimental

Scaled instrument builders are in development allowing configurable scale and more control over the procedural placement of elements allowing the procedural creation of instruments such as harps and xylophones.

## MIDI Control

![MIDIController_clip_6_32_short](https://github.com/jbat100/sonosthesia-unity-demo-instrument/assets/1318918/bd43d460-3643-41e9-9492-1cbd801c8fbb)

## MPE Control

<p align="center">
    <img alt="MPE Controller" src="https://github.com/jbat100/sonosthesia-unity-demo-instrument/assets/1318918/b21e625a-6ba0-4535-a195-c89b7fe42217" width="75%">
</p>

The procedural builder uses a configurable prefab which can handle the production of MPE note streams. Currently pointer based and trigger (using physics) based interactions are supported. When using the pointer interaction the pressure, slide and bend of each note can be controlled sepearately using drag and pressure on multitouch platforms. 
