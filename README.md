# Tailwind CSS Practice Project

This repository is for **practicing Tailwind CSS** by cloning a given UI design.  
Your goal is to **recreate the sample UI exactly** using **Tailwind CSS CLI and Node.js**.

---

## 📁 Project Structure

```
tailwindcss-practice/
│
├── img/
│   └── (7 iPhone images – use these assets in the UI)
│
├── src/
│   └── (place all your HTML files here)
│
├── task-tailwind.png
│   └── (sample UI that you need to clone)
│
└── README.md
```

---

## 🎯 Objective

- Clone the UI design shown in **`task-tailwind.png`**
- Use **Tailwind CSS (CLI)** only
- Do **NOT** use any UI frameworks (Bootstrap, Material UI, etc.)
- Focus on layout, spacing, typography, and responsiveness

---

## 🛠 Requirements

Make sure you have the following installed:

- **Node.js** (v18 or later recommended)
- **npm** (comes with Node.js)

---

## 🚀 Getting Started

### 1️⃣ Clone the Repository

```bash
git clone https://github.com/enehry/tailwindcss-practice.git
cd tailwindcss-practice
```

---

### 2️⃣ Initialize Node.js

```bash
npm init -y
```

---

### 3️⃣ Install Tailwind CSS via CLI

```bash
npm install -D tailwindcss
npx tailwindcss init
```

---

### 4️⃣ Configure Tailwind

Edit **`tailwind.config.js`**:

```js
/** @type {import('tailwindcss').Config} */
module.exports = {
  content: ["./src/**/*.{html,js}"],
  theme: {
    extend: {},
  },
  plugins: [],
}
```

---

### 5️⃣ Create Tailwind Input File

Create a CSS file (example: `src/input.css`):

```css
@tailwind base;
@tailwind components;
@tailwind utilities;
```

---

### 6️⃣ Build Tailwind CSS

Run the Tailwind CLI build command:

```bash
npx tailwindcss -i ./src/input.css -o ./src/output.css --watch
```

This will generate `output.css` and automatically rebuild on changes.

---

## 🧩 Development Guidelines

- Place **HTML files inside the `src/` folder**
- Link `output.css` in your HTML file
- Use images from the `img/` folder
- Match:
  - Layout
  - Colors
  - Font sizes
  - Spacing
  - Responsive behavior

---

## 📱 Assets

- **`img/`** contains **7 iPhone images** you must use
- **`task-tailwind.png`** is the **reference UI**

⚠️ Pixel-perfect accuracy is encouraged.

---

## 📌 Rules

- ✅ Use Tailwind utility classes only  
- ❌ No custom CSS (unless absolutely necessary)  
- ❌ No external CSS frameworks  
- ✅ Use semantic HTML  

---

## 📦 Optional NPM Script

You may add this to `package.json`:

```json
"scripts": {
  "dev": "tailwindcss -i ./src/input.css -o ./src/output.css --watch"
}
```

Then run:

```bash
npm run dev
```

---

## 🏁 Goal

By completing this task, you should be comfortable with:

- Tailwind CSS utilities  
- Responsive design  
- Tailwind CLI workflow  
- Translating UI designs into code  

---

Happy coding 🚀
