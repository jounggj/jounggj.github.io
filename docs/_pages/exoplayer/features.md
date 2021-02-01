---
title: "Features of ExoPlayer for Unity"
layout: single
permalink: /product/exoplayer/features/
sidebar:
  nav: "docs"
toc: true
toc_label: "Table of Contents"
toc_icon: "cog"
---

## Features

- provides basic features of Android [ExoPlayer](https://exoplayer.dev/)
- uses ExoPlayer v2.12.2
- support for playlist
- support for [DASH](https://exoplayer.dev/dash.html)
- support for [HLS](https://exoplayer.dev/hls.html)
- supports various media formats



## Requirements
- Supported Unity versions: Unity 2019.2 or later, Unity 2020.x
- Supported Platform: Android (API level 28+)


## Limitations

- Supported Settings
  - `Vulkan` is **not** supported
  - `Multi-threaded Rendering` is **not** supported

      | Multi-threaded Rendering | Off | On |
      |--:|:--:|:--:|
      | OpenGL ES 2.0 | **O** | X |
      | OpenGL ES 3.0 | **O** | X |
      | Vulkan | X | X |

- Playing Unity Streaming Assets is **not** supported

- **NOT** tested [Cue](https://exoplayer.dev/doc/reference/com/google/android/exoplayer2/text/Cue.html) support feature (yet)


