# MIUI Autostart
- MIUI 10 (firebase)
- MIUI 11 (physical device 11.0.9)
- MIUI 12 (physical device 12.5)
- MIUI 13 (untested, but works)
- MIUI 14 (physical device 14.0.2)


<b>But not limited for newer releases</b>

<hr>

## Setup

### Gradle

Add the JitPack repository to your build file

```groovy
repositories {
    maven { url 'https://jitpack.io' }
}
```

Add the dependency

```groovy
dependencies {
    implementation 'com.github.XomaDev:MIUI-autostart:v1.3'
}
```

### Maven

Add the JitPack repository to your build file

```html
<repositories>
    <repository>
        <id>jitpack.io</id>
        <url>https://jitpack.io</url>
    </repository>
</repositories>
```

Add the dependency

```html
<dependency>
    <groupId>com.github.XomaDev</groupId>
    <artifactId>MIUI-autostart</artifactId>
    <version>v1.3</version>
</dependency>
```

## Usage

It's recommended to use the Safe API, refer documentation

```kotlin
val enabled: Boolean = Autostart.getSafeState(context)
```
```java
boolean enabled = Autostart.INSTANCE.getSafeState(context);
```

Or using `isAutoStartEnabled(Context, DefaultValue)`
