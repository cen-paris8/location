# Par rapport à la version initiale Margouillat master dans Firebase
# J'ai ajouté comme demandé ddans la doc du package location:

https://pub.dev/packages/location

AndroidManifest.xml
<uses-permission android:name="android.permission.ACCESS_FINE_LOCATION" />

gradle-wrapper.properties et local.properties comme il n'y a pas de gradle properties :
android.enableJetifier=true
android.useAndroidX=true
org.gradle.jvmargs=-Xmx1536M

build.gradle
classpath 'com.android.tools.build:gradle:3.3.0'
classpath 'com.google.gms:google-services:4.2.0'



et pour finir dans pubspec.yaml
location: ^2.3.5