# EX NO : 01  LifeCycles Methods in Android Studio 

## DATE :  14/08/2023

## AIM:

To create a HelloWorld Activity using all lifecycles methods to display messages using Android Studio.

## EQUIPMENTS REQUIRED:

Latest Version Android Studio

## ALGORITHM:

### Step 1: 
Open Android Stdio and then click on File -> New -> New project.

### Step 2: 
Then type the Application name as HelloWorld and click Next. 

### Step 3: 
Then select the Minimum SDK as shown below and click Next.

### Step 4: 
Then select the Empty Activity and click Next. Finally click Finish.

### Step 5: 
Design layout in activity_main.xml.

### Step 6: 
Display message give in MainActivity file.

### Step 7: 
Save and run the application.



## PROGRAM:
```
Program to print the text “Hello World”.
Developed by: YUGENDARAN.G
Registeration Number :212221220063
```


## MainActivity.java:-
```
package com.example.helloworld;
import androidx.appcompat.app.AppCompatActivity;
import android.os.Bundle;
import android.util.Log;
import android.widget.Toast;

public class MainActivity extends AppCompatActivity {

    private static final String TAG = "HelloWorldActivity";

    @Override
    protected void onCreate(Bundle savedInstanceState) {
        super.onCreate(savedInstanceState);
        setContentView(R.layout.activity_main);
        Log.d(TAG, "onCreate: ");
        Toast.makeText(this, "onCreate", Toast.LENGTH_SHORT).show();
    }

    @Override
    protected void onStart() {
        super.onStart();
        Log.d(TAG, "onStart: ");
        Toast.makeText(this, "onStart", Toast.LENGTH_SHORT).show();
    }

    @Override
    protected void onResume() {
        super.onResume();
        Log.d(TAG, "onResume: ");
        Toast.makeText(this, "onResume", Toast.LENGTH_SHORT).show();
    }

    @Override
    protected void onPause() {
        super.onPause();
        Log.d(TAG, "onPause: ");
        Toast.makeText(this, "onPause", Toast.LENGTH_SHORT).show();
    }

    @Override
    protected void onStop() {
        super.onStop();
        Log.d(TAG, "onStop: ");
        Toast.makeText(this, "onStop", Toast.LENGTH_SHORT).show();
    }

    @Override
    protected void onDestroy() {
        super.onDestroy();
        Log.d(TAG, "onDestroy: ");
        Toast.makeText(this, "onDestroy", Toast.LENGTH_SHORT).show();
    }

    @Override
    protected void onRestart() {
        super.onRestart();
        Log.d(TAG, "onRestart: ");
        Toast.makeText(this, "onRestart", Toast.LENGTH_SHORT).show();
    }
}

```


## Activity_main.xml:-
```
<?xml version="1.0" encoding="utf-8"?>
<androidx.constraintlayout.widget.ConstraintLayout xmlns:android="http://schemas.android.com/apk/res/android"
    xmlns:app="http://schemas.android.com/apk/res-auto"
    xmlns:tools="http://schemas.android.com/tools"
    android:layout_width="match_parent"
    android:layout_height="match_parent"
    tools:context=".MainActivity">

    <TextView
        android:layout_width="238dp"
        android:layout_height="105dp"
        android:text="Hello World!"
        android:textSize="100px"
        android:textStyle="italic"
        app:layout_constraintBottom_toBottomOf="parent"
        app:layout_constraintEnd_toEndOf="parent"
        app:layout_constraintHorizontal_bias="0.591"
        app:layout_constraintStart_toStartOf="parent"
        app:layout_constraintTop_toTopOf="parent"
        app:layout_constraintVertical_bias="0.499" />

</androidx.constraintlayout.widget.ConstraintLayout>
```

## OUTPUT:

## onStart()
![image](https://github.com/Yugendaran/Mobile-Application-Development/assets/128135616/91bb271e-3cf6-4f44-98a1-f6904c3d4e9a)


## onCreate()
![image](https://github.com/Yugendaran/Mobile-Application-Development/assets/128135616/281372ab-37f9-4a4f-b49f-6da9e7488cae)


## onRestart()
![image](https://github.com/Yugendaran/Mobile-Application-Development/assets/128135616/23d0fc48-396f-413f-b5e9-2b116ce7702e)


## onPause()
![image](https://github.com/Yugendaran/Mobile-Application-Development/assets/128135616/a9c876d7-11d6-461b-b52e-c4089bbdff57)


## onResume()
![image](https://github.com/Yugendaran/Mobile-Application-Development/assets/128135616/c63affe3-b20f-4263-a2a2-9e347fe84fd3)


## onDestroy()
![image](https://github.com/Yugendaran/Mobile-Application-Development/assets/128135616/0548f65b-10fd-48d2-ad32-4b17e603194f)


## onStop()
![image](https://github.com/Yugendaran/Mobile-Application-Development/assets/128135616/21a84e4e-e569-4af4-aaaf-52a3ad0dcd67)


## RESULT:
Thus a Simple Android Application create a HelloWorld Activity using all lifecycles methods to display messages using Android Studio is developed and executed successfully.
