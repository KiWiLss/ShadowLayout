# ShadowLayout
阴影布局控件
- 1,效果
![](https://github.com/KiWiLss/ShadowLayout/blob/master/app/src/main/res/drawable/shadow.jpg)

- 2,直接在xml中使用
```
<?xml version="1.0" encoding="utf-8"?>
<LinearLayout
    xmlns:android="http://schemas.android.com/apk/res/android"
    xmlns:app="http://schemas.android.com/apk/res-auto"
    xmlns:tools="http://schemas.android.com/tools"
    android:layout_width="match_parent"
    android:layout_height="match_parent"
    tools:context="com.magicsoft.shadowlayout.MainActivity"
    android:orientation="vertical">

    <TextView
        android:layout_width="wrap_content"
        android:layout_height="wrap_content"
        android:text="Hello World!"
        app:layout_constraintBottom_toBottomOf="parent"
        app:layout_constraintLeft_toLeftOf="parent"
        app:layout_constraintRight_toRightOf="parent"
        app:layout_constraintTop_toTopOf="parent" />

        <com.magicsoft.mylibrary.ShadowLayout
            android:layout_width="wrap_content"
            android:layout_height="wrap_content"
            android:padding="15dp"
            app:sl_shadow_color="@color/colorAccent"
            app:sl_shadow_angle="45"
            app:sl_shadow_distance="5dp"
            app:sl_shadow_radius="5dp"
            >


            <ImageView
                android:layout_width="wrap_content"
                android:layout_height="wrap_content"
                android:src="@mipmap/hl_heart0"/>


        </com.magicsoft.mylibrary.ShadowLayout>



    <com.magicsoft.mylibrary.ShadowLayout
        android:layout_width="wrap_content"
        android:layout_height="wrap_content"
        android:padding="15dp"
        app:sl_shadow_angle="90"
        app:sl_shadow_color="#97E9EF"
        app:sl_shadow_distance="3dp"
        app:sl_shadow_radius="3dp"
        app:sl_shadowed="true">

        <ImageView
            android:layout_width="35dp"
            android:layout_height="35dp"
            android:src="@mipmap/hl_heart1" />
    </com.magicsoft.mylibrary.ShadowLayout>

    <com.magicsoft.mylibrary.ShadowLayout
        android:layout_width="wrap_content"
        android:layout_height="wrap_content"
        android:padding="15dp"
        app:sl_shadow_angle="210"
        app:sl_shadow_color="#FDB59D"
        app:sl_shadow_distance="5dp"
        app:sl_shadow_radius="5dp"
        app:sl_shadowed="true">

        <ImageView
            android:layout_width="65dp"
            android:layout_height="65dp"
            android:src="@mipmap/hl_heart2" />
    </com.magicsoft.mylibrary.ShadowLayout>

    <com.magicsoft.mylibrary.ShadowLayout
        android:layout_width="wrap_content"
        android:layout_height="wrap_content"
        android:padding="15dp"
        app:sl_shadow_angle="0"
        app:sl_shadow_color="@color/colorAccent"
        app:sl_shadow_distance="6dp"
        app:sl_shadow_radius="10dp"
        app:sl_shadowed="true">

        <ImageView
            android:layout_width="95dp"
            android:layout_height="95dp"
            android:src="@mipmap/hl_heart1" />
    </com.magicsoft.mylibrary.ShadowLayout>

    <LinearLayout
        android:layout_width="match_parent"
        android:layout_height="wrap_content"
        android:orientation="horizontal">

        <com.magicsoft.mylibrary.ShadowLayout
            android:layout_width="wrap_content"
            android:layout_height="wrap_content"
            android:padding="15dp"
            app:sl_shadow_angle="90"
            app:sl_shadow_color="#873930"
            app:sl_shadow_distance="5dp"
            app:sl_shadow_radius="3dp"
            app:sl_shadowed="true">

            <TextView
                android:layout_width="wrap_content"
                android:layout_height="wrap_content"
                android:text="Apple"
                android:textColor="#873930"
                android:textSize="16dp" />
        </com.magicsoft.mylibrary.ShadowLayout>

        <com.magicsoft.mylibrary.ShadowLayout
            android:layout_width="wrap_content"
            android:layout_height="wrap_content"
            android:padding="15dp"
            app:sl_shadow_angle="270"
            app:sl_shadow_color="#3e3e3e"
            app:sl_shadow_distance="3dp"
            app:sl_shadow_radius="3dp"
            app:sl_shadowed="true">

            <TextView
                android:layout_width="wrap_content"
                android:layout_height="wrap_content"
                android:text="Orange"
                android:textColor="#3e3e3e"
                android:textSize="19dp" />
        </com.magicsoft.mylibrary.ShadowLayout>

        <com.magicsoft.mylibrary.ShadowLayout
            android:layout_width="wrap_content"
            android:layout_height="wrap_content"
            android:padding="15dp"
            app:sl_shadow_angle="45"
            app:sl_shadow_color="#71e430"
            app:sl_shadow_distance="5dp"
            app:sl_shadow_radius="5dp"
            app:sl_shadowed="true">

            <TextView
                android:layout_width="wrap_content"
                android:layout_height="wrap_content"
                android:text="Banana"
                android:textColor="#71e430"
                android:textSize="22dp" />
        </com.magicsoft.mylibrary.ShadowLayout>

    </LinearLayout>
</LinearLayout>

```
- 3,引入
```
project的build.gradle
allprojects {
    repositories {

        maven { url 'https://www.jitpack.io' }
    }
}

model的build.gradle
compile 'com.github.KiWiLss:ShadowLayout:0.0.1'
```