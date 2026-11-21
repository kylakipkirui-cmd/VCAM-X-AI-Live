# VCAM X AI Live

Windows x64 real-time face replacement application.

## Project source

The application source is expected under `vcam-x-starter/`. The Windows installer build workflow is prepared in `.github/workflows/windows-build.yml` and can be run after the source files are committed.

## Build output

A successful Windows build publishes `VCAM-X-Setup-x64.exe` as a GitHub Actions artifact. This repository currently contains the build configuration only; the application source and installer scripts must be added before a complete installer can be produced.

## Important

- Target: Windows 10/11 x64.
- GPU acceleration is hardware/driver dependent and must be verified at runtime.
- `pyvirtualcam` does not install a system virtual-camera driver by itself; OBS Virtual Camera or another compatible driver may be required.
- Model-weight redistribution must comply with each model's license.
