# Login-Register-firebase
Login-Register-firebase
// Enabling Firebase Auth
1. First thing you need to do is go to https://firebase.google.com/ and make an account to gain access to their console. After you gain access to the console you can start by creating your first project.

2. Give the package name of your project (mine is info.androidhive.firebase) in which you are going to integrate the Firebase. Here the google-services.json file will be downloaded when you press add app button.

3. Next go to your project dashboard. Find the Auth and click get started. Go to set up sign in method and choose Email & Password and enable it.


//add permissions to your manifest file

<uses-permission android:name="android.permission.INTERNET" />


//google-services.json
Paste the google-services.json file to your project’s app folder.

//build.gradle(project)
dependencies {
        classpath 'com.android.tools.build:gradle:3.1.4'
        classpath 'com.google.gms:google-services:4.1.0'
        

        // NOTE: Do not place your application dependencies here; they belong
        // in the individual module build.gradle files
    }



//build.gradle(app)

dependencies {
    compile "com.google.firebase:firebase-auth:9.0.2"
}
 
apply plugin: 'com.google.gms.google-services'



you can set resources on your own...like,dimens,strings,colors,drawables etc...

And you are all set!!!
