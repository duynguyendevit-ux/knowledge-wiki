---
title: Lịch Sử Unity Game Engine
tags: [unity, game-engine, history, timeline]
date: 2026-06-09
---

# Lịch Sử Unity Game Engine

## 📅 Timeline Chính

### 2004 - Khởi Đầu

**Thành lập bởi 3 nhà phát triển người Đan Mạch:**
- David Helgason
- Joachim Ante
- Nicholas Francis

**Mục tiêu:** "Democratize game development" - làm cho phát triển game dễ tiếp cận hơn

---

### 2005 - Ra Mắt (Unity 1.0)

- **June 8, 2005:** Unity 1.0 chính thức ra mắt
- Được giới thiệu tại **Apple WWDC** (Worldwide Developers Conference)
- Trình bày bởi **Scott Forstall** trên Mac OS X
- Ban đầu chỉ hỗ trợ **Mac OS X**

---

### 2006

- Đạt giải **Runner-up** trong Apple Design Awards
- Danh mục: Best Use of Mac OS X Graphics

---

### 2007 - Unity 2.0

**~50 tính năng mới:**
- **DirectX support** được thêm vào
- Terrain engine tối ưu cho môi trường 3D chi tiết
- Real-time dynamic shadows
- Directional lights và spotlights
- Video playback
- Version control system
- **Networking Layer** (UDP-based multiplayer)
  - Network Address Translation
  - State Synchronization
  - Remote Procedure Calls

---

### 2008 - Mobile Revolution

- Apple ra mắt **App Store**
- Unity thêm hỗ trợ **iPhone** → **Bước ngoặt lớn!**

---

### 2009 - Unity 2.5

- **March 2009:** Editor support cho **Windows**

---

## 🚀 Giai Đoạn Tăng Trưởng

### 2010 - Unity 3.0

**September 2010:**
- **Android support**
- Beast Lightmap integration
- Deferred rendering
- Built-in tree editor
- Native font rendering
- Automatic UV mapping
- Audio filters

---

### 2012 - Milestone

- **1.3 million developers** sử dụng Unity
- Top game engine cho mobile platforms (Game Developer magazine survey)
- VentureBeat: "Few companies have contributed as much to the flowing of independently produced games as Unity Technologies"

---

### 2012 - Unity 4.0

**November 2012:**
- **DirectX 11** support
- **Adobe Flash** support
- **Mecanim** animation system
- Linux preview access

---

### 2013

- Facebook tích hợp **SDK** cho Unity games
- Ad tracking, deep linking, in-game image sharing

---

### 2015 - Unity 5

**Major release:**
- Real-time global illumination
- Light mapping previews
- Unity Cloud
- New audio system
- **Nvidia PhysX 3.3**
- **WebGL support** (games chạy trên browser không cần plugin!)
- Cinematic Image Effects
- **August 2015:** Linux editor build (experimental)

**The Verge:** "Unity started with the goal of making game development universally accessible. Unity 5 is a long-awaited step towards that future."

---

### 2016

- Facebook phát triển PC gaming platform với Unity
- **Unity 5.6:**
  - **Nintendo Switch** support
  - **Facebook Gameroom**
  - **Google Daydream**
  - **Vulkan graphics API**
  - 4K video player (360° VR videos)

---

## 📆 Annual Releases (2017-2023)

### December 2016 - Version Numbering Change

- Thay đổi version numbering: từ 5.6 → **Unity 2017**
- Căn chỉnh theo năm phát hành

---

### Unity 2017

- Real-time graphics rendering engine
- Color grading và worldbuilding
- Live operations analytics
- Performance reporting
- **Timeline tool** (drag-and-drop animations)
- **Cinemachine** (smart camera system)
- **3DS Max & Maya integration**

---

### Unity 2018

- **Scriptable Render Pipeline (SRP)**
  - **HDRP** (High-Definition) - console/PC
  - **LWRP** (Lightweight) → sau đổi thành **URP (Universal)**
- Machine learning tools (Imitation Learning)
- **Magic Leap** support
- Templates cho developers mới
- **Unity Hub introduced** (project & version management)
- **March 2018:** C# source code published (reference-only license)

---

### 2020 - Massive Scale

**Statistics:**
- **1.5 billion devices** chạy Unity
- **50% mobile games** được làm bằng Unity
- **3 billion downloads/month**
- **15,000 new projects daily**

**New Features:**
- **MARS** (Mixed and Augmented Reality Studio)
- Unity Forma (automotive & retail)
- **Apple Silicon** support announced
- First beta shipped

**Popular Games:**
- Pokémon Go
- Call of Duty Mobile

---

### Unity 2021

- **Bolt** (Visual Scripting system)
- New multiplayer library
- Improved Il2cpp runtime
- Volumetric clouds (HDRP)
- Shadow caching
- Screen Space Global Illumination
- **Full Apple Silicon support** (Unity 2021.2)
- **Unity Hub 3.0** with Apple Silicon support (January 2022)

