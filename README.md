# Expo Android Build Failure: Gradle Version Mismatch

This repository demonstrates a common yet difficult-to-diagnose issue encountered when building Android APKs using the Expo CLI. The problem stems from a mismatch between the Gradle plugin version specified in the project's `android/build.gradle` file and the version required or expected by the Expo build system. 

**Problem:**
The Expo build process might fail without clear indication of an underlying Gradle version incompatibility.  Error messages may be vague, leading to significant troubleshooting time. This example showcases a scenario where this occurs.

**Solution:**
The solution involves carefully reviewing and updating the Gradle plugin version in the `android/build.gradle` file. The specific version needed might depend on the Expo CLI version and other project dependencies.  The example shows how to resolve this by correcting the Gradle plugin version. 

**Steps to reproduce:**
1. Clone this repository.
2. Navigate to the `android` directory.
3. Try to build the project using the Expo CLI (you'll likely encounter the error).
4. Replace the incorrect `build.gradle` with the fixed version.
5. Try building again; the build should now succeed.