# ProDev Mobile App 0x00 — Expo Router Setup

## 📘 Objective
Set up your first mobile application using the **Expo Router** template.  
Document the scaffolding process, understand the file structure of a React Native application built with Expo, and observe the behavior of the reset command.

---

## 🧭 Step 1: Navigate to Project Directory

Open your terminal and move into your parent directory:

```bash
cd prodev-mobile-setup

🚀 Step 2: Set Up the Project Using Expo Router Template

Initialize a new Expo project using the latest Expo Router template:

npx create-expo-app@latest app-example


When prompted, choose:

✔ Choose a template: › Navigation (Expo Router)


This will automatically create a new Expo app inside the folder app-example.

🗂️ Step 3: Folder Structure After Scaffolding

After the project is created, your folder should look like this:

app-example/
├── app/
│   ├── (tabs)/
│   │   ├── index.tsx
│   │   └── explore.tsx
│   ├── _layout.tsx
│   └── +not-found.tsx
│
├── assets/
├── constants/
│   └── Colors.tsx
├── package.json
└── README.md


This is the typical structure of an Expo Router project:

app/ — contains screens and layouts.

constants/ — reusable configuration values (like colors).

assets/ — images, fonts, and static files.

package.json — manages dependencies and scripts.

📝 Step 4: Modify the Home Screen

Open the following file:

app-example/app/(tabs)/index.tsx


Find this line:

<Text style={styles.title}>Welcome!</Text>


Replace it with:

<Text style={styles.title}>First App Created</Text>


Save your changes.

▶️ Step 5: Run and Test the Application

Start the Expo development server:

npx expo start


You’ll see a QR code appear in your terminal.

For iOS: Open your Camera app and scan the QR code.

For Android: Use the Expo Go app to scan the QR code.

Once the app opens, it should display:

First App Created


🎉 Congratulations! You’ve successfully built and modified your first Expo Router app.

🔁 Step 6: Reset the Application

Run the reset command to clear the cache and restart the bundler:

npm run reset-project


This command is usually defined in your package.json as:

"reset-project": "expo start --clear"

🧠 Observations

Clears the Metro bundler cache.

Rebuilds project assets.

Helps fix common issues caused by stale caches.

Terminal output shows:

Starting Metro Bundler...
Clearing cache...


Your project source files remain intact.

🧩 Step 7: Verify Project Files

Ensure the following files exist and contain valid code:

✅ app-example/app/(tabs)/index.tsx
→ Includes the updated text "First App Created".

✅ app-example/constants/Colors.tsx
→ Defines color constants used across the app.

✅ README.md
→ Documents the setup and reset process.

🧾 Step 8: Summary of Key Commands
Purpose	Command
Create new Expo app	npx create-expo-app@latest app-example
Navigate into app folder	cd app-example
Start the Expo server	npx expo start
Reset the project	npm run reset-project
🧱 Step 9: Repository Details

Repository: prodev-mobile-setup

Project Directory: prodev-mobile-app-0x00

Main App Folder: app-example

Key Files:

README.md

app-example/app/(tabs)/index.tsx

app-example/constants/Colors.tsx

🔧 Troubleshooting

If your checker or terminal shows:

app-example/app/(tabs)/index.tsx doesn't exist

It means your Expo project was created in the wrong folder.
Fix it by ensuring your structure looks like:

app-example/app/(tabs)/index.tsx


If you created the app in the root, move it manually:

mkdir -p app-example
mv app app-example/
mv assets app-example/
mv constants app-example/


Then re-run your checker.

✅ Final Outcome

After completing all steps:

The Expo app builds successfully.

The home screen text shows “First App Created”.

The npm run reset-project command clears caches and reloads the app.

Folder structure matches the expected Expo Router layout.

Author: [Your Name]
Date: [Submission Date]
Project: ProDev Mobile App 0x00