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

![Desktop 2024 01 17 - 10 30 49 01_short](https://github.com/jbat100/sonosthesia-unity-demo-instrument/assets/1318918/2a9622b9-c820-4f28-991e-22df35698778)

### Experimental

Scaled instrument builders are in development allowing configurable scale and more control over the procedural placement of elements allowing the procedural creation of instruments such as harps and xylophones.

## MIDI Controller



## MPE Controller

![Desktop 2024 01 17 - 10 50 06 02_short](https://github.com/jbat100/sonosthesia-unity-demo-instrument/assets/1318918/b21e625a-6ba0-4535-a195-c89b7fe42217)
