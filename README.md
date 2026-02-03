# Webpage HTML Fetcher Utility

A robust Python command-line application that retrieves and displays the raw HTML source code of a specified website. This project focuses on professional error handling and network request management.

## 📌 Assignment Description
This utility was developed to demonstrate the practical application of the `requests` library in Python. The script securely connects to a remote server, fetches webpage data, and implements a multi-layer exception handling system to manage common networking failures.

### Logic Flow & Error Handling
The script is designed with a "Safety First" approach:



1. **Timeout Control:** Limits the wait time to 10 seconds to avoid system hangs.
2. **Schema Validation:** Detects if the user forgot `http://` or `https://`.
3. **Status Verification:** Uses `raise_for_status()` to catch HTTP errors like 404 (Not Found) or 503 (Service Unavailable).
4. **Connectivity Checks:** Provides specific feedback if the local internet is disconnected.

## 🛠️ Prerequisites

Ensure you have Python 3.x installed. You will also need the `requests` library.

```bash
pip install requests
