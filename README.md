# Shockwave Content Slider

A fullscreen image slider with a ripple displacement transition effect, built with **Three.js**, **GSAP**, and **Vite**.

**Author:** AJ

## Features

- WebGL shader-based ripple displacement on slide transitions
- Animated title and description text with GSAP SplitText
- Click or tap anywhere to advance slides
- Responsive fullscreen layout

## Tech Stack

- [Three.js](https://threejs.org/) — WebGL rendering and custom shaders
- [GSAP](https://gsap.com/) — text animations and transition timing
- [Vite](https://vitejs.dev/) — dev server and bundling

## Getting Started

### Prerequisites

- [Node.js](https://nodejs.org/) (v18 or later recommended)

### Install

```bash
npm install
```

### Run locally

```bash
npm run dev
```

Open the URL shown in the terminal (typically `http://localhost:5173`).

## Project Structure

```
├── index.html      # Page markup
├── script.js       # Slider logic, Three.js scene, transitions
├── shaders.js      # Vertex and fragment shaders for displacement
├── slides.js       # Slide content (titles, descriptions, images)
├── styles.css      # Layout and typography
└── package.json
```

## Customizing Slides

Edit `slides.js` to change titles, descriptions, and image paths:

```js
export const slides = [
  {
    title: "Your Title",
    description: "Your description text.",
    image: "/your-image.jpg",
  },
  // ...
];
```

Place slide images in the project root (or `public/` folder) so Vite can serve them.

## License

ISC
