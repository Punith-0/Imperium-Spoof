DynamicIQ
Quick Start Guide
Review customer-support conversations, add remarks, and track completed reviews.
🚀 Launch DynamicIQ
For judges: use the deployed website. No installation or personal API key is needed when the deployment is configured by the project team.
Use the website · Run locally · Review a conversation · Need help?
Option 1: Use the website
1. Click here to open DynamicIQ.
2. Follow the Analyze and review steps below.
Dataset to upload: DynamicIQ_shuffled.csv — provided with the project submission.

Option 2: Run locally
Before starting: install Python if needed. Open the project folder in VS Code, then select Terminal → New Terminal. Your terminal must be in the folder containing app.py.
1. Install the required packages
python -m pip install -r requirements.txt
2. Configure AI mode
Create a file named .env beside app.py. If already configured, skip this step.
OPENAI_API_KEY=your_groq_api_key
OPENAI_MODEL=openai/gpt-oss-20b
Replace your_groq_api_key with your actual Groq API key. Keep this file private.
3. Start the app
python -m streamlit run app.py
4. Open the local app
If the terminal shows a different Local URL, open that URL instead. Keep the terminal running while using the app.
Analyze and review
These steps apply to both the website and the local app.
Step	What to do
1 · Select AI mode	Click the arrow at the top-left to open the sidebar. Expand Analysis settings under Workspace settings, then select AI analysis.
2 · Upload the dataset	Expand Dataset · upload or change → choose Upload dataset → upload DynamicIQ_shuffled.csv.
3 · Choose a conversation	Select Convo 1, Convo 2, etc. from the right-side list.
4 · Analyze	Click Analyze conversation. Wait for the results, then read the transcript, findings and quoted evidence.
5 · Add remarks	Enter Overall remarks. Tick I have reviewed this conversation and its available evidence.
6 · Complete the review	Click Save & Done. The conversation shows Done, and the next unfinished conversation opens.
7 · Download results	Select the reviewed conversation, expand Download saved review, then choose JSON report or Findings CSV.
