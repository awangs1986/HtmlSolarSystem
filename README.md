# ORBIT — Solar System Explorer

> **Project origin | 项目来源**<br>
> This application was generated in a single pass by **Astra**.<br>
> 本项目由 **Astra 一次性生成**。

## 🧪 智能体能力测试 | Agent Capability Test

> **中文**<br>
> 这是一个智能体能力测试的题目，可以简单测试模型能力。使用一段提示词：<br>
> **“生成一个名为“ORBIT · 太阳系漫游”的单文件 HTML，内嵌全部代码和资源以支持离线运行，使用 Three.js/WebGL 展示太阳与九颗天体（水星至海王星及冥王星）的三维公转和自转，包含高清表面纹理、太阳辉光、星空、小行星带、地球大气与云层、木星条纹和大红斑、分层土星环、天王星倾斜自转及冥王星心形冰原，采用深色背景、暖金色点缀和简洁精致的天文观测界面，左侧显示行星介绍、直径、公转周期、平均日距与轴倾角，底部提供行星导航，支持拖拽旋转、滚轮及双指缩放、点击行星平滑进入近景、一键返回全景、暂停播放、速度调节、轨道与名称开关、中英文即时切换和移动端适配，并注明尺寸与轨道采用示意比例、冥王星属于矮行星。”**
>
> **English**<br>
> This is an agent capability test that offers a simple way to assess a model’s capabilities. Use this prompt:<br>
> **“Create a self-contained, offline-ready HTML file named “ORBIT · Solar System Explorer” with all code and assets embedded, using Three.js/WebGL to animate the orbits and axial rotation of the Sun’s nine worlds—Mercury through Neptune plus Pluto—with detailed surface textures, solar glow, a starfield, an asteroid belt, Earth’s atmosphere and clouds, Jupiter’s bands and Great Red Spot, layered Saturn rings, Uranus’s tilted rotation, and Pluto’s heart-shaped ice region; use a refined astronomical observatory interface with a dark background and warm gold accents, a left-hand panel showing each world’s description, diameter, orbital period, mean distance from the Sun, and axial tilt, plus bottom planet navigation; support drag-to-rotate, mouse-wheel and pinch zoom, smooth close-up transitions when selecting planets, one-click return to the overview, pause/resume, speed adjustment, orbit and label toggles, instant English/Chinese switching, and responsive mobile layouts, while noting that sizes and orbits are illustrative and Pluto is a dwarf planet.”**

---

ORBIT is a self-contained, interactive 3D tour of the Sun, the eight planets, and Pluto. It pairs an orbiting WebGL solar system with a calm, editorial-style explorer interface. Select a world to open its profile, then zoom in to study its surface, atmosphere, or rings.

The page supports **English and Chinese**. Use the language button in the upper-right corner to switch the entire interface and planet information instantly.

## Screenshots

### Solar system overview

![ORBIT solar system overview in Chinese](screenshots/overview-zh.png)

### Saturn close-up

![ORBIT close-up view of Saturn in English](screenshots/saturn-closeup-en.png)

## A simple test of an AI model’s intelligence level

This project can serve as a small, informal test of an AI model’s ability to understand and complete a multi-part creative coding task. The task is approachable, but it asks the model to connect several kinds of work: building a 3D scene, making the scene usable, presenting meaningful information, and delivering a finished project.

It is **not** a standardized intelligence test, a scientific benchmark, or a measure of general IQ. Results depend on the prompt, the model’s tools, and the evaluator. Use it as a quick, qualitative way to compare how well models turn a short brief into a coherent working experience.

### Short-prompt baseline

> Create an HTML animation of the nine planets orbiting the Sun. It should let me rotate the view and zoom in or out, and each planet should have its own distinctive features.

Choose one prompt before the test. Give each agent the same prompt, starting files, tools, browser, and time limit. Open the delivered HTML and score only behavior you can verify. Award 0, 1, or 2 points in each category below.

| Prompt requirement | 0 points | 1 point | 2 points |
| --- | --- | --- | --- |
| Nine worlds and the Sun | No usable solar-system scene | The Sun and some, but not all, of the nine worlds are visible | The Sun and all nine worlds are visible |
| Orbital animation | No visible orbital motion | Some worlds orbit, or motion is clearly broken | All nine worlds visibly orbit the Sun |
| Rotatable view | The view cannot be rotated | Rotation works but is difficult or unreliable | The user can rotate the view smoothly and predictably |
| Zoom | The view cannot be zoomed | Zoom works but is difficult or unreliable | The user can zoom in and out smoothly and predictably |
| Individual features | Worlds are visually interchangeable | Some worlds have recognizable, distinct features | Every world has its own recognizable visual characteristics |

