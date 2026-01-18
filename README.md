

Browser
The Chrome browser is recommended

# Install Deno
curl -fsSL https://deno.land/install.sh | sh
# Install Deno Jupyter Kernel
deno jupyter --install
# Activate Deno Jupyter Kernel
deno jupyter --unstable

You should be able to select the Deno kernel from the available kernels list.
Sign up for LangSmith
Create a LangSmith account and API key 

this is my Key: lsv2_Apt_A7a1d183ee8b242b28a98c2840bf78214_A2198fd84a5



Installation
Clone the repository:
git clone https://github.com/langchain-ai/lca-langchainV1-essentials.git //  Download new update file from here
cd ./lca-langchainV1-essentials/js
Install the package and dependencies:

corepack enable // is command ko Js ke ander use karna hai jis jaga packages file hai
pnpm install
Create a .env file in the project root with your API keys:

# Create .env file
cp example.env .env
Add your API keys to the .env file:

# Required for model usage
ANTHROPIC_API_KEY=your_anthropic_api_key_here

# Optional: For evaluation and tracing
LANGSMITH_API_KEY=your_langsmith_api_key_here
LANGSMITH_TRACING=true
LANGSMITH_PROJECT=lc-essentials

# If you are on the EU instance:
LANGSMITH_ENDPOINT=https://eu.api.smith.langchain.com // this is a link of langchain server



-----------------------------------------------------------------------------------------


Running Jupyter Notebooks
If you don’t have Jupyter installed, you can install it using pip or pipx:

# Using pip with a virtual environment
python3 -m venv .venv
source .venv/bin/activate
pip install jupyterlab
Once Jupyter is installed and the Deno kernel is set up (see Prerequisites), start Jupyter:

# Start Jupyter Lab 
jupyter lab - is command ko use karo to run jupyter file

This will open Jupyter in your browser. When opening any of the .ipynb files in this directory, make sure to select the Deno kernel from the kernel selector in the top-right corner of the notebook interface.
