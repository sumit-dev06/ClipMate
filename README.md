# ✂️ Clipmate 

A lightweight, completely free clipboard manager built exclusively for macOS. Clipmate lives in your menu bar and lets you access your clipboard history instantly from anywhere using a global shortcut.

## ✨ Features
*   **Instant Access:** Bring up your clipboard history anywhere on your Mac with a single shortcut.
*   **100% Free:** No paywalls or subscriptions, unlike many alternatives on the App Store.
*   **Customizable Shortcut:** Total control over the hotkey you use to trigger the app.
*   **Favorites:** Mark important clips as favorites so you never lose them.
*   **Native Feel:** Sits quietly in your Mac's menu bar (Control Center).

## 🛠️ Built With
*   Electron

## 🚀 Build & Installation Guide

Since Clipmate is open-source, you will build the Mac `.dmg` file locally. Make sure you have Node.js and npm installed on your Mac before starting.

### 1. Download and Prepare
1. Download the `clipmate.zip` source code from the Releases page.
2. Extract the zip file into your `Downloads` folder.

### 2. Customize Your Shortcut (Optional)
Before building the app, you can change the global shortcut used to open Clipmate:
1. Open the extracted `clipmate` folder and open `main.js` in a text editor.
2. Find the variable `const shortcut`.
3. Change it to your preferred key combination (I recommend `Option+Space`). 
*Note: Make sure your new shortcut doesn't conflict with existing macOS system shortcuts!*

### 3. Build the App
Open your Terminal and run the following commands sequentially:

```bash
# Navigate to the extracted folder
cd ~/Downloads/clipmate

# Install required dependencies
npm install

# Build the macOS application
npm run build
```

### 4. Install
1. Once the build finishes, a new `dist/` folder will be generated inside the `clipmate` directory.
2. Open the `dist/` folder and double-click the newly created `.dmg` file.
3. Drag the **Clipmate** app into your Applications folder.

## 💻 How to Use
*   Launch Clipmate from your Applications folder. You will see its icon appear in your top menu bar.
*   Use your global shortcut to access your clipboard anywhere.
*   **Auto-Start:** To make Clipmate launch automatically when you turn on your Mac, go to **System Settings > General > Login Items** and add Clipmate to the list.
