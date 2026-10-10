DynamicIQ - How to Use
Choose one option below. The website is the easiest option.
Option 1: Use the deployed website
1. Open imperiumcbc.streamlit.app. No installation is needed.
2. Follow Analyze and review below.
Option 2: Run locally
1. Open the project folder in VS Code. Open Terminal → New Terminal. Make sure the terminal is in the folder containing app.py.
2. Install the required packages:
   python -m pip install -r requirements.txt
3. For AI mode, create or update .env in the same folder as app.py:
   OPENAI_API_KEY=your_groq_api_key
   OPENAI_MODEL=openai/gpt-oss-20b
   Replace your_groq_api_key with your actual Groq API key. If already configured, skip this step.
4. Start the application:
   python -m streamlit run app.py
5. Open the Local URL shown in the terminal, usually http://localhost:8501. Keep the terminal running.
Analyze and review — both options
1. Switch to AI mode: open the left sidebar using the arrow at the top-left. Under Workspace settings → Analysis settings → Analysis mode, select AI analysis. You can then collapse the sidebar.
   - The deployed website uses its configured API key; reviewers do not need to enter one.
   - Offline demo uses basic keyword rules and does not provide a full AI assessment.
2. Upload the dataset: expand Dataset · upload or change, select Upload dataset, then upload DynamicIQ_shuffled.csv.
3. Choose a conversation: click Convo 1, Convo 2, etc. in the right-side list.
4. Analyze: click Analyze conversation and wait for the results. Read the transcript, findings and quoted evidence.
5. Add remarks: enter Overall remarks, then tick I have reviewed this conversation and its available evidence.
6. Save: click Save & Done. The conversation is marked Done, and the next unfinished conversation opens. Use Save draft if you want to finish reviewing later.
7. Download results: expand Download saved review and select JSON report or Findings CSV. To download a completed call's report, select that Done conversation first.
