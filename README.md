# AR & VR Demo for Meta Quest 2 using Unity and MQDH

This repository showcases an **Augmented Reality (AR)** demo built in **Unity** for the **Meta Quest 2**, using the **Meta Quest Developer Hub (MQDH)** for deployment and real-time debugging. By blending VR pass-through and AR concepts, the project demonstrates how the **player’s physical space** (real environment) can become the **game space** for interactive, mixed reality experiences. The **AR.apk** and accompanying videos (`ARUnity.mp4`, `ARQuest.mp4`) illustrate the Unity setup and final application running on the Quest.

---

## Table of Contents
1. [Overview](#overview)  
2. [Technical Highlights](#technical-highlights)  
3. [Files in This Repository](#files-in-this-repository)  
4. [Running the APK on Quest](#running-the-apk-on-quest)  
5. [Player Space, Environment, and Interactions](#player-space-environment-and-interactions)  
6. [Mixed Reality Terminology](#mixed-reality-terminology)  
7. [Future Possibilities](#future-possibilities)  
8. [Contact & License](#contact--license)

---

## 1. Overview
This demo merges elements of **Augmented Reality** with the **VR capabilities** of the Quest 2:
- **Unity** was used to create an AR pass-through style experience, harnessing the player’s real environment as part of the game world.  
- **Meta Quest Developer Hub** (MQDH) streamlined deployment, debugging, and performance checks on the headset.

By installing and running the provided **AR.apk**, you can see how the in-editor Unity setup translates to a standalone mixed reality application on the Quest.

---

## 2. Technical Highlights
1. **Unity Project Setup**  
   - Unity’s **XR Plugin Management** and optional **AR Foundation** dependencies let you integrate pass-through or partial AR effects on the Quest.  
   - Scenes combine VR camera rigs with references to the real environment.

2. **Meta Quest Developer Hub (MQDH)**  
   - Offers quick APK sideloading.  
   - Monitors logs (logcat) for real-time error or performance details.  
   - Manages multiple builds and device screenshots/recordings.

3. **Real-World & Game-World Overlap**  
   - The user’s **physical environment** is recognized as an anchor or baseline for the AR content, bridging real space with digital overlays.

---

## 3. Files in This Repository
- **AR.apk**  
  - The packaged Android build ready for sideloading onto the Quest or any compatible device.

- **ARUnity.mp4**  
  - Video demonstration of the **Unity Editor** setup, showing how scenes and scripts are arranged.

- **ARQuest.mp4**  
  - A short clip capturing the **Quest headset** view, illustrating how the final experience looks in pass-through or partial AR mode.

- **README.md**  
  - This documentation.

---

## 4. Running the APK on Quest
1. **Enable Developer Mode**  
   - In the **Meta Quest** mobile app or with the VR device itself, activate Developer Mode.
2. **Install Meta Quest Developer Hub (MQDH)**  
   - Download from [Oculus Developer](https://developer.oculus.com/) site.  
   - Connect your Quest via **USB** or **wireless ADB**.
3. **Sideload the APK**  
   - Launch MQDH → **My Device** → **Apps** → **Install APK**.  
   - Alternatively, use `adb install AR.apk` if you prefer command-line.
4. **Launch the App**  
   - On the Quest, go to **Apps** → **Unknown Sources** → find **AR**.  
   - Start the application to see your real environment integrated with virtual content.

---

## 5. Player Space, Environment, and Interactions

- **Player Space**  
  - Represents the **real area** you occupy. The Quest’s position tracking merges your movements with Unity’s coordinate system.
- **Environment as Game Space**  
  - The camera feed or pass-through transforms your surroundings into a **dynamic stage**. Virtual objects may be anchored relative to physical surfaces or appear to float in mid-air.
- **Interactables & Interactions**  
  - Basic examples could include:
    - **Gaze/Pointer**: Focusing on an object triggers highlighting or distance-based events.  
    - **Controller Input**: Pressing triggers or grip buttons to pick up or rotate items.  
  - Unity’s **XR Interaction Toolkit** can unify these interactions across AR/VR experiences.

---

## 6. Mixed Reality Terminology

1. **MR (Mixed Reality)**  
   - A spectrum between fully real and fully virtual experiences, where real and digital content coexist and interact in real time.
2. **Pass-Through**  
   - A VR headset technique that uses onboard cameras to show the user’s real environment, enabling AR-like overlays.
3. **Player Anchor / World Anchor**  
   - A reference point (in software) linking digital objects to stable positions in the user’s physical space.
4. **Pose Tracking**  
   - Combining sensor data (IMUs, cameras, etc.) to update the user’s head and controller positions within the 3D scene.

---

## 7. Future Possibilities
1. **Enhanced Hand Tracking**  
   - Remove reliance on controllers, letting the Quest’s built-in hand tracking manage gestures for object manipulation.
2. **ARCore Integration**  
   - Extend the app to run on Android phones that support ARCore, bridging pass-through AR across multiple devices.
3. **Networking for Shared Spaces**  
   - Real-time multiplayer where multiple Quest users share a single mixed reality environment.
4. **AI Scene Understanding**  
   - Integrate computer vision methods for dynamic object detection or semantic labeling of physical surfaces.

---

## 8. Contact & License
**Author:**  
- [Ashish Paka](https://github.com/Ashish-Paka)

**License:**  
- This project is provided under the [MIT License](LICENSE) (or specify if different).

**Further Inquiries / Issues:**  
- [Open an Issue](https://github.com/Ashish-Paka/AugmentedReality_in_Quest_Android_unity/issues) detailing suggestions or encountered bugs.  
- Pull requests are welcomed to expand or refine this project.

**Enjoy exploring the boundaries of Mixed Reality with Unity, MQDH, and Meta Quest!**  
Watch the attached videos (`ARUnity.mp4`, `ARQuest.mp4`) for more insights on setup and final deployment.
