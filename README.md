# android-proguard

[![Build Status](https://cloud.drone.io/api/badges/v7lin/android-proguard/status.svg)](https://cloud.drone.io/v7lin/android-proguard)
[![GitHub tag](https://img.shields.io/github/tag/v7lin/android-proguard.svg)](https://github.com/v7lin/android-proguard/releases)
[![API](https://img.shields.io/badge/API-14%2B-brightgreen.svg?style=flat)](https://android-arsenal.com/api?level=14)

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
