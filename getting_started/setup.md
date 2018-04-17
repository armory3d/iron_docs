# Setup

## Quick start
- git clone --recursive https://github.com/armory3d/iron_examples
- Drop one of the example folders into [KodeStudio](https://github.com/Kode/KodeStudio/releases)
- Run

## Content pipeline

Iron does not import standard 3D file formats directly. Instead, a custom `.arm` scene format is developed for efficiency. See structure of the [scene format](https://github.com/armory3d/iron/blob/master/Sources/iron/data/SceneFormat.hx). JSON (textual, debug) or ArmPack (binary, based on MessagePack, deploy) serialization is used, with optional compression supported.

[.arm exporter](https://github.com/armory3d/iron/blob/master/tools/exporter.py) for Blender is provided. Blender can be operated from command line, making it easy to integrate is as an asset converter.

To import `.fbx`/`.gltf`/`.obj` formats, use [iron_format](https://github.com/armory3d/iron_format).

## Render pipeline

Shaders are written in glsl syntax and cross-compiled using [krafix](https://github.com/Kode/krafix).

TBD
