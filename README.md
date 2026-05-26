# Sign Language 3D Models

> **Open Source** · ASL 3D Animations & Rigs for Sign Language Visualization

This repository contains 3D animations, character rigs, and assets for **American Sign Language (ASL)** — built as part of **SignifyAI**, developed at the **SUDHEE 2025 CBIT Hackathon**.

## 🎬 Demo

https://github.com/user-attachments/assets/89cb8782-3274-4971-96d1-b571ae4192b7
> Sample animation: 'hello' greeting (ASL) rendered on the Eric character.

---

## 📁 Folder Structure

```
SignLanguage3DModels/
│
├── animations/
│   ├── angry/            # Word animations with angry facial expression
│   ├── letters/          # A–Z fingerspelling animations (normal expression)
│   ├── numbers/          # Numbers 0–7 animations (normal expression)
│   ├── sad/              # Word animations with sad facial expression
│   └── words_normal/     # Common word animations (normal expression)
│
├── eric_fbx/             # Eric character — FBX files + textures (A-pose & T-pose)
│
├── rig/                  # Animated rigs for letters A–Z (apply to any character)
│
└── media/                # Sample images and videos of working animations
```

---

## 🚀 About the Project — SignifyAI

This asset pack was built for **SignifyAI**, a real-time sign language generation system created at **SUDHEE 2025, CBIT Hackathon**.

**The problem:** Millions of people with hearing and speech impairments face communication barriers daily. Existing solutions are slow, inaccurate, or lack emotional depth.

**Our solution:**
- 🎤 Converts spoken language → English → English Sign Grammar
- 😊 Uses Sentiment Analysis to reflect emotions in signing
- 🤖 Generates real-time sign animations using a custom AI avatar
- 🌍 Makes communication seamless and expressive for the deaf community


## 🧩 How to Use the Animations

### Option 1 — Use with the Eric Character (Included)

The `eric_fbx/` folder contains the **Eric character** in both **A-pose** and **T-pose** along with his textures. You can directly import him into your project and apply any animation from the `animations/` folder.

1. Import `eric_fbx/Eric_TPose.fbx` (or A-pose) into your 3D software (Blender, Unity, Unreal Engine, etc.)
2. Import any animation `.fbx` from the `animations/` subfolders
3. Apply the animation to Eric's armature/skeleton
4. Export or render as needed

---

### Option 2 — Use the Rigs with Your Own Character

The `rig/` folder contains **letter rigs (A–Z)** that can be retargeted to any humanoid character.

#### Step 1: Download a Free Character
You can download free humanoid characters from:
- [Mixamo](https://www.mixamo.com) — Free rigged characters, no login needed for downloads
- [Sketchfab](https://sketchfab.com) — Search "rigged humanoid free"
- [ReadyPlayerMe](https://readyplayer.me) — Free custom avatars (GLB/FBX)
- [TurboSquid](https://turbosquid.com) — Filter by free + rigged

> ✅ Make sure the character is **rigged with a humanoid skeleton** and exported as `.fbx` or `.glb`.

#### Step 2: Import into Blender (Recommended — Free)
1. Open Blender → `File > Import > FBX` → import your character
2. Import the rig from `rig/letter_A.fbx` (or whichever letter you need)
3. Select your character's armature

#### Step 3: Retarget the Animation
In **Blender**:
1. Select your character's armature
2. Go to **Object Properties > Relations > Parent** and link it to the animation rig
3. Use the **BoneMapper** or the **Action Editor** to copy the animation action from the rig to your character's bones
4. Alternatively, use the **NLA Editor** to bake the animation onto your character

In **Unity**:
1. Import your character and set the rig type to **Humanoid** in the Inspector
2. Import the animation FBX from `rig/` and also set it to **Humanoid**
3. Open the **Animator** and drag the animation clip onto your character's Animator Controller

In **Unreal Engine**:
1. Import your character FBX with skeleton
2. Import the rig animation FBX and choose **"Use Existing Skeleton"** when prompted, selecting your character's skeleton
3. Apply via the **Animation Blueprint** or **Sequencer**

---

## 🎭 Emotion Variants

Animations are available in multiple emotional expressions to make signing more natural and communicative:

| Folder | Expression | Content |
|---|---|---|
| `animations/letters/` | Normal | A–Z fingerspelling |
| `animations/numbers/` | Normal | Numbers 0–7 |
| `animations/words_normal/` | Normal | Common words |
| `animations/angry/` | Angry | Selected words |
| `animations/sad/` | Sad | Selected words |

---

## 🛠️ Recommended Tools

| Tool | Purpose | Cost |
|---|---|---|
| [Blender](https://blender.org) | 3D editing, retargeting, rendering | Free |
| [Unity](https://unity.com) | Real-time game/app integration | Free tier |
| [Unreal Engine](https://unrealengine.com) | High-fidelity real-time rendering | Free |
| [Mixamo](https://mixamo.com) | Free rigged character downloads | Free |

---

## 📜 License

This project is released as **open source** for educational, research, and non-commercial use. Feel free to use, modify, and build upon these assets to create more inclusive technology.



---



## 📬 Contact

**Mohammad Abdul Muqeet** 
[LinkedIn](https://www.linkedin.com/in/mabdulmuqeet/)

> *"No voice should go unheard."* — SignifyAI Team
