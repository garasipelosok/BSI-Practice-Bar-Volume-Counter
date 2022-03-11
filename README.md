# BSI-Practice-Bar-Volume-Counter
This repository is source code of Mobile Programming Course for Activity Practice using Android Studio in BSI University

Run single activity using:
```
onCreate();
```

Keeping Hasil | Result when changing display orientation using: 
```
onSaveInstanceState();
savedInstanceState();
```

Steps
 1. Create new Project
 2. Choose no activity
 6. file -> new -> activity -> empty activity -> activity name[MainActivity], layout name[activity_main], pacagename[auto], language[java] 
 3. file -> new -> XML -> Layout XML file -> Layout file name [activity_main] -> this for manually generated 
 4. on yellow light android:text="Panjang" alt+enter Extract string resource, to add value into strings
 5. file -> new -> value source file -> filename[dimens], source set[main], directory name[values] -> ok | res/values/dimens.xml ->setting centralize resource value
 6. if error "Could not identify launch activity: Default Activity not found" try to edit AndroidManifest.xml

```
<?xml version="1.0" encoding="utf-8"?>
<manifest xmlns:android="http://schemas.android.com/apk/res/android"
    package="com.garasipelosok.bsipractice_barvolume">

    <application
        android:allowBackup="true"
        android:icon="@mipmap/ic_launcher"
        android:label="@string/app_name"
        android:roundIcon="@mipmap/ic_launcher_round"
        android:supportsRtl="true"
        android:theme="@style/Theme.BSIPracticeBarVolume">

        <activity
            android:name="com.garasipelosok.bsipractice_barvolume.MainActivity"
            android:exported="true">
<!--  As of Android 12, `android:exported` must be set; use `true` to make the activity \<br/> available to other apps, and `false` otherwise. For launcher activities, this should be set to `true`. -->
            <intent-filter>
                <action android:name="android.intent.action.MAIN" />
                <category android:name="android.intent.category.LAUNCHER" />
            </intent-filter>
        </activity>
    </application>
</manifest>
```
