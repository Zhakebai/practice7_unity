# practice7_unity
# Dragon Picker - Unity WebGL Game

## 🎮 Project Overview
Dragon Picker is a Unity-based game built for WebGL and hosted on **simmer.io**. This project is part of a learning exercise to structure Unity projects properly and deploy them on a web-based platform.

## 📂 Project Structure
The project follows a structured file organization for better maintainability:

- **Scripts:** Game logic and mechanics.
- **Textures & Materials:** Visual assets used in the game.
- **Audio:** Background music and sound effects.
- **Animations & Controllers:** Character animations.
- **Prefabs & Scenes:** Game objects and level design.

## 🚀 Deployment on Simmer.io
### Steps to Upload:
1. Build the project for **WebGL**:
   - Go to **File → Build Settings**.
   - Select **WebGL** as the platform.
   - Disable **Compression Format** in **Player Settings**.
   - Click **Build And Run**.

2. Upload the build folder to [simmer.io](https://simmer.io/upload):
   - Register/Login.
   - Drag and drop the `DragonPickerBuild` folder.
   - Set a name and URL.
   - Save and publish.

## 🔧 Troubleshooting
### ❌ Error: "Cannot read properties of undefined (reading 'buildUrlIsIncludeBuildDirectory')"
- Ensure the **WebGL module** is installed in **Unity Hub**.
- Make sure the **Compression Format** is set to **Disable**.
- Restart Unity after switching the platform to **WebGL**.

### ❌ Error Loading Script (`error loading script`)
- Check **Build Settings** and **Player Settings**.
- Make sure all **scenes** are included in the build.
- Ensure that **simmer.io** supports the Unity version used.

## 📜 License
This project is for educational purposes only.
