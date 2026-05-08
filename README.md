OpportunityAgent is a proactive AI agent built using the OpenClaw 2026 framework. It is designed to solve the "information overload" problem for engineering students by automating the search and summarization of niche AI/ML internships from high-signal platforms like Reddit.

Theme: Theme 3: Productivity Platforms

Developer: Monisha M, Pocha Om Shivani, Mehak Malik

Institution: RV College of Engineering (RVCE), CSE[AIML]

🛠️ The Solution
The agent bridges the gap between student ambition and career opportunities by delegating the "toil" of manual searching to an intelligent orchestrator. It runs on local hardware to ensure data sovereignty while leveraging high-speed cloud inference for reasoning.

✨ Key Features
Proactive Discovery: Utilizes the OpenClaw Heartbeat Daemon to execute daily searches at 8:00 AM without user prompting.

Intelligent Summarization: Powered by Groq Llama-3-8b for near-instant extraction of internship details and application links.

Durable Configuration: Uses openclaw.json and .env for persistent session management and secure credential handling.

🚀 Setup & Installation
Install Dependencies: Ensure Node.js ≥ 22 is installed on your system.

Initialize Environment:

PowerShell
openclaw setup
Configure API Keys: Create a .env file in the root directory and add your GROQ_API_KEY.

Set Agent Model:

PowerShell
openclaw config set agents.default.model "groq/llama3-8b-8192"
Launch the Gateway:

PowerShell
openclaw gateway --allow-unconfigured
📈 Usage
Manual Trigger: Run openclaw chat and ask: "fetch me some AI internships from Reddit".

Autonomous Mode: The agent automatically monitors the HEARTBEAT.md file to perform scheduled tasks.

🧠 AI Disclosure
Core Model: Groq Llama-3-8b-8192.

Development Support: Gemini was used for architecture design, Node.js event-loop debugging, and structuring project artifacts.
