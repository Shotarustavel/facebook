# facebook
java

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




    <LinearLayout
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

    <!-- შემოვიტანეთ სიცარიელესთვის <ImageView -->

    <ImageView

        android:background="#4140"
        android:layout_width="match_parent"
        android:layout_height="20dp" />
    <LinearLayout
        android:orientation="vertical"
        android:layout_width="match_parent"
        android:layout_height="wrap_content">

        <LinearLayout
            android:layout_width="match_parent"
            android:layout_height="wrap_content">


            <ImageView
                android:src="@drawable/alex"
                android:layout_width="50dp"
                android:layout_height="50dp"/>
