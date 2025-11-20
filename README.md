# Ex.No:1 To create a HelloWorld Activity using all lifecycles methods to display messages.


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
Developed by:DHINESH R
Registeration Number :212223220019
*/
```
activity_main.xml
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
        android:text="Hello World"
        android:textColor="#673AB7"
        android:textColorHighlight="#0A1013"
        android:textColorHint="#4A3F3F"
        android:textColorLink="#2F3D43"
        android:textSize="34sp"
        app:layout_constraintBottom_toBottomOf="parent"
        app:layout_constraintEnd_toEndOf="parent"
        app:layout_constraintStart_toStartOf="parent"
        app:layout_constraintTop_toTopOf="parent"
        app:layout_constraintVertical_bias="0.179" />

```
Mainactivity.java
```
package com.example.exp1;
import android.os.Bundle;
import android.widget.Toast;
import androidx.appcompat.app.AppCompatActivity;

public class MainActivity extends AppCompatActivity {

    @Override
    protected void onCreate(Bundle savedInstanceState) {
        super.onCreate(savedInstanceState);
        setContentView(R.layout.activity_main);
        Toast toast = Toast.makeText(getApplicationContext(), "onCreate Called", Toast.LENGTH_LONG);
        toast.show();
    }
    protected void onStart() {
        super.onStart();
        Toast toast = Toast.makeText(getApplicationContext(), "onStart Called", Toast.LENGTH_LONG);
        toast.show();
    }
    @Override

    protected void onRestart() {
        super.onRestart();
        Toast toast = Toast.makeText(getApplicationContext(), "onRestart Called", Toast.LENGTH_LONG);
        toast.show();

    }
    protected void onPause() {
        super.onPause();
        Toast toast = Toast.makeText(getApplicationContext(), "onPause Called", Toast.LENGTH_LONG);
        toast.show();

    }
    protected void onResume(){
        super.onResume();
        Toast toast = Toast.makeText(getApplicationContext(), "onResume Called", Toast.LENGTH_LONG);
        toast.show();

    }
    protected void onStop() {
        super.onStop();
        Toast toast = Toast.makeText(getApplicationContext(), "onStop Called", Toast.LENGTH_LONG);
        toast.show();

    }
    protected void onDestroy() {
        super.onDestroy();
        Toast toast = Toast.makeText(getApplicationContext(), "onDestroy Called", Toast.LENGTH_LONG);
        toast.show();

    }
}
```

## OUTPUT
![Screenshot (81)](https://github.com/KayyuruTharani/lifecyclemethods/assets/142209319/d5ad46bc-1465-456a-9cf3-d8e3f94c8eae)

![Screenshot (82)](https://github.com/KayyuruTharani/lifecyclemethods/assets/142209319/2006d2ad-0051-4427-9d51-650b6cb39d8c)

![Screenshot (84)](https://github.com/KayyuruTharani/lifecyclemethods/assets/142209319/cbe15bc8-62d5-4c21-9e97-783d6b2216c0)

![Screenshot (66)](https://github.com/KayyuruTharani/lifecyclemethods/assets/142209319/0914167e-ec9a-4831-a64b-58da70413c2e)

![Screenshot (87)](https://github.com/KayyuruTharani/lifecyclemethods/assets/142209319/4f6aabbf-5352-48c1-aa83-400252741ca6)

![Screenshot (85)](https://github.com/KayyuruTharani/lifecyclemethods/assets/142209319/f482e7b7-1132-471e-8a78-aa6aa8415d01)

![Screenshot (86)](https://github.com/KayyuruTharani/lifecyclemethods/assets/142209319/10ef6e61-d7f4-40b2-a817-f863e06ea9c9)



## RESULT
Thus a Simple Android Application create a HelloWorld Activity using all lifecycles methods to display messages using Android Studio is developed and executed successfully.
