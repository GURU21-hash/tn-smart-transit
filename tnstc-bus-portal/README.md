# Tamil Nadu Bus Portal Demo

A Streamlit website prototype based on the supplied Python code. It includes route search, estimated fares, sample schedules, a seat-selection flow, passenger passes, fare reference tables, and an optional admin/AI area.

## Important

This is an independent prototype, not an official TNSTC, SETC, or Government of Tamil Nadu website. Route schedules, fares, seat inventory, scheme rules, and booking records are sample/simulated data. A displayed boarding pass does not reserve a real seat or authorize travel. Verify travel details with official sources.

## Run on Windows

1. Install Python 3.10 or newer.
2. Double-click `run.bat`. It creates a local virtual environment, installs dependencies, and launches the website.
3. Open the local URL printed in the terminal (usually `http://localhost:8501`).

Manual setup: `py -m venv .venv`, activate `.venv\Scripts\Activate.ps1`, run `python -m pip install -r requirements.txt`, then `streamlit run app.py`.

## Optional admin and Gemini features

Admin access is disabled until you set a password. In PowerShell, set `$env:TN_ADMIN_PASSWORD = "choose-a-strong-local-password"` before starting Streamlit. Gemini features also require the optional `google-genai` Python package and an API key entered in the app. Without it, a built-in demo response is used. Do not deploy this prototype publicly with real credentials or treat generated route content as verified government information.


To enable the optional Gemini integration, install google-genai in the virtual environment and provide an API key in the admin panel. The output is AI-generated and must be checked against trusted official information.