---

### Unity 2022

**Productivity improvements:**
- Faster play mode
- Faster file import
- Visual search queries
- Multi-selection in package manager

**2D improvements:**
- Accelerated core software
- Import, animation, physics improvements
- Sprite atlasing revision
- **PSD extension files** support
- Layer management (2D PSD Importer)
- **Delaunay tessellation** (2D physics)

---

### 2023 - Unity 6 Announced

**November 16, 2023:**
- Công bố **Unity 6**
- Quay lại cách đặt tên version numbering cũ

---

## 🎯 Unity 6 Era (2024-Present)

### October 17, 2024 - Unity 6 Launch

**New Features:**
- **Unity Muse** (generative AI tools)
- **Unity Sentis** (generative AI tools)
- New multiplayer workflows
- Web project performance enhancements
- Improved graphics rendering

**Revised Licensing:**
- Runtime fee announced
- **September 2024:** Runtime fee canceled (sau phản ứng tiêu cực)

---

### Current (2026)

**Latest Stable Releases:**
- **Unity 6000.4.0f1** (Mainline) - March 18, 2026
- **Unity 6000.3.12f1** (LTS)
- **Unity 6000.0.71f1** (LTS)
- **Unity 6000.5.0b1** (Beta) - March 26, 2026

---

## 💻 Technical Details

### Ngôn Ngữ Lập Trình

**Evolution:**
- **Ban đầu:** Boo, UnityScript (JavaScript-like)
- **Unity 5:** Boo removed
- **August 2017:** UnityScript deprecated
- **Current:** **C#** (primary language)

**Engine Code:**
- **Runtime:** C++
- **Scripting API:** C#
- **Mono:** Used for scripting

---

### Render Pipelines

**Three Pipelines:**
1. **Built-in Pipeline** (legacy)
2. **HDRP** (High-Definition Render Pipeline) - console/PC
3. **URP** (Universal Render Pipeline) - mobile/VR/AR

⚠️ **Note:** All three pipelines are incompatible with each other

---

## 🌍 Platforms Supported (2022.3 LTS)

### Mobile
- iOS, iPadOS, Android, Android TV, tvOS

### Desktop
- Windows, Universal Windows Platform
- macOS
- Linux, ChromeOS

### Web
- WebGL, WebGPU

### Console
- PlayStation 4, PlayStation 5
- Xbox One, Xbox Series X/S
- Nintendo Switch, Nintendo Switch 2

### VR/AR
- Meta Quest
- PlayStation VR, PlayStation VR2
- Apple Vision Pro
- Windows Mixed Reality, HoloLens
- Magic Leap
- Steam VR, Google Cardboard
- ARCore

### Formerly Supported
- Wii, Wii U
- PlayStation 3, Xbox 360
- PlayStation Vita
- Oculus, Tizen

---

## 🎮 Popular Games & Applications

**Major Titles:**
- **Pokémon Go**
- **Call of Duty Mobile**
- Hàng triệu game khác

**Industries Using Unity:**
- Gaming (primary)
- Film production
- Automotive
- Architecture
- Engineering
- Construction
- US Armed Forces

---

## 📊 Key Milestones

| Year | Milestone |
|------|-----------|
| **2004** | Founded in Denmark |
| **2005** | Unity 1.0 launched at Apple WWDC |
| **2008** | iPhone support added |
| **2010** | Android support (Unity 3.0) |
| **2012** | 1.3M developers, Unity 4.0 |
| **2015** | Unity 5 with WebGL |
| **2017** | Annual versioning system |
| **2018** | Unity Hub, SRP, 1.5B devices |
| **2020** | 50% mobile market share |
| **2024** | Unity 6 launched |

---

## 💡 Unity Asset Store

**Launched:** 2010

**Statistics (2018):**
- ~40 million downloads
- 3D and 2D assets
- Environments, tools, plugins
- User-generated content marketplace

---

## 🏆 Thành Tựu

### Market Share
- **50% of all mobile games** (2020)
- **Most popular mobile game engine**
- **Over 1.5 billion devices** running Unity (2020)

### Developer Base
- **1.3 million developers** (2012)
- **15,000 new projects daily** (2020)
- **3 billion downloads/month** (2020)

### Recognition
- Apple Design Awards (2006)
- Industry standard for indie games
- Cross-platform development leader

---

## 🎯 Triết Lý

> **"Democratize game development - making it accessible to everyone"**

Unity bắt đầu với mục tiêu làm cho phát triển game dễ tiếp cận hơn. Từ một engine cho Mac OS X, Unity đã trở thành nền tảng cross-platform hàng đầu thế giới, hỗ trợ 19+ platforms và được sử dụng bởi hàng triệu developers toàn cầu.

---

## 📚 Sources

- Wikipedia: Unity (game engine)
- Unity Technologies official documentation
- Game Developer magazine
- VentureBeat, The Verge, Financial Times coverage
- Unity blog and changelogs

---

**Last Updated:** 2026-06-09