**Short-prompt score: 0–10 points.** Count Pluto as the ninth world for this historical wording; Pluto is classified as a dwarf planet today. Bilingual text, planet facts, and visual polish are welcome, but the short prompt does not request them, so they do not affect this score.

### Detailed-prompt extension

If you use the longer bilingual prompt at the top of this README, score the five core categories above **plus** these five categories. This yields a separate **0–20 point detailed-prompt score**; do not compare it directly with a short-prompt score.

| Additional requirement | 0 points | 1 point | 2 points |
| --- | --- | --- | --- |
| Single-file WebGL delivery | No working WebGL page | WebGL works, but the page needs external files or a network connection | One HTML file contains all code and assets and works offline |
| Requested scene details | No requested textures or scene details | Some requested details are recognizable | Detailed textures, axial rotation, Sun glow, starfield, asteroid belt, and all specifically named planetary features are present |
| Interface and planet information | No usable planet navigation or information | Navigation, styling, or planet information is incomplete | Dark-and-gold observatory interface, bottom navigation, and descriptions plus all four requested facts for each world |
| Exploration and playback controls | No requested extra controls work | Some controls work | Planet selection and close-up, overview return, pause/resume, speed, orbit lines, and labels all work |
| Language, mobile, and scientific notes | None of these requirements are met | Some are met | Instant English/Chinese switch, usable mobile layout, and explicit scale and Pluto notes |

A page that cannot render earns 0 in every category. Test controls directly; do not award points for claims in documentation or source code alone. Record category scores alongside the total so another reader can see where a result succeeded or fell short. These are practical task scores, not scientific measures of general intelligence.

## Features

- **Three-dimensional WebGL scene** with a textured Sun, nine orbiting worlds, starfield, asteroid belt, and adjustable orbit and name overlays.
- **Distinct planetary details:** cloud-shrouded Venus, Earth's oceans and clouds, Jupiter’s banded atmosphere, Saturn’s rings, tilted Uranus, and an illustrated Pluto surface.
- **Planet profiles** with a short description, diameter, orbital period, average distance from the Sun, and axial tilt.
- **Close-up exploration** for each planet, with a quick return to the full solar-system view.
- **Camera controls:** drag to rotate, mouse wheel to zoom, pinch on touchscreens, and on-screen zoom and reset controls.
- **Animation controls:** pause or resume the motion and adjust the simulation speed.
- **One-click English/Chinese switch** for the interface, controls, labels, and planet profiles.
- **Single-file delivery:** Three.js and the planet maps are embedded in `astra/index.html`; the page makes no external requests when opened.
- Responsive layout for desktop and mobile screens.

> Planet sizes, distances, orbital spacing, and simulation speed are visualized for clarity; they are not presented to scale. Pluto is included as a dwarf planet.

## Run it

Open [`astra/index.html`](astra/index.html) in a current browser with WebGL enabled. The repository root redirects to this page for GitHub Pages. No package installation, build step, or network connection is required. Hardware acceleration is recommended for smooth rendering.

## Controls

| Action | Control |
| --- | --- |
| Rotate the view | Drag on the solar-system canvas |
| Zoom | Scroll, pinch, or use the `+` and `−` buttons |
| Explore a planet | Select a planet in the bottom navigation or click its sphere |
| Return to the overview | Use **Overview** / **全景** |
| Pause or resume | Use the `Ⅱ` / `▶` button, or press Space while the canvas is focused |
| Rotate with a keyboard | Focus the canvas and use the arrow keys |
| Show or hide orbit lines and labels | Use the controls in the top-right corner |
| Change language | Use **EN** / **中文** in the top-right corner |

## Implementation

- HTML, CSS, and JavaScript in one page
- [Three.js](https://threejs.org/), bundled in `astra/index.html` (MIT License)
- Planet texture maps from [Solar System Scope](https://www.solarsystemscope.com/textures/) (CC BY 4.0)

The interface and simulation run locally. The source texture maps remain subject to their original attribution and license.
