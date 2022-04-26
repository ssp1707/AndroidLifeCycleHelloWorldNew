# Ex.No:1 To create a HelloWorld Activity using all lifecycles methods to display messages.


## AIM:

To create a HelloWorld Activity using all lifecycles methods to display messages using Android Studio.

## EQUIPMENTS REQUIRED:

Android Studio(Min.required Artic Fox)

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
Developed by: S. Sanjna Priya
Registeration Number : 212220230043
*/
```
# MainActivity.java
```
package com.example.test;
        import androidx.appcompat.app.AppCompatActivity;
        import android.os.Bundle;
        import android.widget.Toast;
public class MainActivity extends AppCompatActivity {
    @Override
protected void onCreate(Bundle savedInstanceState) { super.onCreate(savedInstanceState); setContentView(R.layout.activity_main);
    Toast toast=Toast.makeText(getApplicationContext(),"OnCreate Invoked",Toast.LENGTH_LONG);
    toast.show();
}

    protected void onStart(){ super.onStart();
        Toast toast=Toast.makeText(getApplicationContext(),"OnStart Invoked",Toast.LENGTH_LONG);
        toast.show();
    }

    protected void onResume(){ super.onResume();
        Toast toast=Toast.makeText(getApplicationContext(),"OnResume Invoked",Toast.LENGTH_LONG);
        toast.show();
    }

    protected void onPause(){ super.onPause();
        Toast toast=Toast.makeText(getApplicationContext(),"OnPause Invoked",Toast.LENGTH_LONG);
        toast.show();
    }

    protected void onStop(){ super.onStop();
        Toast toast=Toast.makeText(getApplicationContext(),"OnStop Invoked",Toast.LENGTH_LONG);
        toast.show();
    }

    protected void onRestart(){ super.onRestart();

        Toast toast=Toast.makeText(getApplicationContext(),"OnRestart Invoked",Toast.LENGTH_LONG);
        toast.show();
    }

    protected void onDestroy(){ super.onDestroy();
        Toast toast=Toast.makeText(getApplicationContext(),"OnDestroy Invoked",Toast.LENGTH_LONG);
        toast.show();
    }
}
```

# activity_main.xml
```
<?xml version="1.0" encoding="utf-8"?>
<androidx.constraintlayout.widget.ConstraintLayout xmlns:android="http://schemas.android.com/apk/res/android"
    xmlns:app="http://schemas.android.com/apk/res-auto"
    xmlns:tools="http://schemas.android.com/tools"
    android:layout_width="match_parent"
    android:layout_height="match_parent"
    tools:context=".MainActivity">

    <TextView
        android:id="@+id/textView"
        android:layout_width="wrap_content"
        android:layout_height="wrap_content"
        android:text="Hello World"
        app:layout_constraintBottom_toBottomOf="parent"
        app:layout_constraintEnd_toEndOf="parent"
        app:layout_constraintStart_toStartOf="parent"
        app:layout_constraintTop_toTopOf="parent" />

</androidx.constraintlayout.widget.ConstraintLayout>
```

## OUTPUT
![image](https://user-images.githubusercontent.com/75234965/165213028-d18631e5-1b58-4b7b-a817-889d344530bd.png)
![image](https://user-images.githubusercontent.com/75234965/165213043-da63d629-346b-4dfa-ab80-08bc24c3b04c.png)
![image](https://user-images.githubusercontent.com/75234965/165213066-d58ba1b7-e169-4afc-b779-972ee6a24a57.png)
![image](https://user-images.githubusercontent.com/75234965/165213082-7daa806f-1f3c-4a45-8b91-bea4b469c01f.png)
![image](https://user-images.githubusercontent.com/75234965/165213096-9a9bd0e2-5470-4691-8cd6-c726a1a52142.png)
![image](https://user-images.githubusercontent.com/75234965/165213113-bd42ef45-8f13-4227-8186-eb7d9229e62d.png)

## RESULT
Thus a Simple Android Application create a HelloWorld Activity using all lifecycles methods to display messages using Android Studio is developed and executed successfully.
