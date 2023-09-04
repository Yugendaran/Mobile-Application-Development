# Ex.No: 2 To develop an application that uses GUI Components with Fonts and Colors. 
Note: Create button for colors and fonts while clicking color or font button should change 


## AIM:

To create an application that uses GUI Components with Fonts and Colors using Android Studio.

## EQUIPMENTS REQUIRED:

Latest Version Android Studio

## ALGORITHM:


## PROGRAM:
```
/*
Program to print the text “GUIcomponent”.
Developed by:
Registeration Number :
*/
```
activity_main.xml
```
<?xml version="1.0" encoding="utf-8"?>
<androidx.constraintlayout.widget.ConstraintLayout xmlns:android="http://schemas.android.com/apk/res/android"
    xmlns:app="http://schemas.android.com/apk/res-auto"
    xmlns:tools="http://schemas.android.com/tools"
    android:id="@+id/bg"
    android:layout_width="match_parent"
    android:layout_height="match_parent"
    android:background="#FF9191"
    tools:context=".MainActivity">

    <TextView
        android:id="@+id/tv1"
        android:layout_width="wrap_content"
        android:layout_height="wrap_content"
        android:layout_marginTop="92dp"
        android:text="Color Change on button click"
        android:textColor="#FF1010"
        android:textSize="24sp"
        android:textStyle="bold"
        app:layout_constraintEnd_toEndOf="parent"
        app:layout_constraintHorizontal_bias="0.47"
        app:layout_constraintStart_toStartOf="parent"
        app:layout_constraintTop_toTopOf="parent" />

    <Button
        android:id="@+id/bt1"
        android:layout_width="158dp"
        android:layout_height="59dp"
        android:layout_marginStart="128dp"
        android:layout_marginTop="332dp"
        android:text="Color Changer"
        app:layout_constraintStart_toStartOf="parent"
        app:layout_constraintTop_toTopOf="parent" />
</androidx.constraintlayout.widget.ConstraintLayout>
```

MainActivty.java
```
package com.example.exercise2;

import androidx.appcompat.app.AppCompatActivity;
import androidx.constraintlayout.widget.ConstraintLayout;

import android.graphics.Color;
import android.os.Bundle;
import android.view.View;
import android.widget.Button;
import android.widget.TextView;
import android.widget.Toast;

public class MainActivity extends AppCompatActivity {

    Button Color_Changer;
    ConstraintLayout bg2;
    TextView tv1;
    @Override
    protected void onCreate(Bundle savedInstanceState) {
        super.onCreate(savedInstanceState);
        setContentView(R.layout.activity_main);

        Color_Changer = findViewById(R.id.bt1);
        bg2 = findViewById(R.id.bg);
        tv1= findViewById(R.id.tv1);

        Color_Changer.setOnClickListener(new View.OnClickListener() {
            @Override
            public void onClick(View view) {
                Toast.makeText(MainActivity.this, "button clicked", Toast.LENGTH_SHORT).show();

                bg2.setBackgroundColor(Color.BLACK);
                tv1.setTextColor(Color.CYAN);

                tv1.setTextSize(30);
            }
        });


    }
}
```

## OUTPUT

![image](https://github.com/suryacse05/Mobile-Application-Development/assets/128135616/d66d0743-7ea6-47ad-adb0-d9bba022c309)

![Uploading image.png…]()




## RESULT
Thus a Simple Android Application that uses GUI Components with Fonts and Colors using Android Studio is developed and executed successfully.


