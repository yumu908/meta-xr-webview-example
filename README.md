# Oculus WebView Example

This Unity project demonstrates how to use the [Vuplex 3D WebView asset](https://developer.vuplex.com/webview/overview) with Oculus Quest, Oculus Go, and Gear VR. It includes the [Oculus Integration](https://assetstore.unity.com/packages/tools/integration/oculus-integration-82022) package, so the only thing you must import is the [3D WebView for Android plugin](https://assetstore.unity.com/packages/tools/gui/3d-webview-for-android-with-gecko-engine-158778).

<p align="center">
  <img alt="demo" src="./demo.gif" width="480">
</p>

## Steps taken to create this project

1. Created a new Unity project
2. Installed v14.0 of the Oculus Integration package from the Asset Store
3. Imported the [Vuplex 3D WebView asset](https://developer.vuplex.com/webview/overview) ([.gitignore](https://github.com/vuplex/oculus-webview-example/blob/69d404181ba188937c124d154d7b1eab6173f609/.gitignore#L62))
4. Created a new scene named OculusWebViewDemoScene to combine 3D WebView's [WebViewPrefab](https://developer.vuplex.com/webview/WebViewPrefab) and [Keyboard](https://developer.vuplex.com/webview/Keyboard) components with the Oculus OVRCameraRig
5. Added the Oculus [UIHelpers prefab](Assets/Oculus/SampleFramework/Core/DebugUI/Prefabs/UIHelpers.prefab) to the scene to add controller support.
6. Made the following tweaks to the UIHelpers prefab instance:
- Set the "Ray Transform" and "Joypad Click Button" values for the OVRInputModule script
- Disabled the Sphere cursor visual
- Enabled the LaserPointer's line renderer and set its material

## License

The Oculus Integration library located in Assets/Oculus is Copyright © Facebook Technologies, LLC and its affiliates. All rights reserved. The Oculus Integration Library is licensed under the [Oculus SDK License](https://developer.oculus.com/licenses/sdk-3.5/).

All other code and assets are Copyright © Vuplex, Inc and licensed under the MIT License.
