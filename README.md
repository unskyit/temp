# 🎬 Video Studio Pro

![Build Status](https://img.shields.io/badge/build-passing-brightgreen) ![Platform](https://img.shields.io/badge/platform-Browser-blue) ![License](https://img.shields.io/badge/license-MIT-green)

**Video Studio Pro** is a high-performance, completely offline, client-side video rendering and procedural generation suite built entirely for the browser. Designed with a strict offline-first philosophy, it processes heavy mathematical rendering, SVG animations, and video transcoding locally, ensuring absolute user privacy and zero server-side compute costs. 

---

### 📖 About the Project

Traditional video rendering tools rely heavily on backend servers, leading to privacy concerns, upload/download bottlenecks, and high infrastructure costs. Video Studio Pro shifts the entire rendering pipeline to the client's machine. By leveraging modern Web APIs, it allows users to generate complex procedural animations (like Spirograph curves), fine-tune visual parameters in real-time, and export directly to formats like H.264 (MP4) right from their browser window.

It features a sleek, premium dark-mode UI with built-in memory management (RAM tracking and manual Garbage Collection) to handle intensive rendering tasks without crashing the browser.

---

### ✨ Key Features

* **⚡ Client-Side Rendering:** Complete offline processing. No video data or telemetry is ever sent to a server.
* **📐 Procedural Math Generation:** Real-time generation of complex mathematical curves with adjustable parameters (Complexity, Symmetry, Color Palettes, and Deterministic Seeds).
* **🎞️ Advanced Export Controls:** Full control over export resolution (up to 4K), framerate (FPS), duration, codecs (H.264, WebM), and bitrate.
* **🎛️ Memory Management:** Real-time RAM usage monitoring with a dedicated "Force GC" (Garbage Collection) trigger for stability during heavy loads.
* **🎨 SVG Rendering & Transcoding:** Dedicated pipelines for animating vector graphics and converting existing media formats.
* **💻 Cozy, Premium UI:** A minimalist, distraction-free environment optimized for long creative sessions.

---

### 🛠️ Architecture & Tech Stack

This project pushes the boundaries of what is possible in a modern web browser, utilizing cutting-edge Web APIs to achieve desktop-level performance.

* **Core Logic:** Vanilla HTML, CSS, JavaScript
* **Graphics & Rendering:** `HTML5 Canvas API`, `WebGL`
* **Video Processing:** `WebCodecs API`, `MediaRecorder API` (and/or WASM-based encoders like `FFmpeg.wasm`)
* **Performance:** `Web Workers` (for off-threading complex math and encoding), `OffscreenCanvas`

---

### 🚀 Usage

1. **Select a Tool:** Navigate between `Math Gen`, `SVG Render`, or `Transcode` using the top tabs.
2. **Configure Parameters:** Adjust the sliders for pattern complexity, symmetry, and select your preferred color palette.
3. **Set Deterministic Seed:** Use the seed input to perfectly recreate animations across different sessions.
4. **Define Output:** Set your desired resolution, frame rate, and duration in the Export Settings sidebar.
5. **Render:** Hit **START RENDER**. The system will generate the frames and compile them into your chosen video container directly in memory, prompting a download when complete.

---
, garbage-collection, web-api, multithreading, browser-performance, local-processing, privacy-first, zero-server
