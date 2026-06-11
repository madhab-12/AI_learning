# 3D Academic Literature Semantic Network 🌐✨

An interactive 3D web platform that maps complex relationships among academic fields, research methodologies, prominent scientists, and publications. By combining Natural Language Processing (NLP) with dynamic 3D force-directed graphing, this project converts unstructured data into an immersive knowledge discovery environment.

![Network Visualization](result_graph.png)

---

## 🛠️ Key Features

* **Interactive 3D Universe:** Spin, pan, and zoom through a live data web using your mouse.
* **Neighborhood Highlighting:** Hover over any node to highlight its direct connections and automatically fade everything else out.
* **Heads-Up Display (HUD):** Click any node to instantly slide open a detailed profile card featuring automated research recommendations.
* **Data-Driven Colors:** Nodes are smartly color-coded into distinct categories (Domains, Methods, Researchers, and Publications).

---

## 🏗️ Project Architecture

The system splits the work into two simple layers:

* **The NLP Processing Pipeline (`ACE080BCT035_LAB.ipynb`):** Uses Part-of-Speech (POS) tagging and Named Entity Recognition (NER) to scan text and output clean, structured knowledge pairs (e.g., `[Author] -> AUTHORED -> [Paper]`).
* **The Web Visualization Layer (`index1.html`):** Ingests organized network data and renders it dynamically using WebGL and Three.js libraries via the `3d-force-graph` engine.

---

## 📊 Data Structure Sample

The application reads structural relationships from the backend pipeline formatted within a JSON dataset using the following node/link layout:

```json
{
  "nodes": [
    {
      "id": "Computer Vision",
      "group": "Domain",
      "category": "Academic Field",
      "rec": "Review literature cross-sections to find multi-disciplinary opportunities."
    }
  ],
  "links": [
    {
      "source": "Dr_G_Hinton",
      "target": "Contrastive Node Clustering via Graph Diffusion Wavelets",
      "label": "AUTHORED"
    }
  ]
}
