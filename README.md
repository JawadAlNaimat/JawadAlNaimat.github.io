# 🎭 Motion, Micro-Interactions & Premium UI/UX Portfolio

> "UI is the body, but motion is the soul of an app." 

Welcome to my animation playground. Below is a curated selection of advanced mobile animations, transitions, and high-fidelity custom UI components built using the **Flutter framework**.

---

## ⚡ Showcase: Core Animation Archetypes

### 1. The Fluid Checkout Experience
*Smooth spatial awareness and micro-interactions designed to minimize drop-offs.*

<table width="100%">
  <tr>
    <td width="40%" valign="top">
      <h4>Key Highlights:</h4>
      <ul>
        <li><b>Glassmorphic Card Overlay:</b> Custom-painted glass blur shifting based on accelerometer input.</li>
        <li><b>Dynamic State Morphing:</b> The "Pay Now" button seamlessly morphs into a success spinner, then scales into a receipt checkmark using <code>ImplicitlyAnimatedWidget</code>.</li>
        <li><b>Physics-Based Sheets:</b> Bottom sheet uses custom spring physics ($e^{-\beta t}$) instead of rigid standard curves.</li>
      </ul>
    </td>
    <td width="60%" align="center">
      <!-- REPLACE WITH YOUR APP GIF OR MP4 -->
      <img src="https://media.giphy.com/media/your-checkout-animation.gif" width="320" alt="Fluid Checkout Animation" style="border-radius: 16px; box-shadow: 0 8px 24px rgba(0,0,0,0.2);"/>
    </td>
  </tr>
</table>

---

### 2. Immersive 3D Parallax & Food Card Transitions
*Designed for deep engagement, blending spatial depth with micro-animations.*

<table width="100%">
  <tr>
    <td width="60%" align="center">
      <!-- REPLACE WITH YOUR APP GIF OR MP4 -->
      <img src="https://media.giphy.com/media/your-3d-parallax.gif" width="320" alt="3D Parallax Food Card" style="border-radius: 16px; box-shadow: 0 8px 24px rgba(0,0,0,0.2);"/>
    </td>
    <td width="40%" valign="top">
      <h4>Key Highlights:</h4>
      <ul>
        <li><b>3D Character Integration:</b> Layered parallax matrix transformations ($4 \times 4$ Skew/Rotation) responding directly to user touch drag gestures.</li>
        <li><b>Shared Element Transitions:</b> Hero animations built completely from scratch using custom bounds and clipping clips for asymmetric expansions.</li>
        <li><b>State Syncing:</b> BLoC-driven state changes hooked directly into custom animation controllers to guarantee zero frame drops ($60\text{fps}/120\text{Hz}$).</li>
      </ul>
    </td>
  </tr>
</table>

---

## 🛠️ The Motion Engine: My Tech Stack

To achieve buttery-smooth, native-grade rendering at stable frame rates, I utilize a specialized suite of animation tools and architecture patterns within Flutter:

```text
📦 Flutter Animation Engine
 ├── 🎨 Rive & Lottie              --> Complex vector math, interactive state machines, and 3D character rigging.
 ├── 📐 CustomPainters & Canvas    --> Mathematical UI execution, custom shaders, and tailored clipping paths.
 ├── 🌪️ Implicit & Explicit Core   --> Tweens, CurvedAnimation, and precisely orchestrated AnimationControllers.
 └── 🧠 BLoC State Orchestration   --> Decoupled UI triggers emitting high-frequency ticks for synchronized UI states.
