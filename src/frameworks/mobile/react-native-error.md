## Error
error Failed to install the app. Please accept all necessary Android SDK licenses using Android SDK Manager: "$ANDROID_HOME/tools/bin/sdkmanager --licenses". Run CLI 
with --verbose flag for more details.
Error: Command failed: gradlew.bat app:installDebug -PreactNativeDevServerPort=8081
FAILURE: Build failed with an exception.

* What went wrong:
Could not determine the dependencies of task ':app:installDebug'.
> Failed to install the following Android SDK packages as some licences have not been accepted.
     build-tools;28.0.3 Android SDK Build-Tools 28.0.3
     platforms;android-28 Android SDK Platform 28
  To build this project, accept the SDK license agreements and install the missing 
components using the Android Studio SDK Manager.
  Alternatively, to transfer the license agreements from one workstation to another, see http://d.android.com/r/studio-ui/export-licenses.html

  Using Android SDK: C:\Users\Rupesh\AppData\Local\Android\Sdk

* Try:
Run with --stacktrace option to get the stack trace. Run with --info or --debug option to get more log output. Run with --scan to get full insights.

* Get more help at https://help.gradle.org

BUILD FAILED in 2s

## Solution
- Go to `cd ~/Library/Android/sdk/tools/bin/` or OR PATH OF YOUR Android > sdk > tools > bin
- Then Run the sdkmanager as follows: `.\sdkmanager --licenses`
- Review Licenses
- Accept all of them