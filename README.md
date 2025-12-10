🧠 Etherscan Agent (Ollama + LangChain + Streamlit)

An intelligent Ethereum blockchain assistant powered by Ollama (local LLM), LangChain tools, and Etherscan API.
Ask natural-language questions about Ethereum mainnet, and the agent will dynamically call tools to fetch the correct blockchain data.

Built by Roopa, Yashwanth, Rohith.



🚀 Features
Query Ethereum blockchain using plain English.

Powered by a local LLM running on your machine (Ollama + Mistral).

LangChain agent intelligently decides which tool to call.

Fully interactive Streamlit UI.


Support for wide range of Ethereum questions:
Latest block info
Miner address
Transaction count
Gas used
Ether balance of any address
Much more (via modular Etherscan tools)



📦 Installation (macOS)

1️⃣ Install Ollama (LLM engine)

Download for macOS:
👉 https://ollama.com/download

Open the Ollama.app. This automatically starts the local server on:
http://localhost:11434

2️⃣ Pull the Mistral model: 
ollama pull mistral

3️⃣ Clone your repository: 
git clone https://github.com/<your-username>/<repo-name>.git
cd <repo-name>

4️⃣ Create a virtual environment: 
python3 -m venv venv
source venv/bin/activate

5️⃣ Install dependencies
pip install -r requirements.txt

If you don’t have a requirements file, install manually:
pip install langchain==0.2.16 langchain-core==0.2.38 langchain-community==0.2.16 streamlit requests

6️⃣ Add your Etherscan API key

Edit etherscan_agent.py:
ETHERSCAN_API_KEY = "YOUR_API_KEY_HERE"

(Do NOT commit real API keys to GitHub.)



▶️ Running the Project
1️⃣ Activate virtual environment:  source venv/bin/activate

2️⃣ Start the Streamlit UI: streamlit run app.py

Open the link:

👉 http://localhost:8501



🖥️ UI Preview

The UI allows you to enter any Ethereum-related question like:

What is the latest Ethereum block number?

How many transactions are in the most recent block?

What is the Ether balance of 0xd8dA…?

What is the miner address of the latest block?
