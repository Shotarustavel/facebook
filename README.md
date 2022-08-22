<?xml version="1.0" encoding="utf-8"?>
<LinearLayout xmlns:android="http://schemas.android.com/apk/res/android"
    xmlns:tools="http://schemas.android.com/tools"
    android:id="@+id/activiy_main"
    android:layout_width="match_parent"
    android:layout_height="match_parent"
    android:paddingBottom="16dp"
    android:paddingLeft="16dp"
    android:paddingRight="16dp"
    android:paddingTop="16dp"
    android:orientation="vertical"
    tools:context="com.bsu.facebook1.MainActivity">


    <!-- მშობელი კონტეინერი <LinearLayout -->
    <!-- A რადგან 3 შვილი გვყავს  weightSum="3"-->
    <!-- ორიენტაცია ვინც ჩაჯდება იყოს ჰორიზონტალური orientation="horizontal"   -->
    <!-- სიგანე მთლიანად გაიწელოს layout_width="wrap_content"  -->
    <!-- სიგრძე რამხელასაც დაიკავებს layout_height="match_parent"  -->


      <!-- შვილი კონტეინერი <LinearLayout  -->
      <!-- დაშორება მარჯვნიდან layout_marginLeft="20dp"   -->
      <!-- ცენტრში განთავსება gravity="center"   -->
      <!-- A თუ გვინდა რომ ყველამ შვილმა თანაბარი ზომები დაიჭიროს layout_width="0dp" -->
      <!-- A  თუ ვინდა რომ ყველამ შვილმა თანაბარი ზომები დაიჭიროს  layout_weight="1" -->

         <!--  ფოტოს შემოტანა ImageView   -->

               <!-- ტექსტის შემოტანა<TextView  -->
               <!--   -->






    <!-- სიცარიელის ველი  <ImageView -->

    <ImageView

        android:background="#4140"
        android:layout_width="match_parent"
        android:layout_height="20dp" />

    <!--ფოტო , ალექსი ამნიაშვილი   ველი    -->

    <LinearLayout
        android:orientation="vertical"
        android:layout_width="match_parent"
        android:layout_height="wrap_content">

        <LinearLayout
            android:layout_marginTop="10dp"
            android:layout_marginLeft="15dp"
            android:layout_width="match_parent"
            android:layout_height="wrap_content">


            <ImageView
                android:src="@drawable/alex"
                android:layout_width="50dp"
                android:layout_height="50dp"/>


      <RelativeLayout
             android:layout_marginLeft="5dp"
             android:gravity="center_vertical"
             android:layout_gravity="center_vertical"
             android:layout_width="wrap_content"
             android:layout_height="wrap_content">


             <TextView
                 android:id="@+id/user_name_text_view_id"
                 android:textSize="11sp"
                 android:textStyle="bold"
                 android:text="ალექსი ამნიაშვილი"
                 android:layout_width="wrap_content"
                 android:layout_height="wrap_content" />
            <TextView
                android:id="@+id/posted_text_view_id"
                android:layout_toRightOf="@+id/user_name_text_view_id"
                android:layout_marginLeft="5dp"
                android:textSize="10sp"
                android:text="posted a photo on"
                android:layout_height="wrap_content"
                android:layout_width="wrap_content"/>

            <TextView
                android:textSize="11sp"
                android:textStyle="bold"
                android:layout_toRightOf="@+id/posted_text_view_id"
                android:text="instagram"
                android:layout_height="wrap_content"
                android:layout_width="wrap_content"/>

                <LinearLayout
                    android:layout_marginTop="5dp"
                    android:layout_below="@+id/user_name_text_view_id"
                    android:orientation="horizontal"
                    android:layout_width="match_parent"
                    android:layout_height="wrap_content">
                    <TextView
                        android:textSize="10sp"
                        android:text="sep 10:20: px"
                        android:layout_width="wrap_content"
                        android:layout_height="wrap_content" />
                    <TextView
                        android:layout_marginLeft="20dp"
                        android:text="instagram"
                        android:textSize="10sp"
                        android:layout_width="wrap_content"
                        android:layout_height="wrap_content"/>
                    <ImageView
                        android:layout_marginLeft="5dp"
                        android:src="@android:drawable/btn_radio"
                        android:layout_width="10dp"
                        android:layout_height="10dp" />





                    </LinearLayout>


                 </RelativeLayout>



              </LinearLayout>

        <TextView
            android:layout_marginLeft="15dp"
            android:layout_marginTop="15dp"
            android:text="Again alex /@ alexa #BASIANI"
            android:layout_width="wrap_content"
            android:layout_height="wrap_content"/>


        </LinearLayout>

    <!--  მამალის ფოტო -->
    <ImageView
        android:layout_marginTop="20dp"
        android:src="@drawable/mamali"
        android:scaleType="centerCrop"
        android:layout_width="match_parent"
        android:layout_height="350dp" />

    <!--tato tato gios da coomments ველი-->

    <LinearLayout
        android:layout_marginTop="20dp"
        android:orientation="horizontal"
        android:gravity="center_vertical"
        android:layout_width="match_parent"
        android:layout_height="wrap_content">
       <ImageView

           android:layout_marginLeft="10dp"
           android:src="@android:drawable/arrow_down_float"
           android:layout_width="wrap_content"
           android:layout_height="wrap_content"/>

        <ImageView
            android:layout_marginLeft="10dp"
            android:src="@android:drawable/arrow_down_float"
            android:layout_width="wrap_content"
            android:layout_height="wrap_content"/>
        <TextView
            android:layout_marginLeft="10dp"
            android:text="tato tato gio"
            android:layout_width="wrap_content"
            android:layout_height="wrap_content"/>
        <TextView
            android:layout_marginEnd="20dp"
            android:gravity="end"
            android:text="3 comments"
            android:layout_width="match_parent"
            android:layout_height="wrap_content"/>
    </LinearLayout>
    <!-- like comment share ველი  -->

    <LinearLayout
        android:layout_marginTop="20dp"
        android:weightSum="3"
        android:gravity="center_vertical"
        android:orientation="horizontal"
        android:layout_width="match_parent"
        android:layout_height="30dp">



        <LinearLayout
            android:layout_marginLeft="20dp"
            android:orientation="horizontal"
            android:layout_width="0dp"
            android:layout_weight="1"
            android:gravity="center_vertical"
            android:layout_height="wrap_content">

            <ImageView
                android:layout_width="20dp"
                android:layout_height="20dp"
                android:src="@drawable/like" />

            <TextView
                android:layout_marginLeft="5dp"
                android:layout_width="wrap_content"
                android:layout_height="wrap_content"
                android:text="like" />


        </LinearLayout>

        <LinearLayout
            android:gravity="center"
            android:orientation="horizontal"
            android:layout_width="0dp"
            android:layout_weight="1"
            android:layout_height="wrap_content">

            <ImageView
                android:src="@drawable/comment"
                android:layout_width="20dp"
                android:layout_height="20dp"/>
            <TextView
                android:layout_marginLeft="5dp"
                android:text="comment"
                android:layout_width="wrap_content"
                android:layout_height="wrap_content"/>


        </LinearLayout>

        <LinearLayout
            android:gravity="center"
            android:orientation="horizontal"
            android:layout_width="0dp"
            android:layout_weight="1"
            android:layout_height="wrap_content">
            <ImageView
                android:src="@drawable/share"
                android:layout_width="20dp"
                android:layout_height="20dp"/>
            <TextView
                android:layout_marginLeft="5dp"
                android:text="share"
                android:layout_width="wrap_content"
                android:layout_height="wrap_content"/>


        </LinearLayout>


    </LinearLayout>

</LinearLayout>
