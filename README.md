# uiautomatorviewer
Rebuild of UiAutomatorViewer app from the sources to make it compatible with modern JDK versions

## How to build
Just run `gradlew shadowJar` in project directory - it will give you build/libs/uiautomatorviewer-all.jar

## How to replace default uiautomatorviewer with this one
1. Copy uiautomatorviewer-all.jar into `%ANDROID_HOME%/tools/lib`
2. Open `%ANDROID_HOME%/tools/bin/uiautomatorviewer`
3. Change string `$APP_HOME/lib/uiautomatorviewer-26.0.0-dev.jar` with `$APP_HOME/lib/uiautomatorviewer-all.jar`
4. Replace `-Djava.ext.dirs="$frameworkdir"` in the last string with `-classpath "$frameworkdir"`
