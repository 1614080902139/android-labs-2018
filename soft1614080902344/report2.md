﻿++#第二次实验
 + +
 + +## 1.实验目标
 + +
 + +（1）在Issues中创建自己的选题：https://github.com/hzuapps/android-labs-2018/issues ；
 + +（2）根据自选题目，编写一个或多个Activity（所有均带上学号前缀，放到自己的Java包下）；
 + +（3）将标题设置为自己的学号+对应的功能或题目；
 + +（4）根据自己选择的题目实现Activity中导航、调用等功能（选做）
 + +
 + +## 2.实验步骤
 + +（1）阅读实验要求：https://github.com/hzuapps/android-labs-2018/labels/Lab
 + +（2）在电脑上Android Studio编写代码// 代码要可以运行！
 + +（3）使用Git将代码提交到自己的库中：https://github.com/wangguifeng/android-labs-2018
 + +   $ git pull
 + +   $ git add 学号目录/* 
 + +   $ git commit "#12345678 "
 + +   $ git push
 + +（4）在自己的GitHub库上创建和发送Pull Request（注意查看Changed files）
 + +       // 是否只修改了自己的文件？
 + +（5）在GitHub中使用Markdown文件编写实验报告（report1.md, report2.md）
 + +      // 保存在自己的文件夹下
 + +
 + +## 3.实验结果
 + 
 + 1.AndroidManifest.xml
 + 
 + <?xml version="1.0" encoding="utf-8"?>
 +<manifest xmlns:android="http://schemas.android.com/apk/res/android"
 +    package="com.example.administrator.soft1614080902344">
 +
 +    <application
 +        android:allowBackup="true"
 +        android:icon="@mipmap/ic_launcher"
 +        android:label="@string/app_name"
 +        android:roundIcon="@mipmap/ic_launcher_round"
 +        android:supportsRtl="true"
 +        android:theme="@style/AppTheme">
 +        <activity android:name=".soft16140809023244Activity">
 +            <intent-filter>
 +                <action android:name="android.intent.action.MAIN" />
 +
 +                <category android:name="android.intent.category.LAUNCHER" />
 +            </intent-filter>
 +        </activity>
 +    </application>
 +
 +</manifest>
 + 
 + 2.Soft1614080902344Activity.java
 + 
 + package com.example.administrator.soft1614080902344;
 +
 +import android.support.v7.app.AppCompatActivity;
 +import android.os.Bundle;
 +
 +public class Soft1614080902344Activity extends AppCompatActivity {
 +
 +    @Override
 +    protected void onCreate(Bundle savedInstanceState) {
 +        super.onCreate(savedInstanceState);
 +        setContentView(R.layout.activity_soft1614080902344);
 +    }
 +}
 +
 +3.activity_soft1614080902344.xml
 +
 +<?xml version="1.0" encoding="utf-8"?>
 +<android.support.constraint.ConstraintLayout xmlns:android="http://schemas.android.com/apk/res/android"
 +    xmlns:app="http://schemas.android.com/apk/res-auto"
 +    xmlns:tools="http://schemas.android.com/tools"
 +    android:layout_width="match_parent"
 +    android:layout_height="match_parent"
 +    tools:context=".soft1614080902344Activity">
 +
 +    <TextView
 +        android:layout_width="wrap_content"
 +        android:layout_height="wrap_content"
 +        android:text="Hello World!"
 +        app:layout_constraintBottom_toBottomOf="parent"
 +        app:layout_constraintLeft_toLeftOf="parent"
 +        app:layout_constraintRight_toRightOf="parent"
 +        app:layout_constraintTop_toTopOf="parent" />
 +
 +</android.support.constraint.ConstraintLayout>
 +
 +4.strings.xml
 +
 +<resources>
 +    <string name="app_name">Soft1614080902344学生成绩管理系统</string>
 +</resources>
 +
 ++## 4.实验体会
 +本次实验比上两次均复杂一些，因为有太多文件要上传，虽然过程有点曲折，但还是完成了，本次实验学到了不少东西。
