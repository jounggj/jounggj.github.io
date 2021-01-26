---
title: "Importing ExoPlayer for Unity"
layout: single
permalink: /product/exoplayer/importing/
sidebar:
  nav: "docs"
toc: true
toc_label: "Table of Contents"
toc_icon: "cog"
---

## Importing

### Unity 2019.x

1. Create or Open target Unity project

1. Import *ExoPlayer for Unity* asset package

1. Switch to Android platform
    - File --> Build Settings --> Platform --> Select Android and Switch Platform

1. Enable Custom Main Gradle Template
    - Edit --> Project Settings --> Publishing Settings --> **check** `Custom Main Gradle Template`
    - Open `Assets/Plugins/Android/mainTemplate.gradle` with any text editor
    - Add below line inside `dependencies {  }`
```javascript
implementation 'com.google.android.exoplayer:exoplayer:2.12.2'
```

1. Set Graphics API
    - Edit --> Project Settings --> Other Settings --> Graphics API
    - **Remove** Vulkan
    - Add OpenGL ES 2.0 or OpenGL ES 3.0

1. Disable Multithreaded Rendering option
    - Edit --> Project Settings --> Other Settings --> **uncheck** `Multithreaded Rendering`

1. Set Minimum API Level to API Level 28 or later
    - Edit --> Project Settings --> Other Settings --> Minimum API Level
    - set to API Level 28 or later

1. Enable Internet access to test sample scenes
    - Edit --> Project Settings --> Other Settings --> Internet Access
    - set to Require


### Unity 2020.x

1. Follow import instruction for Unity 2019.x
1. Enable Custom Base Gradle Template
    - Edit --> Project Settings --> Publishing Settings --> **check** `Custom Base Gradle Template`
    - Open `Assets/Plugins/Android/baseProjectTemplate.gradle` with any text editor, and change version of gradle plugin to **3.4.0**
```javascript
classpath 'com.android.tools.build:gradle:3.4.0'
```



## Demo Scenes

### SampleVideoPlayer

{% include video id="6yEy42vJO6c" provider="youtube" %}

- provides simple video player interface
- play, pause, stop, previous media, next media, rewind, forward



### SampleVideoCubes

{% include video id="B-1e7c0EfPU" provider="youtube" %}

- provides simple video rendering on texture object



### Sample360Video

{% include video id="4DkcartY5EI" provider="youtube" %}

- shows playing a 360 video on a texture object, which is mapped on a sphere object


