# CHANGELOG

## [2.4.3] &mdash; 2018-05-23
- [Fixed] Fix link error when iOS and npm project name are diferent
- [Fixed] Clear event-listeners when `#configure` is called.  When used with `react-native-background-geolocation` in "Headless Mode", this plugin could accumulate event-listeners with each reboot after terminate.
- [Added] Add convenience method `BackgroundGeolocation#registerHeadlessTask`, to be used instead of `AppRegistry#registerHeadlessTask`.

## [2.4.2] &mdash; 2018-05-07
- [Added] Implement ability to provide `UIBackgroundFetchResult` to `#finish` rather than hard-coded `UIBackgroundFetchResultNewData`

## [2.4.1] &mdash; 2018-03-18
- [Fixed] react-native link was broken for iOS due to unused aggregate target.  Remove unused targets.

## [2.4.0] &mdash; 2018-02-27
- [Changed] The Android library `tsbackgroundfetch.aar` has be composed as a *Maven* repository.  The installation procedure has changed slightly now and `flatDirs` has been replaced with a `maven url`.  See the corresponding installation docs for more information.
- [Changed] Android will check for *application-wide configuration properties* `buildSdkVersion`, `buildToolsVersion`, `targetSdkVersion`.  See the Wiki "Solving Android Gradle Conflicts" for more information.

## [2.3.0] &mdash; 2018-01-22
- [Added] Android implementation using `JobScheduler` / `AlarmManager`

