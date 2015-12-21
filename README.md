# Welcome-to-EV
An EV neighborhood app
<?xml version="1.0" encoding="utf-8"?>
<ScrollView xmlns:android="http://schemas.android.com/apk/res/android"
    xmlns:tools="http://schemas.android.com/tools"
    android:layout_width="match_parent"
    android:layout_height="match_parent"
    tools:context="MainActivity">

    <LinearLayout xmlns:android="http://schemas.android.com/apk/res/android"
        android:layout_width="match_parent"
        android:layout_height="match_parent"
        android:background="#8C1515"
        android:orientation="vertical"
        android:paddingLeft="8dp">

        <TextView
            android:layout_width="match_parent"
            android:layout_height="200dp"
            android:background="@drawable/escondido_photo"
            android:textAlignment="center"
            android:textSize="45sp" />

        <TextView
            android:layout_width="match_parent"
            android:layout_height="0dp"
            android:layout_weight="1"
            android:text="5 Things to Know"
            android:textAlignment="center"
            android:textAllCaps="true"
            android:textSize="40sp" />


        <TextView

            android:layout_width="wrap_content"
            android:layout_height="wrap_content"
            android:drawableLeft="@drawable/ic_group_black_18dp"
            android:onClick="visibilityConnect"
            android:singleLine="true"
            android:text="Connect"
            android:textSize="35sp" />


        <TextView
            android:id="@+id/nextdoor"
            android:layout_width="match_parent"
            android:layout_height="0dp"
            android:layout_weight="1"
            android:onClick="openWebPage"
            android:padding="8dp"
            android:text="Nextdoor.com"
            android:textSize="20sp" />

        <TextView
            android:id="@+id/parentnet"
            android:layout_width="match_parent"
            android:layout_height="0dp"
            android:layout_weight="1"
            android:onClick="openWebPageP"
            android:padding="8dp"
            android:text="Stanford Parent-net mailing list"
            android:textSize="20sp" />

        <TextView
            android:layout_width="match_parent"
            android:layout_height="0dp"
            android:layout_weight="1"
            android:onClick="openWebPageP"
            android:padding="8dp"
            android:text="Courtyard Mailing Lists- Ask your Community Associates"
            android:textSize="20sp" />

        <TextView
            android:layout_width="wrap_content"
            android:layout_height="wrap_content"
            android:drawableLeft="@drawable/ic_shopping_basket_black_18dp"
            android:singleLine="true"
            android:text="Shop"
            android:textSize="35sp" />

        <TextView
            android:layout_width="match_parent"
            android:layout_height="0dp"
            android:layout_weight="1"
            android:onClick="showMapGO"
            android:padding="8dp"
            android:text="For Bargains- Grocery Outlet"
            android:textSize="20sp" />

        <TextView
            android:layout_width="match_parent"
            android:layout_height="0dp"
            android:layout_weight="1"
            android:onClick="showMapTJ"
            android:padding="8dp"
            android:text="Nearby- Trader Joes"
            android:textSize="20sp" />

        <TextView
            android:layout_width="match_parent"
            android:layout_height="0dp"
            android:layout_weight="1"
            android:onClick="showMapMP"
            android:padding="8dp"
            android:text="Best Produce-Milk Pail Market"
            android:textSize="20sp" />

        <TextView
            android:layout_width="match_parent"
            android:layout_height="0dp"
            android:layout_weight="1"
            android:onClick="showMapMM"
            android:padding="8dp"
            android:text="Quick Milk Run- The Market at Munger"
            android:textSize="20sp" />

        <TextView
            android:layout_width="wrap_content"
            android:layout_height="wrap_content"
            android:drawableLeft="@drawable/ic_nature_people_black_18dp"
            android:singleLine="true"
            android:text="Play"
            android:textSize="35sp" />

        <TextView
            android:layout_width="match_parent"
            android:layout_height="0dp"
            android:layout_weight="1"
            android:padding="8dp"
            android:text="Peers Park Playground"
            android:textSize="20sp" />

        <TextView
            android:layout_width="match_parent"
            android:layout_height="0dp"
            android:layout_weight="1"
            android:onClick="openWebPageC"
            android:padding="8dp"
            android:text="College Terrace Library Story Time"
            android:textSize="20sp" />

        <TextView
            android:layout_width="wrap_content"
            android:layout_height="wrap_content"
            android:drawableLeft="@drawable/ic_local_dining_black_18dp"
            android:singleLine="true"
            android:text="Eat"
            android:textSize="35sp" />

        <TextView
            android:layout_width="match_parent"
            android:layout_height="0dp"
            android:layout_weight="1"
            android:onClick="openWebPageA"
            android:padding="8dp"
            android:text="Arrillaga Family Dining Commons (Kids Eat Free)"
            android:textSize="20sp" />

        <TextView
            android:layout_width="wrap_content"
            android:layout_height="wrap_content"
            android:drawableLeft="@drawable/ic_link_black_18dp"
            android:singleLine="true"
            android:text="Get Help"
            android:textSize="35sp" />

        <TextView
            android:layout_width="match_parent"
            android:layout_height="0dp"
            android:layout_weight="1"
            android:onClick="openWebPagePS"
            android:padding="8dp"
            android:text="Non-Emergency Public Safety"
            android:textSize="20sp" />

        <TextView
            android:layout_width="wrap_content"
            android:layout_height="wrap_content"
            android:drawableLeft="@drawable/ic_local_phone_black_18dp"
            android:singleLine="true"
            android:text="Contact Us"
            android:textSize="35sp" />

    </LinearLayout>

