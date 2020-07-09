# Native Android Project with React Native

## Description

This project is attempting to add react-native support to an already exising native android project using the instructions provided by https://reactnative.dev/docs/integration-with-existing-apps.

## Setup

1. yarn install
2. yarn start (to start bundler)
3. open android folder in android studio, sync build then run

## Instructions

- Click the react button to start the react-native activity and look at logcat to see the errors thrown.

### Errors:
```Error Log
com.blake.testreactnative D/SoLoader: About to load: libjscexecutor.so
com.blake.testreactnative D/SoLoader: libjscexecutor.so not found on /data/data/com.blake.testreactnative/lib-main
com.blake.testreactnative D/SoLoader: libjscexecutor.so found on /data/app/com.blake.testreactnative-QIGbyGF2mRQe_c1Zn8Rq4A==/lib/x86
com.blake.testreactnative D/SoLoader: Not resolving dependencies for libjscexecutor.so
com.blake.testreactnative E/SoLoader: Error when loading lib: dlopen failed: library "libjsc.so" not found lib hash: 37b75c7fd33e8c94378f65171f48bada search path is /data/app/com.blake.testreactnative-QIGbyGF2mRQe_c1Zn8Rq4A==/lib/x86
com.blake.testreactnative W/System.err: java.lang.UnsatisfiedLinkError: dlopen failed: library "libjsc.so" not found
com.blake.testreactnative W/System.err:     at com.facebook.soloader.SoLoader$1.load(SoLoader.java:374)
com.blake.testreactnative W/System.err:     at com.facebook.soloader.DirectorySoSource.loadLibraryFrom(DirectorySoSource.java:77)
com.blake.testreactnative W/System.err:     at com.facebook.soloader.DirectorySoSource.loadLibrary(DirectorySoSource.java:50)
com.blake.testreactnative W/System.err:     at com.facebook.soloader.ApplicationSoSource.loadLibrary(ApplicationSoSource.java:82)
com.blake.testreactnative W/System.err:     at com.facebook.soloader.SoLoader.doLoadLibraryBySoName(SoLoader.java:766)
com.blake.testreactnative W/System.err:     at com.facebook.soloader.SoLoader.loadLibraryBySoName(SoLoader.java:673)
com.blake.testreactnative W/System.err:     at com.facebook.soloader.SoLoader.loadLibrary(SoLoader.java:611)
com.blake.testreactnative W/System.err:     at com.facebook.soloader.SoLoader.loadLibrary(SoLoader.java:559)
com.blake.testreactnative W/System.err:     at com.facebook.react.ReactInstanceManagerBuilder.getDefaultJSExecutorFactory(ReactInstanceManagerBuilder.java:297)
com.blake.testreactnative W/System.err:     at com.facebook.react.ReactInstanceManagerBuilder.build(ReactInstanceManagerBuilder.java:270)
com.blake.testreactnative W/System.err:     at com.blake.testreactnative.MyReactActivity.onCreate(MyReactActivity.kt:52)
com.blake.testreactnative W/System.err:     at android.app.Activity.performCreate(Activity.java:7009)
com.blake.testreactnative W/System.err:     at android.app.Activity.performCreate(Activity.java:7000)
com.blake.testreactnative W/System.err:     at android.app.Instrumentation.callActivityOnCreate(Instrumentation.java:1214)
com.blake.testreactnative W/System.err:     at android.app.ActivityThread.performLaunchActivity(ActivityThread.java:2731)
com.blake.testreactnative W/System.err:     at android.app.ActivityThread.handleLaunchActivity(ActivityThread.java:2856)
com.blake.testreactnative W/System.err:     at android.app.ActivityThread.-wrap11(Unknown Source:0)
com.blake.testreactnative W/System.err:     at android.app.ActivityThread$H.handleMessage(ActivityThread.java:1589)
com.blake.testreactnative W/System.err:     at android.os.Handler.dispatchMessage(Handler.java:106)
com.blake.testreactnative W/System.err:     at android.os.Looper.loop(Looper.java:164)
com.blake.testreactnative W/System.err:     at android.app.ActivityThread.main(ActivityThread.java:6494)
com.blake.testreactnative W/System.err:     at java.lang.reflect.Method.invoke(Native Method)
com.blake.testreactnative W/System.err:     at com.android.internal.os.RuntimeInit$MethodAndArgsCaller.run(RuntimeInit.java:438)
com.blake.testreactnative W/System.err:     at com.android.internal.os.ZygoteInit.main(ZygoteInit.java:807)
com.blake.testreactnative E/SoLoader: couldn't find DSO to load: libjscexecutor.so caused by: dlopen failed: library "libjsc.so" not found result: 0
com.blake.testreactnative D/SoLoader: init exiting
com.blake.testreactnative D/NetworkSecurityConfig: No Network Security Config specified, using platform default
com.blake.testreactnative W/unknown:ReactNative: Packager connection already open, nooping.
com.blake.testreactnative D/EGL_emulation: eglMakeCurrent: 0xa3b85120: ver 3 0 (tinfo 0xa3b830d0)
com.blake.testreactnative D/EGL_emulation: eglMakeCurrent: 0xa3b85120: ver 3 0 (tinfo 0xa3b830d0)
com.blake.testreactnative D/EGL_emulation: eglMakeCurrent: 0xa3b85120: ver 3 0 (tinfo 0xa3b830d0)
com.blake.testreactnative D/EGL_emulation: eglMakeCurrent: 0xa3b85120: ver 3 0 (tinfo 0xa3b830d0)
com.blake.testreactnative D/EGL_emulation: eglMakeCurrent: 0xa3b85120: ver 3 0 (tinfo 0xa3b830d0)
com.blake.testreactnative I/chatty: uid=10080(com.blake.testreactnative) RenderThread identical 1 line
com.blake.testreactnative D/EGL_emulation: eglMakeCurrent: 0xa3b85120: ver 3 0 (tinfo 0xa3b830d0)
com.blake.testreactnative D/OpenGLRenderer: endAllActiveAnimators on 0x9016fc00 (RippleDrawable) with handle 0xa3b83b40
com.blake.testreactnative D/EGL_emulation: eglMakeCurrent: 0xa3b85120: ver 3 0 (tinfo 0xa3b830d0)
com.blake.testreactnative I/zygote: Do partial code cache collection, code=28KB, data=25KB
com.blake.testreactnative I/zygote: After code cache collection, code=27KB, data=24KB
com.blake.testreactnative I/zygote: Increasing code cache capacity to 128KB
com.blake.testreactnative D/EGL_emulation: eglMakeCurrent: 0xa3b85120: ver 3 0 (tinfo 0xa3b830d0)
com.blake.testreactnative D/SoLoader: About to load: libhermes.so
com.blake.testreactnative D/SoLoader: libhermes.so not found on /data/data/com.blake.testreactnative/lib-main
com.blake.testreactnative D/SoLoader: libhermes.so not found on /data/app/com.blake.testreactnative-QIGbyGF2mRQe_c1Zn8Rq4A==/lib/x86
com.blake.testreactnative D/SoLoader: libhermes.so not found on /vendor/lib
com.blake.testreactnative D/SoLoader: libhermes.so not found on /system/lib
com.blake.testreactnative E/SoLoader: couldn't find DSO to load: libhermes.so result: 0
com.blake.testreactnative E/AndroidRuntime: FATAL EXCEPTION: create_react_context
    Process: com.blake.testreactnative, PID: 6818
    java.lang.UnsatisfiedLinkError: couldn't find DSO to load: libhermes.so result: 0
        at com.facebook.soloader.SoLoader.doLoadLibraryBySoName(SoLoader.java:825)
        at com.facebook.soloader.SoLoader.loadLibraryBySoName(SoLoader.java:673)
        at com.facebook.soloader.SoLoader.loadLibrary(SoLoader.java:611)
        at com.facebook.soloader.SoLoader.loadLibrary(SoLoader.java:559)
        at com.facebook.hermes.reactexecutor.HermesExecutor.<clinit>(HermesExecutor.java:20)
        at com.facebook.hermes.reactexecutor.HermesExecutorFactory.create(HermesExecutorFactory.java:29)
        at com.facebook.react.ReactInstanceManager$5.run(ReactInstanceManager.java:1017)
        at java.lang.Thread.run(Thread.java:764)
com.blake.testreactnative D/SoLoader: About to load: libreactnativejni.so
com.blake.testreactnative D/SoLoader: libreactnativejni.so not found on /data/data/com.blake.testreactnative/lib-main
com.blake.testreactnative D/SoLoader: libreactnativejni.so found on /data/app/com.blake.testreactnative-QIGbyGF2mRQe_c1Zn8Rq4A==/lib/x86
com.blake.testreactnative D/SoLoader: Not resolving dependencies for libreactnativejni.so
com.blake.testreactnative D/SoLoader: Loaded: libreactnativejni.so
com.blake.testreactnative D/SoLoader: About to load: libfbjni.so
com.blake.testreactnative D/SoLoader: libfbjni.so not found on /data/data/com.blake.testreactnative/lib-main
com.blake.testreactnative D/SoLoader: libfbjni.so found on /data/app/com.blake.testreactnative-QIGbyGF2mRQe_c1Zn8Rq4A==/lib/x86
com.blake.testreactnative D/SoLoader: Not resolving dependencies for libfbjni.so
com.blake.testreactnative D/SoLoader: Loaded: libfbjni.so
```
