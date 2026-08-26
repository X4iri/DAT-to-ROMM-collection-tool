Simple, lightweight web tool to build curated collections in RomM using No-Intro, Redump, or Retool 1G1R DAT/XML files.

No backend, no dependencies, no build steps—just open the HTML file in your browser.


What it does
------------
Instead of picking games one by one to create collections in RomM, drop your .dat or .xml file here. The tool will:

1. Connect to your RomM instance via API.
2. Parse the games, CRC32, and SHA-1 checksums from your DAT file.
3. Match them against your platform library on RomM.
4. Create or update the collection with your chosen name/description and link the games automatically.


How to use
----------
1. Download and open index.html in any browser.
2. Enter your RomM server URL (e.g., http://192.168.1.50:8081) and Bearer API token.
3. Click "Connect & Fetch Platforms".
4. Select your system, set a collection name/description, and drop your .dat or .xml file.
5. Hit "Start Syncing Collection" and watch the progress log.


Notes
-----
- 100% Client-Side: Runs locally in the browser. Your server credentials stay in localStorage and all calls go straight to your own RomM box.
- Flexible Matching: Checks CRC32, SHA-1, and cleaned-up title names so slight tag differences (regions, revisions) don't break matches.
- Currently Name/Description is not importing to RoMM, you will need to input manually.

<img width="875" height="881" alt="image" src="https://github.com/user-attachments/assets/881a0a56-17c5-4847-a644-0ae341a9adbb" />
