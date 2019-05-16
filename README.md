# Par rapport à la version initiale Margouillat master dans Firebase
# J'ai ajouté comme demandé dans la doc du package location:

https://pub.dev/packages/location

AndroidManifest.xml
<uses-permission android:name="android.permission.ACCESS_FINE_LOCATION" />

gradle.properties :
android.enableJetifier=true
android.useAndroidX=true
org.gradle.jvmargs=-Xmx1536M

build.gradle
classpath 'com.android.tools.build:gradle:3.3.0'
classpath 'com.google.gms:google-services:4.2.0'

Modifier car log du flutter run a demandé de monter de version.
distributionUrl=https\://services.gradle.org/distributions/gradle-4.10.1-all.zip

et pour finir dans pubspec.yaml
location: ^2.3.5

Log du run :
 flutter run
Launching lib/main.dart on F5321 in debug mode...
Initializing gradle...                                              6,6s
Resolving dependencies...                                          78,0s
Running Gradle task 'assembleDebug'...                            230,6s (!)
Built build\app\outputs\apk\debug\app-debug.apk.
Installing build\app\outputs\apk\app.apk...                         6,9s
Syncing files to device F5321...                                 6 873ms (!)

