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
Developed by:RAKESH KUMAR.S
Registeration Number :212221040137
*/
```
## ACTIVITY_MAIN.XML:

    <?xml version="1.0" encoding="utf-8"?>
                
    <androidx.constraintlayout.widget.ConstraintLayout xmlns:android="http://schemas.android.com/apk/res/android"
    
    xmlns:app="http://schemas.android.com/apk/res-auto"
    
    xmlns:tools="http://schemas.android.com/tools"
    
    android:layout_width="match_parent"
    
    android:layout_height="match_parent"
    
    android:rotationX="8"
    
    tools:context=".MainActivity">

    <TextView
    
        android:id="@+id/textView"
        
        android:layout_width="271dp"
        
        android:layout_height="54dp"
        
        android:layout_marginStart="156dp"
        
        android:layout_marginEnd="176dp"
        
        android:text="HELLO WORLD"
        
        android:textSize="40dp"
        
        app:layout_constraintEnd_toEndOf="parent"
        
        app:layout_constraintHorizontal_bias="0.491"
        
        app:layout_constraintStart_toStartOf="parent"
        
        tools:layout_editor_absoluteY="312dp" />


        </androidx.constraintlayout.widget.ConstraintLayout>






## MAINACTIVITY.JAVA:

        package com.example.androidlifecycle;
        
        import androidx.appcompat.app.AppCompatActivity;
        
        import android.annotation.SuppressLint;
        
        import android.os.Bundle;
        
        import android.widget.Toast;
        
        public class MainActivity extends AppCompatActivity
        
        {

    @Override
    
    protected void onCreate(Bundle savedInstanceState)
    
    {
    
        super.onCreate(savedInstanceState);
        
        setContentView(R.layout.activity_main);
        
        Toast.makeText(getApplicationContext(), "On Create Called", Toast.LENGTH_SHORT).show();
    
    }
    
    protected void onStart()
    
    {
    
        super.onStart();
        
        Toast.makeText(getApplicationContext(), "On Start Called ", Toast.LENGTH_SHORT).show();



    }
    
    protected void onRestart()
    
    {
    
        super.onRestart();
        
        Toast.makeText(getApplicationContext(), "On Restart Called", Toast.LENGTH_SHORT).show();
    }
    
    
    protected void onResume()
    
    {
    
        Toast.makeText(getApplicationContext(), "On Resume Called", Toast.LENGTH_SHORT).show();
        super.onResume();
    }
    
    
    protected void onStop()
    {
    
        super.onStop();
        
        Toast.makeText(getApplicationContext(), "On Stop Called", Toast.LENGTH_SHORT).show();
    }
    
    
    protected void onPause()
    
    {
    
        super.onPause();
        
        Toast.makeText(getApplicationContext(), "On Pause Called", Toast.LENGTH_SHORT).show();
    }
    
    
    protected void onDestroy()
    
    {
    
        super.onDestroy();
        
        
        Toast.makeText(getApplicationContext(), "On Destroy Called", Toast.LENGTH_SHORT).show();
    }
    
}

## OUTPUT

![image](https://github.com/Rakesh2k23/Mobile-Application-Development/assets/141472158/63d54a30-7d01-4ce1-af52-ca11f9b8bf6e)
![image](https://github.com/Rakesh2k23/Mobile-Application-Development/assets/141472158/1b2521aa-8f37-44e5-92ed-72a1026101a5)
![image](https://github.com/Rakesh2k23/Mobile-Application-Development/assets/141472158/1eddeaa7-9b3f-491b-bf10-f2a7aa87d578)
![image](https://github.com/Rakesh2k23/Mobile-Application-Development/assets/141472158/d626b85d-0d4f-4a06-ac09-90d52443cae0)
![image](https://github.com/Rakesh2k23/Mobile-Application-Development/assets/141472158/dff626a1-b71b-4ce9-a3fc-e15998a8aad7)
![image](https://github.com/Rakesh2k23/Mobile-Application-Development/assets/141472158/90adb70b-0b25-47c5-96d7-3b13d123c1ac)
![image](https://github.com/Rakesh2k23/Mobile-Application-Development/assets/141472158/ae2a53c5-5e66-45ce-91c9-80599f0e115c)



## RESULT
Thus a Simple Android Application create a HelloWorld Activity using all lifecycles methods to display messages using Android Studio is developed and executed successfully.
