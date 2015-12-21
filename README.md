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
