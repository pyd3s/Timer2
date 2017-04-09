#HTML5打包为Android APK
```Shell
 aptitude install npm 
 npm install -g cordova
 /usr/bin/nodejs /usr/bin/nodeln -s /usr/bin/nodejs /usr/bin/node
 cd /home/Pydes/Desktop
 cordova create Timer com.pydes.pydes
 cd Timer
 cordova platform add android@^5.0.0
 cordova platforms ls
 
 su root
 cd /home/Pydes/Desktop/Html5/Test 
 cp index.html /home/Pydes/Desktop/Timer/www/index.html
 cp js/* /home/Pydes/Desktop/Timer/www/js/ 
 cp -r sound /home/Pydes/Desktop/Timer/www/
 cp css/jquery.mobile-1.4.5.min.css /home/Pydes/Desktop/Timer/www/css/
 cd /home/Pydes/Desktop/Timer 
 vim ~/.bashrc 
 #add 
     export ANDROID_HOME=/home/Pydes/.buildozer/android/platform/android-sdk-20/
     PATH=.:$PATH:/home/Pydes/.buildozer/android/platform/android-sdk-20/tools
     export PATH
 #source ~/.bashrc
 android update sdk --no-ui --all --filter build-tools-25.0.1,android-25,extra-android-m2repository
 cordova-plugin-exitapp
 cordova build android
 /home/Pydes/Desktop/Timer/platforms/android/build/outputs/apk/android-debug.apk
 ```
