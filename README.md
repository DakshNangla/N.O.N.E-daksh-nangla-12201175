This version provides the essential overview and technical steps, which you will expand with the full architecture and results later.

-----

## **README.md: N.O.N.E. - Neural Operational Network Entity**

### **Project Overview**

**N.O.N.E.** is an autonomous, multi-agent research assistant built for the CloudCosmos Hackathon (Track 2: AI Agents). It is designed to generate real-time, fact-checked reports on complex topics by orchestrating a team of specialized AI agents, thereby reducing hallucination and improving research reliability.

### **Problem Statement**

Cloning the idea of a powerful AI assistant, the goal is to solve the problem of LLM hallucination and information overload by creating a self-verifying system that uses multiple agents to conduct research, summarize findings, and critically review the output before delivery.

### **Technical Stack**

| Category            | Component                      | Detail                   |
| :---                | :---                           | :---                 
| **Backend/API**     | **Python, FastAPI**            | High-performance API to trigger the agent workflow. 
| **Agent Framework** | **CrewAI**                     | Orchestration of the multi-agent system.
| **LLM / AI Models** | **Gemini Pro**                 | Primary LLM used for reasoning, summarization, and critique. 
| **Tools / APIs**    | **Google Search API / Serper** | Tool for the Researcher Agent to pull real-time, current information.
| **Frontend**        | Streamlit / Flask UI           | Simple web interface for input and visualization. 

### **Setup Instructions (Mandatory)**

Follow these exact steps to clone and run the project locally.

1.  **Clone the Repository:**

    ```bash
    git clone https://github.com/<your-repo-link>.git
    cd <repo-folder>
    ```

2.  **Setup Environment (using Conda):**

    ```bash
    conda create -n cloudcosmos python=3.10 -y
    conda activate cloudcosmos
    ```

3.  **Install Dependencies:**

    ```bash
    pip install -r requirements.txt
    ```

4.  **Configure API Keys:**
    Create a file named `.env` in the root directory and set your LLM and search tool API keys:

    ```
    # Replace with your actual keys
    GEMINI_API_KEY="YOUR_GEMINI_KEY_HERE"
    SERPER_API_KEY="YOUR_SERPER_KEY_HERE" 
    ```

5.  **Run the Application (FastAPI Backend):**

    ```bash
    uvicorn app:app --reload
    ```

6.  **Run the Frontend (Example for Streamlit):**

    ```bash
    # Assuming your frontend entry file is in a 'frontend' directory
    streamlit run frontend/app.py 
    ```

-----

### **Next Steps**

  * **Demo Video (Mandatory):** Upload the demo video ($\le 3$ minutes) to YouTube and add the link here.
      * **YouTube Link:** `https://youtu.be/your-demo-link`
  * **Deployment (Optional):** Add your live link here.
      * **Live Demo URL:** `https://your-deployed-app-link.com`
