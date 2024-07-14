
# FIREBASE LOGIN AND REGISTRATION SYSTEM

CREATED BY NOYON BISWAS

![esport_24_logo](https://github.com/user-attachments/assets/0478002c-4abf-4a96-a718-7c1dacf93a83)

##  First Connected Firebase
#### 1.Make Realtime Database and sclect Test(2nd)
#### 2.Authentication On(Email and Phone)
#### 3.Put Jeson File In App


# LOG IN .XML Part = STEP : 1  

   ```bash

<?xml version="1.0" encoding="utf-8"?>
<androidx.constraintlayout.widget.ConstraintLayout xmlns:android="http://schemas.android.com/apk/res/android"
    xmlns:app="http://schemas.android.com/apk/res-auto"
    xmlns:tools="http://schemas.android.com/tools"
    android:layout_width="match_parent"
    android:layout_height="match_parent"
    android:background="@drawable/one"
    tools:context=".login">

    <de.hdodenhof.circleimageview.CircleImageView
        android:id="@+id/profilerg0"
        android:layout_width="202dp"
        android:layout_height="178dp"
        android:src="@drawable/esport_512_logo"
        app:layout_constraintBottom_toBottomOf="parent"
        app:layout_constraintEnd_toEndOf="parent"
        app:layout_constraintHorizontal_bias="0.497"
        app:layout_constraintStart_toStartOf="parent"
        app:layout_constraintTop_toTopOf="parent"
        app:layout_constraintVertical_bias="0.122" />

    <TextView
        android:id="@+id/textView3"
        android:layout_width="@dimen/_298sdp"
        android:layout_height="@dimen/_166sdp"
        android:gravity="center"
        android:text="Log In"
        android:textSize="@dimen/_60sdp"
        android:textStyle="bold"
        app:layout_constraintBottom_toBottomOf="parent"
        app:layout_constraintEnd_toEndOf="parent"
        app:layout_constraintHorizontal_bias="0.495"
        app:layout_constraintStart_toStartOf="parent"
        app:layout_constraintTop_toTopOf="parent"
        app:layout_constraintVertical_bias="0.435" />

    <TextView
        android:id="@+id/textView4"
        android:layout_width="@dimen/_227sdp"
        android:layout_height="@dimen/_90sdp"
        android:gravity="center"
        android:text="Sing In To Continue"
        android:textSize="@dimen/_20sdp"
        android:textStyle="bold"
        app:layout_constraintBottom_toBottomOf="parent"
        app:layout_constraintEnd_toEndOf="parent"
        app:layout_constraintStart_toStartOf="parent"
        app:layout_constraintTop_toTopOf="parent"
        app:layout_constraintVertical_bias="0.544" />

    <TextView

        android:layout_width="138dp"
        android:layout_height="46dp"
        android:gravity="center"
        android:text="Email"
        android:textSize="@dimen/_20sdp"
        android:textStyle="bold"
        app:layout_constraintBottom_toBottomOf="parent"
        app:layout_constraintEnd_toEndOf="parent"
        app:layout_constraintHorizontal_bias="0.0"
        app:layout_constraintStart_toStartOf="parent"
        app:layout_constraintTop_toTopOf="parent"
        app:layout_constraintVertical_bias="0.604" />

    <EditText
        android:id="@+id/edlogemail"
        android:layout_width="@dimen/_260sdp"
        android:layout_height="wrap_content"
        android:ems="10"
        android:hint="Email"
        android:inputType="textEmailAddress"
        app:layout_constraintBottom_toBottomOf="parent"
        app:layout_constraintEnd_toEndOf="parent"
        app:layout_constraintHorizontal_bias="0.493"
        app:layout_constraintStart_toStartOf="parent"
        app:layout_constraintTop_toTopOf="parent"
        app:layout_constraintVertical_bias="0.67" />

    <TextView

        android:layout_width="173dp"
        android:layout_height="42dp"
        android:gravity="center"
        android:text="Password"
        android:textSize="@dimen/_20sdp"
        android:textStyle="bold"
        app:layout_constraintBottom_toBottomOf="parent"
        app:layout_constraintEnd_toEndOf="parent"
        app:layout_constraintHorizontal_bias="0.042"
        app:layout_constraintStart_toStartOf="parent"
        app:layout_constraintTop_toTopOf="parent"
        app:layout_constraintVertical_bias="0.722" />

    <EditText
        android:id="@+id/edlogpass"
        android:layout_width="@dimen/_260sdp"
        android:layout_height="wrap_content"
        android:ems="10"
        android:inputType="textPassword"
        app:layout_constraintBottom_toBottomOf="parent"
        app:layout_constraintEnd_toEndOf="parent"
        app:layout_constraintHorizontal_bias="0.493"
        app:layout_constraintStart_toStartOf="parent"
        app:layout_constraintTop_toTopOf="parent"
        app:layout_constraintVertical_bias="0.787"
        android:hint="Password"/>

    <Button
        android:id="@+id/btnlog"
        android:layout_width="@dimen/_300sdp"
        android:layout_height="wrap_content"
        android:text="LOG IN"
        android:backgroundTint="@color/black"
        android:textSize="@dimen/_20sdp"
        android:textStyle="bold"
        app:layout_constraintBottom_toBottomOf="parent"
        app:layout_constraintEnd_toEndOf="parent"
        app:layout_constraintHorizontal_bias="0.471"
        app:layout_constraintStart_toStartOf="parent"
        app:layout_constraintTop_toTopOf="parent"
        app:layout_constraintVertical_bias="0.897" />

    <TextView
        android:id="@+id/textView5"
        android:layout_width="wrap_content"
        android:layout_height="wrap_content"
        android:layout_marginEnd="148dp"
        android:text="Need an Account?"
        app:layout_constraintBottom_toBottomOf="parent"
        app:layout_constraintEnd_toEndOf="parent"
        app:layout_constraintTop_toTopOf="parent"
        app:layout_constraintVertical_bias="0.939" />

    <TextView
        android:id="@+id/tx_singup"
        android:layout_width="wrap_content"
        android:layout_height="wrap_content"
        android:layout_marginEnd="156dp"
        android:text="Sing Up?"
        android:textSize="@dimen/_20sdp"
        android:textStyle="bold"
        app:layout_constraintBottom_toBottomOf="parent"
        app:layout_constraintEnd_toEndOf="parent"
        app:layout_constraintTop_toTopOf="parent"
        app:layout_constraintVertical_bias="0.988" />
</androidx.constraintlayout.widget.ConstraintLayout>



```

## REGISTRATION XML STEP : 2



   ```bash

<?xml version="1.0" encoding="utf-8"?>
<androidx.constraintlayout.widget.ConstraintLayout xmlns:android="http://schemas.android.com/apk/res/android"
    xmlns:app="http://schemas.android.com/apk/res-auto"
    xmlns:tools="http://schemas.android.com/tools"
    android:layout_width="match_parent"
    android:layout_height="match_parent"
    tools:context=".registration"
    android:background="@drawable/two">

    <de.hdodenhof.circleimageview.CircleImageView
        android:id="@+id/imageprofile"
        android:layout_width="151dp"
        android:layout_height="130dp"
        android:src="@drawable/esport_512_logo"
        app:layout_constraintBottom_toBottomOf="parent"
        app:layout_constraintEnd_toEndOf="parent"
        app:layout_constraintHorizontal_bias="0.538"
        app:layout_constraintStart_toStartOf="parent"
        app:layout_constraintTop_toTopOf="parent"
        app:layout_constraintVertical_bias="0.232" />

    <TextView
        android:id="@+id/textView3"
        android:layout_width="232dp"
        android:layout_height="85dp"
        android:gravity="center"
        android:text="Create New"
        android:textColor="@color/white"
        android:textSize="@dimen/_30sdp"
        android:textStyle="bold"
        app:layout_constraintBottom_toBottomOf="parent"
        app:layout_constraintEnd_toEndOf="parent"
        app:layout_constraintHorizontal_bias="0.0"
        app:layout_constraintStart_toStartOf="parent"
        app:layout_constraintTop_toTopOf="parent"
        app:layout_constraintVertical_bias="0.0" />

    <TextView
        android:id="@+id/textView4"
        android:layout_width="189dp"
        android:layout_height="44dp"
        android:gravity="center"
        android:text="New Account"
        android:textColor="@color/white"
        android:textSize="@dimen/_20sdp"
        android:textStyle="bold"
        app:layout_constraintBottom_toBottomOf="parent"
        app:layout_constraintEnd_toEndOf="parent"
        app:layout_constraintHorizontal_bias="0.0"
        app:layout_constraintStart_toStartOf="parent"
        app:layout_constraintTop_toTopOf="parent"
        app:layout_constraintVertical_bias="0.096" />

    <TextView

        android:layout_width="107dp"
        android:layout_height="49dp"
        android:gravity="center"
        android:text="Email"
        android:textSize="@dimen/_20sdp"
        android:textStyle="bold"
        app:layout_constraintBottom_toBottomOf="parent"
        app:layout_constraintEnd_toEndOf="parent"
        app:layout_constraintHorizontal_bias="0.141"
        app:layout_constraintStart_toStartOf="parent"
        app:layout_constraintTop_toTopOf="parent"
        app:layout_constraintVertical_bias="0.548" />

    <TextView

        android:id="@+id/textView6"
        android:layout_width="wrap_content"
        android:layout_height="@dimen/_40sdp"
        android:gravity="center"
        android:text="Username"
        android:textSize="@dimen/_20sdp"

        android:textStyle="bold"
        app:layout_constraintBottom_toBottomOf="parent"
        app:layout_constraintEnd_toEndOf="parent"
        app:layout_constraintHorizontal_bias="0.054"
        app:layout_constraintStart_toStartOf="parent"
        app:layout_constraintTop_toTopOf="parent"
        app:layout_constraintVertical_bias="0.437" />

    <EditText
        android:id="@+id/edrgemail"
        android:layout_width="@dimen/_170sdp"
        android:layout_height="wrap_content"
        android:ems="10"
        android:hint="Email"
        android:inputType="textEmailAddress"
        app:layout_constraintBottom_toBottomOf="parent"
        app:layout_constraintEnd_toEndOf="parent"
        app:layout_constraintHorizontal_bias="0.81"
        app:layout_constraintStart_toStartOf="parent"
        app:layout_constraintTop_toTopOf="parent"
        app:layout_constraintVertical_bias="0.545" />

    <TextView

        android:layout_width="@dimen/_128sdp"
        android:layout_height="@dimen/_62sdp"
        android:gravity="center"
        android:text="Password"
        android:textSize="@dimen/_20sdp"
        android:textStyle="bold"
        app:layout_constraintBottom_toBottomOf="parent"
        app:layout_constraintEnd_toEndOf="parent"
        app:layout_constraintHorizontal_bias="0.035"
        app:layout_constraintStart_toStartOf="parent"
        app:layout_constraintTop_toTopOf="parent"
        app:layout_constraintVertical_bias="0.632" />

    <TextView

        android:layout_width="@dimen/_128sdp"
        android:layout_height="@dimen/_62sdp"
        android:gravity="center"
        android:text="Re-Password"
        android:textSize="@dimen/_20sdp"
        android:textStyle="bold"
        app:layout_constraintBottom_toBottomOf="parent"
        app:layout_constraintEnd_toEndOf="parent"
        app:layout_constraintHorizontal_bias="0.042"
        app:layout_constraintStart_toStartOf="parent"
        app:layout_constraintTop_toTopOf="parent"
        app:layout_constraintVertical_bias="0.747" />

    <EditText
        android:id="@+id/edrgpass"
        android:layout_width="@dimen/_170sdp"
        android:layout_height="wrap_content"
        android:ems="10"
        android:hint="Password"
        android:inputType="textPassword"
        app:layout_constraintBottom_toBottomOf="parent"
        app:layout_constraintEnd_toEndOf="parent"
        app:layout_constraintHorizontal_bias="0.847"
        app:layout_constraintStart_toStartOf="parent"
        app:layout_constraintTop_toTopOf="parent"
        app:layout_constraintVertical_bias="0.641" />

    <EditText
        android:id="@+id/edrgrepass"
        android:layout_width="@dimen/_170sdp"
        android:layout_height="wrap_content"
        android:ems="10"
        android:hint="Password"
        android:inputType="textPassword"
        app:layout_constraintBottom_toBottomOf="parent"
        app:layout_constraintEnd_toEndOf="parent"
        app:layout_constraintHorizontal_bias="0.852"
        app:layout_constraintStart_toStartOf="parent"
        app:layout_constraintTop_toTopOf="parent"
        app:layout_constraintVertical_bias="0.74" />

    <Button
        android:id="@+id/btnreg"
        android:layout_width="@dimen/_300sdp"
        android:layout_height="wrap_content"
        android:text="Sing Up"
        android:backgroundTint="@color/black"
        android:textSize="@dimen/_20sdp"
        android:textStyle="bold"
        app:layout_constraintBottom_toBottomOf="parent"
        app:layout_constraintEnd_toEndOf="parent"
        app:layout_constraintHorizontal_bias="0.471"
        app:layout_constraintStart_toStartOf="parent"
        app:layout_constraintTop_toTopOf="parent"
        app:layout_constraintVertical_bias="0.897" />


    <TextView

        android:id="@+id/rglogin"
        android:layout_width="wrap_content"
        android:layout_height="wrap_content"
        android:layout_marginEnd="152dp"
        android:text="Log In"
        android:textSize="@dimen/_20sdp"
        android:textStyle="bold"
        app:layout_constraintBottom_toBottomOf="parent"
        app:layout_constraintEnd_toEndOf="parent"
        app:layout_constraintTop_toTopOf="parent"
        app:layout_constraintVertical_bias="0.977" />

    <EditText
        android:id="@+id/edrgusername"
        android:layout_width="wrap_content"
        android:layout_height="wrap_content"
        android:ems="10"
        android:inputType="text"

        app:layout_constraintBottom_toBottomOf="parent"
        app:layout_constraintEnd_toEndOf="parent"
        app:layout_constraintHorizontal_bias="0.756"
        app:layout_constraintStart_toStartOf="parent"
        app:layout_constraintTop_toTopOf="parent"
        app:layout_constraintVertical_bias="0.432" />

</androidx.constraintlayout.widget.ConstraintLayout>

   ```

# Java Part Started

## Log In With java = STEP : 1



   ```bash
package com.example.test;

import androidx.annotation.NonNull;
import androidx.appcompat.app.AppCompatActivity;

import android.content.Intent;
import android.os.Bundle;
import android.text.TextUtils;
import android.view.View;
import android.widget.Button;
import android.widget.EditText;
import android.widget.TextView;
import android.widget.Toast;

import com.google.android.gms.tasks.OnCompleteListener;
import com.google.android.gms.tasks.Task;
import com.google.firebase.auth.AuthResult;
import com.google.firebase.auth.FirebaseAuth;

public class login extends AppCompatActivity {



    Button btnlog;
    EditText edlogemail,edlogpass;
     FirebaseAuth auth;
     TextView tx_singup;

    String emailPattern = "^[\\w.-]+@[\\w.-]+\\.[a-zA-Z]{2,}$";

    @Override
    protected void onCreate(Bundle savedInstanceState) {
        super.onCreate(savedInstanceState);
        setContentView(R.layout.activity_login);

        auth = FirebaseAuth.getInstance();
        btnlog = findViewById(R.id.btnlog);
        edlogemail = findViewById(R.id.edlogemail);
        edlogpass = findViewById(R.id.edlogpass);
        tx_singup = findViewById(R.id.tx_singup);



       tx_singup.setOnClickListener(new View.OnClickListener() {
           @Override
           public void onClick(View v) {
               Intent intent = new Intent(login.this,registration.class);
               startActivity(intent) ;
               finish();

           }
       });



        btnlog.setOnClickListener(new View.OnClickListener() {
            @Override
            public void onClick(View v) {
                String Email = edlogemail.getText().toString();
                String pass = edlogpass.getText().toString();

                if((TextUtils.isEmpty(Email))){
                    Toast.makeText(login.this, "Enter Email", Toast.LENGTH_SHORT).show();
                }else if((TextUtils.isEmpty(pass))){
                    Toast.makeText(login.this, "Enter Password", Toast.LENGTH_SHORT).show();
                } else if (!Email.matches(emailPattern)) {
                    edlogemail.setError("Enter Vaild Email");
                } else if (pass.length()<6) {
                    edlogpass.setError("More Than 6 Charecter");
                    
                }else{
                    auth.signInWithEmailAndPassword(Email,pass).addOnCompleteListener(new OnCompleteListener<AuthResult>() {
                        @Override
                        public void onComplete(@NonNull Task<AuthResult> task) {
                            if(task.isSuccessful()){

                                try {

                                    Intent intent = new Intent(login.this,MainActivity.class);
                                    startActivity(intent);
                                    finish();

                                }catch (Exception e){
                                    Toast.makeText(login.this,e.getMessage(),Toast.LENGTH_LONG).show();
                                }
                            }else{
                                Toast.makeText(login.this, task.getException().getMessage(), Toast.LENGTH_SHORT).show();
                            }
                        }
                    });
                }





            }
        });


    }
}
   ```
## Registration In With java = STEP : 2

Make Method In Java

   ```bash
package com.example.test;

import androidx.annotation.NonNull;
import androidx.annotation.Nullable;
import androidx.appcompat.app.AppCompatActivity;

import android.content.Intent;
import android.net.Uri;
import android.os.Bundle;
import android.text.TextUtils;
import android.util.Log;
import android.view.View;
import android.widget.Button;
import android.widget.EditText;
import android.widget.TextView;
import android.widget.Toast;

import com.google.android.gms.tasks.OnCompleteListener;
import com.google.android.gms.tasks.OnSuccessListener;
import com.google.android.gms.tasks.Task;
import com.google.firebase.auth.AuthResult;
import com.google.firebase.auth.FirebaseAuth;
import com.google.firebase.database.DatabaseReference;
import com.google.firebase.database.FirebaseDatabase;
import com.google.firebase.storage.FirebaseStorage;
import com.google.firebase.storage.StorageReference;
import com.google.firebase.storage.UploadTask;

import de.hdodenhof.circleimageview.CircleImageView;

public class registration extends AppCompatActivity {


    EditText edrgusername,edrgemail,edrgpass,edrgrepass;
    Button btnreg;
    TextView rglogin;
    CircleImageView imageprofile;
    FirebaseAuth auth;
    Uri imageURI;
    String imageuri;

    String emailPattern = "^[\\w.-]+@[\\w.-]+\\.[a-zA-Z]{2,}$";

    FirebaseDatabase database;
    FirebaseStorage store;


    @Override
    protected void onCreate(Bundle savedInstanceState) {
        super.onCreate(savedInstanceState);
        setContentView(R.layout.activity_registration);

        database = FirebaseDatabase.getInstance();
        store = FirebaseStorage.getInstance();
        auth = FirebaseAuth.getInstance();

        edrgusername =findViewById(R.id.edrgusername);
        edrgemail =findViewById(R.id.edrgemail);
        edrgpass =findViewById(R.id.edrgpass);
        btnreg =findViewById(R.id.btnreg);
        edrgrepass =findViewById(R.id.edrgrepass);
        rglogin =findViewById(R.id.rglogin);
        imageprofile =findViewById(R.id.imageprofile);


        //Get Data from Users

        btnreg.setOnClickListener(new View.OnClickListener() {
            @Override
            public void onClick(View v) {
                String namee = edrgusername.getText().toString();
                String emaill = edrgemail.getText().toString();
                String Password = edrgpass.getText().toString();
                String cPassword = edrgrepass.getText().toString();
                String status = "Hey I'm Using This Application";

                if (TextUtils.isEmpty(namee) || TextUtils.isEmpty(emaill) ||
                        TextUtils.isEmpty(Password) || TextUtils.isEmpty(cPassword)){

                    Toast.makeText(registration.this, "Please Enter Valid Information", Toast.LENGTH_SHORT).show();
                }else  if (!emaill.matches(emailPattern)){

                    edrgemail.setError("Type A Valid Email Here");
                }else if (Password.length()<6){

                    edrgpass.setError("Password Must Be 6 Characters Or More");
                }else if (!Password.equals(cPassword)){

                    edrgrepass.setError("The Password Doesn't Match");
                }else {
                    auth.createUserWithEmailAndPassword(emaill,Password).addOnCompleteListener(new OnCompleteListener<AuthResult>() {
                        @Override
                        public void onComplete(@NonNull Task<AuthResult> task) {


                            if (task.isSuccessful()){
                                String id = task.getResult().getUser().getUid();
                                DatabaseReference reference = database.getReference().child("user").child(id);
                                StorageReference storageReference = store.getReference().child("Upload").child(id);

                                if (imageURI!=null){
                                    storageReference.putFile(imageURI).addOnCompleteListener(new OnCompleteListener<UploadTask.TaskSnapshot>() {
                                        @Override
                                        public void onComplete(@NonNull Task<UploadTask.TaskSnapshot> task) {
                                            if (task.isSuccessful()){
                                                storageReference.getDownloadUrl().addOnSuccessListener(new OnSuccessListener<Uri>() {
                                                    @Override
                                                    public void onSuccess(Uri uri) {
                                                        imageuri = uri.toString();
                                                        Users users = new Users(id,namee,emaill,Password,imageuri,status);
                                                        reference.setValue(users).addOnCompleteListener(new OnCompleteListener<Void>() {
                                                            @Override
                                                            public void onComplete(@NonNull Task<Void> task) {
                                                                if (task.isSuccessful()){

                                                                    Intent intent = new Intent(registration.this,MainActivity.class);
                                                                    startActivity(intent);
                                                                    finish();
                                                                }else {
                                                                    Toast.makeText(registration.this, "Error in creating the user", Toast.LENGTH_SHORT).show();
                                                                }
                                                            }
                                                        });
                                                    }
                                                });
                                            }
                                        }
                                    });
                                }else {
                                    String status = "Hey I'm Using This Application";
                                    imageuri = "https://firebasestorage.googleapis.com/v0/b/av-messenger-dc8f3.appspot.com/o/man.png?alt=media&token=880f431d-9344-45e7-afe4-c2cafe8a5257";
                                    Users users = new Users(id,namee,emaill,Password,imageuri,status);
                                    reference.setValue(users).addOnCompleteListener(new OnCompleteListener<Void>() {
                                        @Override
                                        public void onComplete(@NonNull Task<Void> task) {
                                            if (task.isSuccessful()){

                                                Intent intent = new Intent(registration.this,MainActivity.class);
                                                startActivity(intent);
                                                finish();
                                            }else {
                                                Toast.makeText(registration.this, "Error in creating the user", Toast.LENGTH_SHORT).show();
                                            }
                                        }
                                    });
                                }
                            }else {
                                Toast.makeText(registration.this, task.getException().getMessage(), Toast.LENGTH_SHORT).show();
                            }
                        }
                    });
                }

            }
        });



        ///reg kora thakle log in page jua
      rglogin.setOnClickListener(new View.OnClickListener() {
          @Override
          public void onClick(View v) {
              Intent intent = new Intent(registration.this,login.class);
              startActivity(intent);
              finish();
          }
      });

      ////Profile Pic Upload

        imageprofile.setOnClickListener(new View.OnClickListener() {
            @Override
            public void onClick(View v) {
                Intent intent = new Intent();
                intent.setType("image/*");
                intent.setAction(Intent.ACTION_GET_CONTENT);
                startActivityForResult(Intent.createChooser(intent,"Select Profile Picture"),10);
            }
        });




    }

    ///Image Method


    @Override
    protected void onActivityResult(int requestCode, int resultCode, @Nullable Intent data) {
        super.onActivityResult(requestCode, resultCode, data);
        if(requestCode==10){
            if(data!=null){
                imageURI = data.getData();
                imageprofile.setImageURI(imageURI);
            }
        }
    }
}

   ```

## Users Class In With java = STEP : 3

Make Java Class

   ```bash
package com.example.test;

public class Users {
    String profilepic,mail,userName,password,userId,lastMessage,status;

    public  Users(){}

    public Users(String userId, String userName, String mail, String password, String profilepic, String status) {
        this.userId = userId;
        this.userName = userName;
        this.mail = mail;
        this.password = password;
        this.profilepic = profilepic;
        this.status = status;
    }

    public String getProfilepic() {
        return profilepic;
    }

    public void setProfilepic(String profilepic) {
        this.profilepic = profilepic;
    }

    public String getMail() {
        return mail;
    }

    public void setMail(String mail) {
        this.mail = mail;
    }

    public String getUserName() {
        return userName;
    }

    public void setUserName(String userName) {
        this.userName = userName;
    }

    public String getPassword() {
        return password;
    }

    public void setPassword(String password) {
        this.password = password;
    }

    public String getUserId() {
        return userId;
    }

    public void setUserId(String userId) {
        this.userId = userId;
    }

    public String getLastMessage() {
        return lastMessage;
    }

    public void setLastMessage(String lastMessage) {
        this.lastMessage = lastMessage;
    }

    public String getStatus() {
        return status;
    }

    public void setStatus(String status) {
        this.status = status;
    }
}


   ```



   
## 🚀 About Me
I'm a full stack developer..

