### Automated Sales Data Analysis using AI🤖
An automated pipeline that ingests daily sales report emails, loads the data into a PostgreSQL database, and uses AI to clean and analyze it.

### Overview 
This is a project simulating a daily sales reporting workflow. Sales data is sent via email as CSV attachments, and the pipeline automates the flow from inbox to database, then uses AI for data cleaning and analysis,removing the need for manual data entry or manual cleaning.

### Workflow 
1. Gmail Trigger (n8n) - Watches for incoming sales report emails.
2. Extract from File (n8n) - Parses the CSV attachments. 
3. Insert rows into a table (n8n) - Loads the parsed rows into their respective PostgreSQL tables on Supabase.
4. Data cleaning (Quadratic AI) - Once loaded, Quadratic AI's built-in AI chatbot cleans the data. Cleaning steps are validated using Python.
5. Analysis (Quadratic AI) - AI assisted analysis is performed on the cleaned data.

