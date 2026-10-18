Option 1: Run Online
-------------------
click link > 

https://fakejobpostingdetector.com/

Option 2: Run Locally
-------------------
1. Install Python 3.11

2. Install dependencies:
   pip install -r requirements.txt

3. Run backend:
   uvicorn backend.main:app --reload

4. Open:
   http://127.0.0.1:8000

Note:
If using Render, the server may take a few seconds to wake up.

Database File Location:
The SQLite database file is intentionally stored inside the backend folder because the backend
 application is configured to access the database from this specific location. Moving the database file 
to another directory without updating the backend configuration and file path references will 
cause the website to fail to connect to the database and may prevent the system from functioning properly.


