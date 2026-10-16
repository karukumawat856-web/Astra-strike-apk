ASTRA STRIKE — APK BUILDER (FIXED WORKFLOW)

IMPORTANT: Purane GitHub workflow mein gradlew wrapper check tha, isliye build fail ho sakta tha. Is package ka workflow Gradle 8.7 ko khud setup karta hai; gradlew file ki zaroorat nahi.

PHONE SE SETUP:
1) Is ZIP ko download karke File Manager se EXTRACT karein.
2) Extracted folder AstraStrike_GitHub_APK ke andar jo files/folders hain, unhe repository ke ROOT mein upload karein. Root ka matlab repository kholte hi jahan Code tab mein files dikhti hain.
3) Folder structure ko bilkul aisa rakhein:
   .github/workflows/build-apk.yml
   app/build.gradle
   app/src/main/AndroidManifest.xml
   app/src/main/assets/index.html
   app/src/main/java/com/piyush/astrastrike/MainActivity.java
   build.gradle
   settings.gradle
   gradle.properties
4) GitHub par sab files upload karne ke baad Commit changes karein.
5) Actions tab > Build Astra Strike APK > Run workflow > Run workflow.
6) Run green ho jaaye to us run ko kholein, neeche Artifacts mein Astra-Strike-APK download karein.
7) Artifact ZIP ko extract karein aur app-debug.apk install karein. Agar Android warning aaye, to sirf apne banaye hue APK ko install karne ki permission dein.

AGAR PHONE PAR FOLDER STRUCTURE PRESERVE NA HO:
GitHub mobile upload mein files galat jagah root par aa jaati hain to build nahi hoga. Har file ko root mein alag-alag upload na karein; paths upar jaise hi hone chahiye. .github/workflows/build-apk.yml sabse zaroori hai.

GAME STATUS:
- Game landscape/horizontal orientation ke liye Android app wrapper mein set hai.
- Friends/UID section abhi local device par kaam karta hai; true online multiplayer, friend search across phones, rooms aur real-time play ke liye Firebase/server configuration baad mein add karna hoga.
- APK is ZIP ke andar prebuilt nahi hai. GitHub Actions success hone par APK artifact banega.
