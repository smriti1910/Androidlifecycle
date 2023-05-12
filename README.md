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

## activity_main.xml
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
        android:textSize="20dp"
        app:layout_constraintBottom_toBottomOf="parent"
        app:layout_constraintEnd_toEndOf="parent"
        app:layout_constraintStart_toStartOf="parent"
        app:layout_constraintTop_toTopOf="parent" />

</androidx.constraintlayout.widget.ConstraintLayout>

```

## MainActivity.java
```
/*
Program to print text "Hello World."
Developed by: SMRITI .B
Registration Number: 212221040156
*/
import android.os.Bundle;
import android.widget.Toast;

public class MainActivity extends AppCompatActivity {

    @Override
    protected void onCreate(Bundle savedInstanceState) {
        super.onCreate(savedInstanceState);
        setContentView(R.layout.activity_main);
        Toast.makeText(this, "onCreate Called, Welcome Smriti", Toast.LENGTH_LONG).show();
    }

    @Override
    protected void onRestart(){
        Toast.makeText(this, "onRestart Called", Toast.LENGTH_LONG).show();
        super.onRestart();
    }
    @Override
    protected void onStart(){
        Toast.makeText(this, "onStart Called", Toast.LENGTH_LONG).show();

        super.onStart();
    }
    @Override
    protected void onResume(){
        Toast.makeText(this, "onResume Called", Toast.LENGTH_LONG).show();

        super.onResume();
    }
    @Override
    protected void onPause(){
        Toast.makeText(this, "onPause Called", Toast.LENGTH_LONG).show();

        super.onPause();
    }
    @Override
    protected void onStop(){
        Toast.makeText(this, "onStop Called", Toast.LENGTH_LONG).show();

        super.onStop();
    }
    @Override
    protected void onDestroy(){
        Toast.makeText(this, "onDestroy Called", Toast.LENGTH_SHORT).show();

        super.onDestroy();
    }
}
```

## OUTPUT
![Output](https://github.com/smriti1910/Androidlifecycle/assets/133334803/3bf39c5b-d238-4317-a8ed-b695e8638088)
![OnCreate()](https://github.com/smriti1910/Androidlifecycle/assets/133334803/b99a7ebd-678d-4acf-a085-1a298c8db02c)
![OnStart()](https://github.com/smriti1910/Androidlifecycle/assets/133334803/e7ae3fa9-5543-4d31-9cbd-4a4f3ca4d729)
![OnResume()](https://github.com/smriti1910/Androidlifecycle/assets/133334803/df3e2282-9067-42a7-8e25-ecf5b33401d9)
![OnPause()](https://github.com/smriti1910/Androidlifecycle/assets/133334803/d4dc8188-813b-489b-a9de-74091ee32d07)
![OnStop()](https://github.com/smriti1910/Androidlifecycle/assets/133334803/dcb97d0d-4ba7-4baa-a46e-8f2a3dd35f70)
![OnDestroy()](https://github.com/smriti1910/Androidlifecycle/assets/133334803/8a4573dc-fdbf-4d4b-8fc4-df5f0080add2)








## RESULT
Thus a Simple Android Application create a HelloWorld Activity using all lifecycles methods to display messages using Android Studio is developed and executed successfully.
