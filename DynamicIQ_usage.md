<div align="center">

DynamicIQ
Customer conversations. Clear evidence. Confident reviews.
<p>A quick guide to analyzing transcripts and saving reviewer feedback.</p>

<p>
  <a href="https://imperiumcbc.streamlit.app"><img src="https://img.shields.io/badge/OPEN%20DYNAMICIQ-Launch%20App-187D82?style=for-the-badge&amp;logo=streamlit&amp;logoColor=white" alt="Launch DynamicIQ on Streamlit"></a>
</p>

<p>
  <a href="#start-here">Start here</a> &nbsp; · &nbsp;
  <a href="#review-a-conversation">Review steps</a> &nbsp; · &nbsp;
  <a href="#run-locally">Run locally</a> &nbsp; · &nbsp;
  <a href="#quick-help">Quick help</a>
</p>

</div>

<a id="start-here"></a>
Start here
<table>
<tr>
<td><strong>Recommended: deployed website</strong><br>No installation. Open the app and follow the review steps below.<br><br><a href="https://imperiumcbc.streamlit.app"><strong>Launch DynamicIQ →</strong></a></td>
<td><strong>Alternative: run on your computer</strong><br>Use the provided project files and start Streamlit locally.<br><br><a href="#run-locally"><strong>View local setup →</strong></a></td>
</tr>
</table>

Dataset: Upload DynamicIQ_shuffled.csv, provided with the project submission.
For judges: Use the deployed website. The project team manages its API configuration.

<a id="review-a-conversation"></a>
Review a conversation
These steps work for both the deployed website and the local app.
Step	Action
01	Turn on AI analysis. Open the left sidebar using the top-left arrow. Go to Workspace settings → Analysis settings → Analysis mode and select AI analysis.
02	Upload the dataset. Expand Dataset · upload or change, choose Upload dataset, and upload DynamicIQ_shuffled.csv.
03	Pick a conversation. Click Convo 1, Convo 2, etc. in the right-side list.
04	Analyze. Click Analyze conversation and wait. Read the transcript, findings and quoted evidence.
05	Write your review. Enter Overall remarks, then tick I have reviewed this conversation and its available evidence.
06	Save and continue. Click Save & Done. The call is marked Done, and the next unfinished conversation opens.
07	Export. Select the reviewed conversation, expand Download saved review, and choose JSON report or Findings CSV.


<table>
<tr>
<td><strong>Finish later?</strong><br>Click <strong>Save draft</strong> before switching conversations.</td>
<td><strong>Using Offline demo?</strong><br>It uses basic keyword rules. Select <strong>AI analysis</strong> for model-based assessment.</td>
</tr>
</table>

<a id="run-locally"></a>
Run locally
<details>
<summary><strong>Click to expand local setup instructions</strong></summary>

1. Open the project
Install Python if needed. Open the project folder in VS Code, then select Terminal → New Terminal.
The terminal must be in the folder containing app.py and requirements.txt.
2. Install packages
python -m pip install -r requirements.txt
3. Configure AI mode
Create .env beside app.py. Skip this if already configured.
OPENAI_API_KEY=your_groq_api_key
OPENAI_MODEL=openai/gpt-oss-20b
Replace your_groq_api_key with your actual Groq API key. Keep .env private.
4. Start DynamicIQ
python -m streamlit run app.py
Open localhost:8501, or the Local URL printed in your terminal if different. Keep the terminal running.
Continue with the review steps above.
</details>

<a id="quick-help"></a>
Quick help
<details>
<summary><strong>I cannot find AI mode</strong></summary>

Click the arrow at the top-left to open the sidebar. Under Workspace settings, expand Analysis settings, then select AI analysis.
</details>

<details>
<summary><strong>Save &amp; Done is not completing my review</strong></summary>

Tick I have reviewed this conversation and its available evidence., then press Save & Done again.
</details>

<details>
<summary><strong>I need to edit a completed review</strong></summary>

Select the Done conversation from the right-side list and click Reopen review.
</details>

<details>
<summary><strong>The app shows an API or connection error</strong></summary>

Deployed website: contact the project team.
Local app: check .env and the connection. Restart Streamlit after configuration changes. Quota errors require checking the API account's available quota.
</details>

<div align="center">
<p><strong>Upload · Analyze · Review · Save</strong></p>
<p><a href="https://imperiumcbc.streamlit.app">Open DynamicIQ</a> &nbsp; | &nbsp; <a href="#start-here">Back to top</a></p>
<sub>DynamicIQ · Team IMPERIUM</sub>
</div>
