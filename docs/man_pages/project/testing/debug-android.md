debug android
==========

Usage | Synopsis
---|---
Deploy on device, run the app and stop at the first breakpoint | `$ tns debug android --debug-brk [--device <Device ID>] [--debug-port <port>]`
Deploy in the native emulator, run the app and stop at the first breakpoint | `$ tns debug android --debug-brk --emulator [<Emulator Options>]`
Deploy in Genymotion, run the app and stop at the first breakpoint | `$ tns debug android --debug-brk --geny <Geny Name>`
Attach the debug tools to a running app on device | `$ tns debug ios --start [--device <Device ID>] [--debug-port <port>]`
Attach the debug tools to a running app in the native emulator | `$ tns debug android --start --emulator [<Emulator Options>]`
Attach the debug tools to a running app in Genymotion | `$ tns debug android --start --geny <Geny Name> [--print-app-output]`
Retrieve the device port on which you are debugging | `$ tns debug android [--device <Device ID>] --get-port`
Detach the debug tools | `$ tns debug android --stop`

Debugs your project on a connected device, in a native emulator or in Genymotion.

### Options
* `--device` - Specifies a connected device on which to debug the app.
* `--emulator` - Specifies that you want to debug the app in the native Android emulator from the Android SDK.
* `--geny` - Specifies a Genymotion emulator on which you want to debug your app.
* `--debug-brk` - Prepares, builds and deploys the application package on a device or in an emulator, launches the Chrome DevTools of your Chrome browser. 
* `--start` - Attaches the debug tools to a deployed and running app.
* `--stop` - Detaches the debug tools.
* `--get-port` - Retrieves the port on which you are debugging your application.
* `--debug-port` - Sets a new port on which to attach the debug tools.

### Attributes
* `<Device ID>` is the index or name of the target device as listed by `$ tns list-devices` 
* `<Port>` is an accessible port on the device to which you want to attach the debugging tools.
* `<Emulator Options>` is any valid combination of options as listed by `$ tns help emulate android`
* `<GenyName>` is the name of the Genymotion virtual device that you want to use as listed by `$ genyshell -c "devices list"`
 
<% if(isHtml) { %> 
### Prerequisites

* You must have Chrome installed on your system.

### Related Commands

Command | Description
----------|----------
[build android](build-android.html) | Builds the project for Android and produces an APK that you can manually deploy on device or in the native emulator.
[build ios](build-ios.html) | Builds the project for iOS and produces an APP or IPA that you can manually deploy in the iOS Simulator or on device, respectively.
[build](build.html) | Builds the project for the selected target platform and produces an application package that you can manually deploy on device or in the native emulator.
[debug ios](debug-ios.html) | Debugs your project on a connected iOS device or in a native emulator.
[debug](debug.html) | Debugs your project on a connected device or in a native emulator.
[deploy](deploy.html) | Builds and deploys the project to a connected physical or virtual device.
[emulate android](emulate-android.html) | Builds the specified project and runs it in a native Android emulator.
[emulate ios](emulate-ios.html) | Builds the specified project and runs it in the native iOS Simulator.
[emulate](emulate.html) | You must run the emulate command with a related command.
[run android](run-android.html) | Runs your project on a connected Android device or in a native Android emulator, if configured.
[run ios](run-ios.html) | Runs your project on a connected iOS device or in the iOS Simulator, if configured.
[run](run.html) | Runs your project on a connected device or in the native emulator for the selected platform.
<% } %>