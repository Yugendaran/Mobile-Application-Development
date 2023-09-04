# Ex.No: 2 To develop an application that uses GUI Components with Fonts and Colors. 
Note: Create button for colors and fonts while clicking color or font button should change 


## AIM:

To create an application that uses GUI Components with Fonts and Colors using Android Studio.

## EQUIPMENTS REQUIRED:

Latest Version Android Studio

## ALGORITHM:
step 1: Open Android Stdio and then click on File -> New -> New project.

Step 2: Then type the Application name as Button color  and click Next.

Step 3: Then select the Minimum SDK as shown below and click Next.

Step 4: Then select the Empty Activity and click Next. Finally click Finish.

Step 5: Design layout in activity_main.xml.

Step 6: Display message give in MainActivity file.

Step 7: Save and run the application.

## PROGRAM:
```
/*
Program to print the text “GUIcomponent”.
Developed by: Yugendaran G
Registeration Number : 212221220063
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
MainActivity.java
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
![image](https://github.com/Yugendaran/Mobile-Application-Development/assets/128135616/a9cf80f7-09a0-46d5-b988-18f87da25726)

![image](https://github.com/Yugendaran/Mobile-Application-Development/assets/128135616/568488d2-546d-45d4-89a9-cb0810e4ece1)





## RESULT
Thus a Simple Android Application that uses GUI Components with Fonts and Colors using Android Studio is developed and executed successfully.


