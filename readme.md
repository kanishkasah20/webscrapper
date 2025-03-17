#### Web Scraping using python and sqlite3 db

This script scrapes paragraphs (<p> tags) from a given website and stores them in an SQLite database. It clears old data before inserting fresh content, ensuring efficiency.

- Setup & Installation
1️⃣ Install dependencies: pip install requests beautifulsoup4

2️⃣ Run the script: python website_scraper.py

3️⃣ Verify stored data in SQLite: sqlite3 scraped_data.db then SELECT * FROM scraped_content LIMIT 5;

- Working:
Fetches website HTML using requests 2. Extracts <p> tags using BeautifulSoup 3. Drops old table and creates a fresh one 4. Saves new paragraphs into SQLite 5. Prints execution time for efficiency check

