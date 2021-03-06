# Kromx

Krom Experiment

```bash
git clone --recursive https://github.com/armory3d/Kromx
cd Kromx
```
```bash
# Windows
# Unpack `v8\libraries\win32\release\v8_monolith.7z` using 7-Zip (exceeds 100MB)
node Kinc/make -g direct3d11 --noshaders
# Open generated Visual Studio project
# Build for x64 & release
```
```bash
# Linux
node Kinc/make -g opengl --noshaders --compiler clang --compile
cd Deployment
strip Krom
```
```bash
# macOS
node Kinc/make -g opengl --noshaders
# Open generated Xcode project
# Add `path/to/Kromx/v8/libraries/macos/release` into `Project - Krom - Build Settings - Search Paths - Library Search Paths`
# Build
```
```bash
# Android - wip
node Kinc/make android -g opengl --noshaders
# Manual tweaking is required for now:
# https://github.com/armory3d/Kromx/blob/master/kincfile.js#L68
# Open generated Android Studio project
# Build for device
```
```bash
# iOS - wip
node Kinc/make ios -g opengl --noshaders
# Manual tweaking is required for now:
# https://github.com/armory3d/Kromx/blob/master/kincfile.js#L84
# Open generated Xcode project
# Add `path/to/Kromx/v8/libraries/ios/release` into `Project - Krom - Build Settings - Search Paths - Library Search Paths`
# Build for device
```
