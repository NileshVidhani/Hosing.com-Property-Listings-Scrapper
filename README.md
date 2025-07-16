# 🏠 Housing.com Rental Property Scraper

This project is a web scraping application designed to extract **rental property listings** from [Housing.com](https://housing.com). Users can enter any **Indian city** as input, and the scraper fetches property details such as title, price, location, and property link. The data is saved into a structured **CSV file** in the local directory.

---

## 🎯 Objectives

- **Automate Property Data Collection** – Efficiently scrape rental listings from Housing.com.
- **City-Based Scraping** – Let users input any city name for a dynamic search.
- **Data Storage** – Save the extracted property data in a clean, structured CSV file.
- **User-Friendly Execution** – Run the script easily inside a Jupyter Notebook with minimal setup.

---

## 🔧 Technologies & Libraries Used

- **Python 3.x**
- **Selenium** – For automating browser interactions and rendering JavaScript.
- **BeautifulSoup4** – For parsing HTML and extracting listing data.
- **Pandas** – For storing and exporting data in CSV format.
- **ChromeDriver** – Required to render Housing.com pages with Selenium.

---

## 📂 Features & Workflow

1. User provides the **city name** (e.g., `Mumbai`, `Pune`, `Bangalore`).
2. The scraper builds the appropriate Housing.com rent URL.
3. Selenium opens the page, scrolls down to load listings, and collects:
   - 🏠 **Title**
   - 💰 **Price**
   - 📍 **Location**
   - 🔗 **Link to property**
4. Data is extracted using BeautifulSoup.
5. Final output is saved as: `housing_<city>_rent.csv`.

---

## 🚀 How to Run the Notebook

1. 🔽 **Download ChromeDriver**
   - Find your browser version at `chrome://settings/help`
   - Download matching version from: [https://chromedriver.chromium.org/downloads](https://chromedriver.chromium.org/downloads)
   - Place `chromedriver.exe` in your notebook folder or system PATH

2. ✅ **Install Required Packages**
   ```bash
   pip install selenium beautifulsoup4 pandas

3. ▶️ Run the Notebook Cells
Enter the city when prompted
Wait for data extraction to complete
Find your file: housing_<city>_rent.csv

4. 📌 Example Output (CSV Format)
Title	  Price	  Location	  Link
1 BHK Apartment in Andheri	  ₹25,000	  Andheri, Mumbai	  https://housing.com/rent/property-details/
2 BHK Flat in Kharadi	  ₹18,000	  Kharadi, Pune	  https://housing.com/rent/property-details/


⚠️ Disclaimer
This project is intended strictly for educational purposes.
Scraping Housing.com or any commercial website without permission may violate their terms of service.
Always use scrapers responsibly and limit your requests to avoid overwhelming their servers.
