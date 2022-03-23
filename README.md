# Corrado
# General Info

- compileSdk 31
- minSdk 23
- targetSdk 31
- coroutineVersion 1.3.9-native-mt
- ktorVersion 1.6.7

<br />

# Installation

- Open your app or module's **build.gradle,** add the library in dependencies block

    ```groovy
    plugins {
    ...
    ...
    ...
    }
    android{
    ...
    ...
    ...
    }
    dependencies{
    ...
    ...
    def coroutineVersion = "1.3.9-native-mt"
    def ktorVersion = "1.6.7"
    implementation fileTree(dir: 'libs', include: ['.aar', '.jar'], exclude: [])
    implementation files('libs/shared-release.aar')
    implementation "org.jetbrains.kotlinx:kotlinx-coroutines-android:$coroutineVersion"
    implementation "org.jetbrains.kotlinx:kotlinx-coroutines-core:$coroutineVersion"
    implementation "io.ktor:ktor-client-core:$ktorVersion"
    implementation "io.ktor:ktor-client-android:$ktorVersion"
    implementation "org.jetbrains.kotlinx:kotlinx-serialization-json:1.0.1"

    }
    ```

- Permissions needed :
    ```

    ```
<br />
<br />

# Usage
