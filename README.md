# Tauri with Create React App

This project was bootstrapped with [Create React App](https://github.com/facebook/create-react-app).

Make sure to install the [Tauri dependencies](https://tauri.studio/docs/get-started/intro) on your system (I'm using WSL2/Ubuntu).

`npx create-react-app tauri-cra-example`

Added `tauri` to project as dev dep

`yarn add @tauri-apps/cli@latest -D`

`yarn tauri init`

### WSL2 specific notes

When setting up your XServer, make sure to use the correct settings for OpenGL. The following fixed it for me using `VcXsrv` (recommended by Tauri team).

`export LIBGL_ALWAYS_INDIRECT=0`

Start a new instance of VcxSrv with and unselect the Native opengl box on the Extra Settings page, and select the Disable access control box.

![settings](https://i.stack.imgur.com/4n4XH.png)
