# Awiline graphics dependencies

Public, versioned artifacts for Awiline graphics repair. Large binaries are release assets, not Git files.

## Patched MoltenVK 1.4.2

The `graphics-deps-1.4.2-1` release contains `libMoltenVK-1.4.2-UE4-workaround-universal.dylib`.

- SHA-256: `cd6335d19b54904fefed3ba5f01f68889953dcf9ca9cda803da6233a3b8e6c36`
- Architectures: `x86_64`, `arm64`
- Upstream source: https://github.com/KhronosGroup/MoltenVK/tree/v1.4.2
- Patch/build recipe: [build-moltenvk-ue4.yml](build-moltenvk-ue4.yml)
- License: Apache-2.0; [upstream license text](licenses/MoltenVK-LICENSE)

The recipe inserts the historical UE4 shader workaround into the public MoltenVK v1.4.2 source. It documents the build used for this pinned artifact; end-user Macs do not build it.

DXVK-macOS `1.10.3-20230507-async` is acquired from the [Gcenx release](https://github.com/Gcenx/DXVK-macOS/releases/tag/v1.10.3-20230507-repack) and retains its [zlib/libpng license](licenses/DXVK-LICENSE). Its release archive SHA-256 is `acd1520ad105d8ef124a09c8e11a259a5dc8bdc565ad18e0e52693f9807b2477`.
