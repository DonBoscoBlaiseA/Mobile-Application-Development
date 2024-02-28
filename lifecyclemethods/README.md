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
Developed by: Don Bosco Blaise A
Registeration Number : 212221040045
*/
```
## ACTIVITY_MAIN.XML:
```
<?xml version="1.0" encoding="utf-8"?>
<androidx.constraintlayout.widget.ConstraintLayout xmlns:android="http://schemas.android.com/apk/res/android"
    xmlns:app="http://schemas.android.com/apk/res-auto"
    xmlns:tools="http://schemas.android.com/tools"
    android:layout_width="match_parent"
    android:layout_height="match_parent"
    android:background="#EDE177"
    tools:context=".MainActivity">

    <TextView
        android:id="@+id/textView"
        android:layout_width="wrap_content"
        android:layout_height="wrap_content"
        android:text="@string/app_name"
        android:textColor="#F40B0B"
        android:textSize="40sp"
        android:textStyle="bold"
        app:layout_constraintBottom_toBottomOf="parent"
        app:layout_constraintEnd_toEndOf="parent"
        app:layout_constraintStart_toStartOf="parent"
        app:layout_constraintTop_toTopOf="parent" />

</androidx.constraintlayout.widget.ConstraintLayout>
```
## MAINACTIVITY.JAVA:
```
package com.example.helloworld;

import androidx.appcompat.app.AppCompatActivity;

import android.os.Bundle;
import android.widget.Toast;

public class MainActivity extends AppCompatActivity {

    @Override
    protected void onCreate(Bundle savedInstanceState) {
        super.onCreate(savedInstanceState);
        setContentView(R.layout.activity_main);

        Toast.makeText(getApplicationContext(), "OnCreate called", Toast.LENGTH_LONG).show();
    }
    protected void onStart(){
        super.onStart();
        Toast toast = Toast.makeText(getApplicationContext(), "OnStart called", Toast.LENGTH_LONG);
        toast.show();
    }
    protected void onRestart(){
        super.onRestart();
        Toast toast = Toast.makeText(getApplicationContext(), "OnRestart called", Toast.LENGTH_LONG);
        toast.show();
    }
    protected void onStop(){
        super.onStop();
        Toast toast = Toast.makeText(getApplicationContext(), "OnStop called", Toast.LENGTH_LONG);
        toast.show();
    }
    protected void onPause(){
        super.onPause();
        Toast toast = Toast.makeText(getApplicationContext(), "OnPause called", Toast.LENGTH_LONG);
        toast.show();
    }
    protected void onDestroy(){
        super.onDestroy();
        Toast toast = Toast.makeText(getApplicationContext(), "OnDestroy called", Toast.LENGTH_LONG);
        toast.show();
    }
}
```


## OUTPUT
![Screenshot (203)](https://github.com/DonBoscoBlaiseA/Mobile-Application-Development/assets/140850829/98db8968-3eb1-42ce-b701-51391f00513e)
![Screenshot (204)](https://github.com/DonBoscoBlaiseA/Mobile-Application-Development/assets/140850829/dd0fe4c9-1559-4db7-9923-b965bac2e8d8)
![Op1](https://github.com/DonBoscoBlaiseA/Mobile-Application-Development/assets/140850829/7fb45310-b6f0-4762-aa06-2921a9217e72)
![Op2](https://github.com/DonBoscoBlaiseA/Mobile-Application-Development/assets/140850829/d5e0f809-22e5-40c6-b446-18a24810d1f3)
![Op3](https://github.com/DonBoscoBlaiseA/Mobile-Application-Development/assets/140850829/1b5eca00-017e-4d7a-b6ef-39c4a9bd6621)
![Op4](https://github.com/DonBoscoBlaiseA/Mobile-Application-Development/assets/140850829/c0094a15-7aa1-4b4f-bda6-aa02d55e6823)
![Op5](https://github.com/DonBoscoBlaiseA/Mobile-Application-Development/assets/140850829/85cb8a10-5fde-4b91-ab06-385ee004a987)


## RESULT
Thus a Simple Android Application create a HelloWorld Activity using all lifecycles methods to display messages using Android Studio is developed and executed successfully.
