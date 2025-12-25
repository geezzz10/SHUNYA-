# SHUNYA-
A learning bridge translating voice to OpenSCAD code for intuitive 3D design.
🛠️ Voice-to-CAD: The Educational Bridge
"Demystifying 3D engineering by translating spoken ideas into visible OpenSCAD code, making spatial design accessible to everyone."

🌟 Vision & Motivation
Traditional CAD software has a steep learning curve that discourages many beginners. Our project, Voice-to-CAD, acts as a "learning bridge." By using natural language, users can generate 3D geometry instantly, helping them understand the logical relationship between descriptive language and coordinate-based engineering code.

🚀 Key Features
🎙️ Natural Language Processing: Powered by Gemini 1.5 Flash to interpret complex spatial descriptions.

💻 Live Code Generation: Translates voice prompts into clean, render-ready OpenSCAD scripts.

🌐 Dual-Node Architecture: A distributed system with a FastAPI backend and a Streamlit frontend for high performance.

📊 Design Persistence: Integrated with MongoDB to track project history and learning progress.

🏗️ System Architecture
Our project uses a modern distributed architecture across two nodes to separate concerns and ensure a smooth user experience.

Frontend (Node A): A Streamlit interface that handles user input and displays the 3D code.

Backend (Node B): A FastAPI server that communicates with the Gemini API and manages data storage.

Database: MongoDB stores the generated code and prompts for future reference.

🛠️ Tech StackComponentTechnologyLanguagePython 3.10+AI ModelGoogle Gemini 1.5 FlashBackendFastAPI & UvicornFrontendStreamlitDatabaseMongoDBCAD EngineOpenSCAD🚦 Getting Started
Getting Started
Prerequisites
Python 3.9+ installed on both nodes.

A Google Gemini API Key from AI Studio.

MongoDB installed and running locally.

Installation & Setup
Clone the repository:

Bash

git clone https://github.com/YOUR_USERNAME/Voice-to-CAD-Bridge.git
cd Voice-to-CAD-Bridge
Install dependencies:

Bash

pip install -r requirements.txt
Configure Environment: Create a .env file in the root directory:

Code snippet

GOOGLE_API_KEY=your_api_key_here
MONGODB_URI=mongodb://localhost:27017
Launch the Backend:

Bash

python main.py
Launch the Frontend:

Bash

streamlit run app.py
💡 Example Prompts
Try these to see the "learning bridge" in action:

"Create a 20mm cube with a 5mm hole right through the center."

"Generate a gear with 12 teeth and a thickness of 3mm."

"Make a staircase with 10 steps, each 2mm high."

👥 The Team
Bhavya Agarwal - Backend
Aarchi Sa0 - Frontend
