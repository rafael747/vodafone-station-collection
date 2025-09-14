# Bruno Collection for Vodafone Station API

[<img src="https://fetch.usebruno.com/button.svg" alt="Fetch in Bruno" style="width: 130px; height: 30px;" width="128" height="32">](https://fetch.usebruno.com?url=git%40github.com%3Arafael747%2Fvodafone-station-collection.git "target=_blank rel=noopener noreferrer")

## Description

A collection of API operations for Vodafone Station Router.

**Tested with:** CGA6444VF model (Technicolor) - Firmware version 19.3B80-3.5.13

## Setup

1. Create a `.env` file with your router information (check `.env.example` for reference)
2. Open the collection in Bruno
3. Run the **Login** request - it performs the login operation and populates the `PHPSESSID` variable for subsequent requests
4. Run **Refresh** to obtain a new CSRF token (required for POST operations)
   - Note: POST requests will automatically run Refresh (see the pre-script)
5. You're now ready to execute the other requests

---

> **Note:** The login operation was extracted from [vodafone-station-cli](https://github.com/totev/vodafone-station-cli) and uses `crypto-js`, which is available in Bruno.
