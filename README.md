# ExoPlayer #

ExoPlayer is an application level media player for Android. It provides an
alternative to Android’s MediaPlayer API for playing audio and video both
locally and over the Internet. ExoPlayer supports features not currently
supported by Android’s MediaPlayer API, including DASH and SmoothStreaming
adaptive playbacks. Unlike the MediaPlayer API, ExoPlayer is easy to customize
and extend, and can be updated through Play Store application updates.

## Using ExoPlayer ##

#### Via jCenter ####

The easiest way to get started using ExoPlayer is by including the following in
your project's `build.gradle` file:

```gradle
compile 'com.google.android.exoplayer:exoplayer:rX.X.X'
```

where `rX.X.X` is the your preferred version. For the latest version, see the
project's [Releases][]. For more details, see the project on [Bintray][].

[Releases]: https://github.com/google/ExoPlayer/releases
[Bintray]: https://bintray.com/google/exoplayer/exoplayer/view

#### As source ####

ExoPlayer can also be built from source using Gradle. You can include it as a
dependent project like so:

```gradle
// settings.gradle
include ':app', ':..:ExoPlayer:library'

// app/build.gradle
dependencies {
    compile project(':..:ExoPlayer:library')
}
```

#### As a jar ####

If you want to use ExoPlayer as a jar, run:

```sh
./gradlew jarRelease
```

and copy `library.jar` to the libs folder of your new project.


#### Using Android Studio ####

To develop ExoPlayer using Android Studio, simply open the ExoPlayer project in
the root directory of the repository.
