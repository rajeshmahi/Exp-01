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
Developed by: Rajesh K 
Reg.no:212221220041
```
## activity_main.xml
```
<?xml version="1.0" encoding="utf-8"?>
<androidx.constraintlayout.widget.ConstraintLayout xmlns:android="http://schemas.android.com/apk/res/android"
    xmlns:app="http://schemas.android.com/apk/res-auto"
    xmlns:tools="http://schemas.android.com/tools"
    style="TIM"
    android:layout_width="match_parent"
    android:layout_height="match_parent"
    tools:context=".MainActivity">

    <TextView
        android:layout_width="wrap_content"
        android:layout_height="wrap_content"
        android:text="Hello World\nThis is Hiba...!!"
        android:textSize="30dp"
        android:textAppearance="@style/TextAppearance.AppCompat.Large"
        android:textColorHighlight="#FFFFFF"
        app:layout_constraintBottom_toBottomOf="parent"
        app:layout_constraintEnd_toEndOf="parent"
        app:layout_constraintHorizontal_bias="0.455"
        app:layout_constraintStart_toStartOf="parent"
        app:layout_constraintTop_toTopOf="parent"
        app:layout_constraintVertical_bias="0.407" />

</androidx.constraintlayout.widget.ConstraintLayout>
```
## MainActivity.java
```
package com.example.hiba;

import androidx.appcompat.app.AppCompatActivity;

import android.os.Bundle;
import android.widget.Toast;

public class MainActivity extends AppCompatActivity {

    @Override
    protected void onCreate(Bundle savedInstanceState) {
        super.onCreate(savedInstanceState);
        setContentView(R.layout.activity_main);
        Toast t2= Toast.makeText(getApplicationContext(),"OnCreate Executed",Toast.LENGTH_LONG);
        t2.show();
    }
    protected void onStart() {
        super.onStart();
        setContentView(R.layout.activity_main);
        Toast t2= Toast.makeText(getApplicationContext(),"OnStart Executed",Toast.LENGTH_LONG);
        t2.show();
    }
    protected void onResume() {
        super.onResume();
        setContentView(R.layout.activity_main);
        Toast t2= Toast.makeText(getApplicationContext(),"OnResume Executed",Toast.LENGTH_LONG);
        t2.show();
    }
    protected void onPause() {
        super.onPause();
        setContentView(R.layout.activity_main);
        Toast t2= Toast.makeText(getApplicationContext(),"OnPause Executed",Toast.LENGTH_LONG);
        t2.show();
    }
    protected void onRestart() {
        super.onRestart();
        setContentView(R.layout.activity_main);
        Toast t2= Toast.makeText(getApplicationContext(),"OnRestart Executed",Toast.LENGTH_LONG);
        t2.show();
    }
    protected void onDestroy() {
        super.onDestroy();
        setContentView(R.layout.activity_main);
        Toast t2= Toast.makeText(getApplicationContext(),"OnDestroy Executed",Toast.LENGTH_LONG);
        t2.show();
    }
}
```

## OUTPUT

![image](https://github.com/JaganSivakumaran/Experiment-1/assets/134905062/1c47447a-9a70-4e51-9099-8c3e959515a5)
![image](https://github.com/JaganSivakumaran/Experiment-1/assets/134905062/6abd7bc5-7965-4920-afb7-bdd9a8619542)



## RESULT
Thus a Simple Android Application create a HelloWorld Activity using all lifecycles methods to display messages using Android Studio is developed and executed successfully.