</ScrollView>
package com.example.android.welcometoev;

import android.content.Intent;
import android.net.Uri;
import android.os.Bundle;
import android.support.v7.app.AppCompatActivity;
import android.view.View;

public class MainActivity extends AppCompatActivity {

    @Override
    protected void onCreate(Bundle savedInstanceState) {
        super.onCreate(savedInstanceState);
        setContentView(R.layout.activity_main);
    }

    public void openWebPage(View view) {
        Uri webpage = Uri.parse("http://www.nextdoor.com");
        Intent intent = new Intent(Intent.ACTION_VIEW, webpage);
        if (intent.resolveActivity(getPackageManager()) != null) {
            startActivity(intent);
        }
    }
    public void openWebPagePS(View view) {
        Uri webpage = Uri.parse("http://web.stanford.edu/group/SUDPS/");
        Intent intent = new Intent(Intent.ACTION_VIEW, webpage);
        if (intent.resolveActivity(getPackageManager()) != null) {
            startActivity(intent);
        }

    }
    public void openWebPageC(View view) {
        Uri webpage = Uri.parse("http://www.cityofpaloalto.org/gov/depts/lib/kids/storytime.asp");
        Intent intent = new Intent(Intent.ACTION_VIEW, webpage);
        if (intent.resolveActivity(getPackageManager()) != null) {
            startActivity(intent);
        }
    }
    public void openWebPageA(View view) {
        Uri webpage = Uri.parse("https://rde.stanford.edu/dining/arrillaga-family-dining-commons");
        Intent intent = new Intent(Intent.ACTION_VIEW, webpage);
        if (intent.resolveActivity(getPackageManager()) != null) {
            startActivity(intent);
        }
    }
    public void openWebPageP(View view) {
        Uri webpage = Uri.parse("https://mailman.stanford.edu/mailman/listinfo/PARENT-NET");
        Intent intent = new Intent(Intent.ACTION_VIEW, webpage);
        if (intent.resolveActivity(getPackageManager()) != null) {
            startActivity(intent);
        }
    }
//    public void visibilityConnect(View view){
//        TextView nextdoor = (TextView)findViewById(R.id.nextdoor);
//        nextdoor.setVisibility(TextView.INVISIBLE);
//
//    }

    public void showMapMP(View view) {
//        Intent intent = new Intent(Intent.ACTION_VIEW);
//        intent.setData(Uri.parse("geo:47.6,-122.3"));
//        if (intent.resolveActivity(getPackageManager()) != null) {
//            startActivity(intent);
//
//        }
        Intent intent = new Intent(android.content.Intent.ACTION_VIEW,
                Uri.parse("https://www.google.com/maps/place/The+Milk+Pail+Market/@37.4052369,-122.1101418,15z/data=!4m2!3m1!1s0x0:0xdf2977762c01504a"));
        startActivity(intent);
    }
    public void showMapTJ(View view) {
    Intent intent = new Intent(android.content.Intent.ACTION_VIEW,
            Uri.parse("https://www.google.com/maps/place/Trader+Joe's/@37.4384642,-122.1598149,17z/data=!3m2!4b1!5s0x808fbb2380644d83:0xff95595ed2eadb00!4m2!3m1!1s0x808fbb2516173e1f:0x51708040db758a08"));
        startActivity(intent);
    }
    public void showMapGO(View view) {
        Intent intent = new Intent(android.content.Intent.ACTION_VIEW,
                Uri.parse("https://www.google.com/maps/place/Grocery+Outlet/@37.4384434,-122.2278435,12z/data=!4m5!1m2!2m1!1sgrocery+outlet!3m1!1s0x808fba613c12e2f5:0xc82b42ded926ef59"));
        startActivity(intent);

    }
    public void showMapMM(View view) {
        Intent intent = new Intent(android.content.Intent.ACTION_VIEW,
                Uri.parse("https://www.google.com/maps/place/The+Market+at+Munger/@37.4228689,-122.1699903,17z/data=!4m5!1m2!2m1!1sMarket+at+Munger!3m1!1s0x808fbad138652a45:0x4a91d529555b1d3e"));
        startActivity(intent);
    }
}
