# 🚀 Nexstern – DAG Pipeline Editor  
A professional-grade visual editor for creating and validating **Directed Acyclic Graphs (DAGs)** in the browser. Designed for data scientists, developers, and workflow architects.

> 👩‍💻 Built from scratch by [**Snehalatha Medasari**](https://github.com/Snehalatha-23) using React, TypeScript, Tailwind CSS, and Dagre.

---

## 🌐 Live Demo  
🎯 [Try it Live → nexstern-by-sneha.vercel.app](https://nexstern-by-sneha.vercel.app)

---

## 🧠 Overview

Nexstern allows users to visually create complex DAGs with node dragging, edge connection, validation, and auto-layout features. It’s intuitive, scalable, and performance-optimized.

---

## ✨ Features

- ➕ Add, delete, and drag nodes
- 🔗 Connect nodes with edges (validation prevents invalid DAGs)
- 📐 Auto-layout using **Dagre** algorithm
- 🧾 Export/import DAGs as JSON
- 🎯 Real-time DAG validation
- 🖱️ Context menu (right-click actions)
- 🔍 Zoom & pan support
- 🌈 Color-coded node types
- ⚡ Fast performance for large graphs

---

## 🛠️ Tech Stack

| Technology       | Purpose                            |
|------------------|-------------------------------------|
| React            | Component-based UI framework        |
| TypeScript       | Type-safe development               |
| Tailwind CSS     | Utility-first CSS framework         |
| Vite             | Fast build & development tool       |
| Dagre            | DAG layout engine                   |
| Lucide Icons     | Clean & lightweight icon set        |

---

## 📦 Project Setup

### 1️⃣ Clone the Repo

```bash
git clone https://github.com/Snehalatha-23/nexstern.git
cd nexstern
2️⃣ Install Dependencies
bash
Copy
Edit
npm install
3️⃣ Start Local Server
bash
Copy
Edit
npm run dev
🔗 Visit http://localhost:5173 in your browser

📁 Project Structure
cpp
Copy
Edit
src/
├── components/          // Canvas, Node, Edge, PipelineEditor
├── hooks/               // useDAGValidation, useNodeManagement
├── utils/               // layoutUtils, geometryUtils
├── types/               // DAG types
📸 Screenshots
Interface (Node Canvas with Zoom & Edge Creation)


🧠 Key Innovations
✅ Canvas-Relative Coordinate Logic
ts
Copy
Edit
const canvasRect = canvas.getBoundingClientRect();
const position = {
  x: event.clientX - canvasRect.left,
  y: event.clientY - canvasRect.top
};
✅ DAG Cycle Validation
ts
Copy
Edit
function detectCycle(nodes, edges) {
  // DFS-based cycle detection
}
✅ Auto Layout with Dagre
ts
Copy
Edit
dagre.layout(graph);
const layoutedNodes = nodes.map(node => ({
  ...node,
  position: {
    x: graph.node(node.id).x,
    y: graph.node(node.id).y
  }
}));
🙋‍♀️ About Me
Hi! I’m Snehalatha Medasari, a passionate frontend developer with a vision to simplify complex interfaces through innovation and interactivity.

🔭 I build web apps using React, TypeScript, and Node.js

🎯 I specialize in UI/UX, real-time logic, and visual tools

💼 GitHub: @Snehalatha-23

💡 Future Enhancements
🌙 Dark Mode support

🔁 Real-time collaboration (WebSocket)

📥 Cloud DAG Save & Load

✨ Node Templates & Custom Plugins

📄 License
This project is licensed under the MIT License.

🧠 “Innovation isn’t just about having ideas — it’s about building them.”
— Sneha Latha

yaml
Copy
Edit

---

### ✅ Final Step

After pasting this into your `README.md`, run:

```bash
git add README.md
git commit -m "📄 Personalized README by Snehalatha"
git push
Then check your GitHub repo:
👉 https://github.com/Snehalatha-23/nexstern
