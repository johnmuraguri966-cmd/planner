# Planner: build your APK (no Android Studio needed)

1. Create a free account at github.com and make a new repository (any name, can be private).
2. Upload everything in this folder to it, keeping the structure
   (www/, .github/workflows/, package.json, capacitor.config.json, .gitignore).
   Tip: on the repository page choose Add file > Upload files, and drag the contents in.
   The hidden .github folder must be included.
3. Open the Actions tab. The "Build APK" workflow starts by itself (or click Run workflow). It takes about 5 minutes.
4. When it shows a green tick, open the run and download "planner-apk" under Artifacts. Unzip it to get app-debug.apk.
5. Copy the APK to your phone and open it. Allow "Install unknown apps" when asked.
6. Open Planner, tap the bell icon, and allow notifications. If asked, also allow "Alarms & reminders" so reminders arrive on time.

Your activities are stored on the phone. Reminders are scheduled with Android, so they fire even when the app is closed.
To change the app, edit www/index.html and commit: a new APK is built each time.
