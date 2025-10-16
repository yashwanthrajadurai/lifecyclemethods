# Ex.No:2 To create a HelloWorld Activity using all lifecycles methods to display messages.

## AIM:
To create a HelloWorld Activity using all lifecycles methods to display messages using Android Studio.

## EQUIPMENTS REQUIRED:
Latest Version Android Studio

## ALGORITHM:
Step 1: Open Android Stdio and then click on File -> New -> New project.

Step 2: Then type the Application name as HelloWorld and click Next. 

Step 3: Then select the Minimum SDK as shown below and click Next.

Step 4: Then select the Empty Activity and click Next. Finally click Finish.

Step 5: Design layout in activity_main.xml.

Step 6: Display message give in MainActivity file.

Step 7: Save and run the application.

## PROGRAM:

```
/*
Program to print the text “Hello World”.
Developed by: YASHWANTH RAJA DURAI V
Registeration Number : 212222040184
*/
```

### In activitymain.xml

```
<?xml version="1.0" encoding="utf-8"?>
<androidx.constraintlayout.widget.ConstraintLayout xmlns:android="http://schemas.android.com/apk/res/android"
    xmlns:app="http://schemas.android.com/apk/res-auto"
    xmlns:tools="http://schemas.android.com/tools"
    android:layout_width="match_parent"
    android:layout_height="match_parent"
    tools:context=".MainActivity">

    <TextView
        android:layout_width="wrap_content"
        android:layout_height="wrap_content"
        android:fontFamily="cursive"
        android:text="Hello World!"
        android:textColor="#630C71"
        android:textSize="34sp"
        android:textStyle="bold"
        app:layout_constraintBottom_toBottomOf="parent"
        app:layout_constraintEnd_toEndOf="parent"
        app:layout_constraintStart_toStartOf="parent"
        app:layout_constraintTop_toTopOf="parent" />

</androidx.constraintlayout.widget.ConstraintLayout>
```
### In MainActivity.java
```
package com.example.methods;
import androidx.appcompat.app.AppCompatActivity;
import android.os.Bundle;
import android.widget.Toast;

public class MainActivity extends AppCompatActivity {
    @Override
    protected void onCreate(Bundle savedInstanceState) {
        super.onCreate(savedInstanceState);
        setContentView(R.layout.activity_main);
        Toast toast = Toast.makeText(getApplicationContext(), "onCreate Called", Toast.LENGTH_LONG);
        toast.show();
    }
    protected void onRestart() {
        // It will show a message on the screen
        // then onRestart is invoked
        super.onRestart();
        Toast toast = Toast.makeText(getApplicationContext(), "onRestart Called", Toast.LENGTH_LONG);
        toast.show();
    }
    protected void onResume() {
        // It will show a message on the screen
        // then onResume is invoked
        super.onResume();
        Toast toast = Toast.makeText(getApplicationContext(), "onResume Called", Toast.LENGTH_LONG);
        toast.show();
    }
    protected void onPause() {
        // It will show a message on the screen
        // then onPause is invoked
        super.onPause();
        Toast toast = Toast.makeText(getApplicationContext(), "onPause Called", Toast.LENGTH_LONG);
        toast.show();
    }
    protected void onStop() {
        // It will show a message on the screen
        // then onStop is invoked
        super.onStop();
        Toast toast = Toast.makeText(getApplicationContext(), "onStop Called", Toast.LENGTH_LONG);
        toast.show();
    }
    protected void onDestroy() {
        // It will show a message on the screen
        // then onDestroy is invoked
        super.onDestroy();
        Toast toast = Toast.makeText(getApplicationContext(), "onDestroy Called", Toast.LENGTH_LONG);
        toast.show();
    }
}
```
### In AndroidManifest.xml
```
<?xml version="1.0" encoding="utf-8"?>
<manifest xmlns:android="http://schemas.android.com/apk/res/android"
    xmlns:tools="http://schemas.android.com/tools">

    <application
        android:allowBackup="true"
        android:dataExtractionRules="@xml/data_extraction_rules"
        android:fullBackupContent="@xml/backup_rules"
        android:icon="@mipmap/ic_launcher"
        android:label="@string/app_name"
        android:roundIcon="@mipmap/ic_launcher_round"
        android:supportsRtl="true"
        android:theme="@style/Theme.Methods"
        tools:targetApi="31">
        <activity
            android:name=".MainActivity"
            android:exported="true">
            <intent-filter>
                <action android:name="android.intent.action.MAIN" />

                <category android:name="android.intent.category.LAUNCHER" />
            </intent-filter>
        </activity>
    </application>

</manifest>
```

## OUTPUT
![IMG-20240311-WA0006](https://github.com/AnnBlessy/lifecyclemethods/assets/119477835/d5a32035-8569-416f-af00-1691f3645c10)  ![IMG-20240311-WA0007](https://github.com/AnnBlessy/lifecyclemethods/assets/119477835/97d41ee3-c5b0-4d14-a4d2-fff59783f672) ![IMG-20240311-WA0008](https://github.com/AnnBlessy/lifecyclemethods/assets/119477835/63da561b-db79-4abe-889e-de895c597247)
![IMG-20240311-WA0009](https://github.com/AnnBlessy/lifecyclemethods/assets/119477835/a9eb0c0e-f461-41b8-ade8-a73756ee40ed) _ ![IMG-20240311-WA0010](https://github.com/AnnBlessy/lifecyclemethods/assets/119477835/bebd28a3-586e-4335-9a36-a43b0c152b78)

## RESULT
Thus a Simple Android Application create a HelloWorld Activity using all lifecycles methods to display messages using Android Studio is developed and executed successfully.
