3D Academic Semantic Network 🌐✨
This project takes academic data (like research papers, fields of study, and authors) and turns it into an interactive 3D visual network graph. Instead of reading flat text, you can fly through a 3D space to see how different research topics, scientists, and publications connect to each other.

🚀 What This Project Does
Reads Text & Finds Connections (ACE080BCT035_LAB.ipynb)

Uses Natural Language Processing (NLP) to break down text.

Finds important names (like Dr. G. Hinton) and concepts (like Computer Vision).

Connects them together into "triples" (Subject ➔ Action ➔ Object), such as:

[Dr. G. Hinton] ➔ AUTHORED ➔ [Deep Learning Paper].

Saves Structured Data (network_data.json)

Organizes everything into a clean list of Nodes (the points/dots) and Links (the lines connecting them).

Displays a Beautiful 3D World (index1.html)

Uses WebGL and Three.js to show a glowing, interactive network in your web browser.

🛠️ Features
3D Flight & Control: Zoom in, rotate, and pan around the network using your mouse.

Smart Highlighting: Hover your mouse over any point (node) to highlight its direct connections and dim everything else.

Information Cards: Click on a node to open a sleek, cyberpunk-style sidebar that tells you exactly what it is and gives you a "recommendation" step.

Color Coding: Everything is organized neatly into color groups (Domains, Methods, Researchers, and Publications).

💻 How to Run It on Your Computer
Step 1: Clone the Project
Open your terminal or command prompt and run:

Bash
git clone https://github.com/your-username/academic-semantic-network.git
cd academic-semantic-network
Step 2: Start a Simple Local Server
Because web browsers block files from loading directly from your computer for security reasons, you need to spin up a quick local web server.

If you have Python installed, just run this command:

Bash
python -m http.server 8000
Step 3: View the 3D Graph
Open your web browser and go to:

Plaintext
http://localhost:8000/index1.html

🕹️ Interaction Guide
Rotate Space: Left-click and drag anywhere on the canvas to orbit the 3D graph view.

Pan Canvas: Right-click and drag to glide seamlessly across various thematic clusters.

Zoom Scope: Use the scroll wheel to dive deep into localized graph neighborhoods.

Inspect Entities: Hover over individual nodes to illuminate their direct connections, and click them to reveal actionable data in the HUD (Heads-Up Display) overlay.

🔮 Future Enhancements
Real-World Scalability: Integrating automated ingestion pipelines from live scholarly APIs (e.g., Semantic Scholar, arXiv).

Graph Neural Networks (GNNs): Transitioning static recommendation attributes into deep link-prediction models using structural embeddings.

Temporal Dimensions: Adding timeline scaling animations to watch machine learning paradigms shift and evolve across decades.
