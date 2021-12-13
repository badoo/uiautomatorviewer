# uiautomatorviewer
Rebuild of UiAutomatorViewer app from the sources to make it compatible with modern JDK versions

## How to build
Just run `gradlew shadowJar` in project directory - it will give you build/libs/uiautomatorviewer-all.jar

## How to replace default uiautomatorviewer with this one
1. Copy uiautomatorviewer-all.jar into `%ANDROID_HOME%/tools/lib`
2. Replace `%ANDROID_HOME%/tools/bin/uiautomatorviewer` with uiautomatorviewer from `etc/uiautomatorviewer`

## **NOTICE**
This was tested only on macOS / Linux
