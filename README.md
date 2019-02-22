# android-proguard

[![Build Status](https://cloud.drone.io/api/badges/v7lin/android-proguard/status.svg)](https://cloud.drone.io/v7lin/android-proguard)
[ ![Download](https://api.bintray.com/packages/v7lin/maven/proguard-android/images/download.svg) ](https://bintray.com/v7lin/maven/proguard-android/_latestVersion)

### 声明

通用混淆配置

### snapshot

````
ext {
    latestVersion = '1.0.0-SNAPSHOT'
}

allprojects {
    repositories {
        ...
        maven {
            url 'https://oss.jfrog.org/artifactory/oss-snapshot-local'
        }
        ...
    }
}
````

### release

````
ext {
    latestVersion = '1.0.0'
}

allprojects {
    repositories {
        ...
        jcenter()
        ...
    }
}
````

### usage

android
````
...
dependencies {
    ...
    implementation "io.github.v7lin:proguard-android:${latestVersion}"
    ...
}
...
````
