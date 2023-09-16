# Ex.No:3 Develop program to create a text field and a button “Navigate”. When you enter “www.google.com” and press navigate button it should open google page using Implicit Intents.


## AIM:

To create a navigate button using Implicit Intent to display the google page using Android Studio.

## EQUIPMENTS REQUIRED:

Latest Version Android Studio

## ALGORITHM:

Step 1: Open Android Studio and then click on File -> New -> New project.

Step 2: Then type the Application name as HelloWorld and click Next.

Step 3: Then select the Minimum SDK as shown below and click Next.

Step 4: Then select the Empty Activity and click Next. Finally click Finish.

Step 5: Design layout in activity_main.xml.

Step 6: Display message give in MainActivity file.

Step 7: Save and run the application.

## PROGRAM:
```
/*
Program to print the text “Implicitintent”.
Developed by:Rakesh Kumar S
Registeration Number :212221040137
*/
```
## activity_main.xml :

<?xml version="1.0" encoding="utf-8"?>
<android.support.constraint.ConstraintLayout xmlns:android="http://schemas.android.com/apk/res/android"
    xmlns:app="http://schemas.android.com/apk/res-auto"
    xmlns:tools="http://schemas.android.com/tools"
    android:layout_width="match_parent"
    android:layout_height="match_parent"
    android:background="@color/purple_200"
    tools:context=".MainActivity">

    <Button
        android:id="@+id/button"
        android:layout_width="wrap_content"
        android:layout_height="wrap_content"
        android:layout_marginEnd="48dp"
        android:text="NAVIGATE"
        app:layout_constraintBottom_toBottomOf="parent"
        app:layout_constraintEnd_toEndOf="parent"
        app:layout_constraintTop_toTopOf="parent"
        app:layout_constraintVertical_bias="0.219" />

    <EditText
        android:id="@+id/editTextTextPersonName"
        android:layout_width="wrap_content"
        android:layout_height="wrap_content"
        android:layout_marginStart="32dp"
        android:ems="10"
        android:inputType="textPersonName"
        app:layout_constraintBottom_toBottomOf="parent"
        app:layout_constraintStart_toStartOf="parent"
        app:layout_constraintTop_toTopOf="parent"
        app:layout_constraintVertical_bias="0.218" />
</android.support.constraint.ConstraintLayout> 
## MainActivity.java :
package com.example.intent;

import android.support.v7.app.AppCompatActivity;
import android.os.Bundle;
import android.content.Intent;
import android.net.Uri;
import android.widget.Button;
import android.widget.EditText;

public class MainActivity extends AppCompatActivity {
    Button button;
    EditText editText;
    @Override
    protected void onCreate(Bundle savedInstanceState) {
        super.onCreate(savedInstanceState);
        setContentView(R.layout.activity_main);
        button = findViewById(R.id.button);
        editText = findViewById(R.id.editTextTextPersonName);
        button.setOnClickListener(view -> {
            String url=editText.getText().toString();
            Intent intent=new Intent(Intent.ACTION_VIEW, Uri.parse(url));
            startActivity(intent);
        });
    }
}


## OUTPUT


![image](https://github.com/Rakesh2k23/Mobile-Application-Development/assets/141472158/23f9c093-81ae-4c9c-a56c-5b1dd794043f)
![image](https://github.com/Rakesh2k23/Mobile-Application-Development/assets/141472158/4b774840-5da0-44db-92a7-db43c74bde8f)
![image](https://github.com/Rakesh2k23/Mobile-Application-Development/assets/141472158/3b1d48dc-04c0-4518-a554-15c6f901fc1f)





## RESULT
Thus a Simple Android Application create a navigate button using Implicit Intent to display the google page using Android Studio is developed and executed successfully.


