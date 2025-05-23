# Disney Theme Park Attractions Web Scraper

This project scrapes the list of Disney theme park attractions from Wikipedia and saves the data into a CSV file for easy analysis or reference.

## Purpose

This project was created as an exercise to experiment with scraping websites with BeautifulSoup and to serve as a personal reference.

## Features

- Fetches the main attractions table from [Wikipedia](https://en.wikipedia.org/wiki/List_of_Disney_theme_park_attractions)
- Parses attraction names, opening years, park locations, and more
- Cleans and structures the data
- Outputs a clean CSV file: `disney_attractions.csv`

## Technologies Used

- Python 3
- [Jupyter Notebook](https://jupyter.org/) for interactive code and data exploration
- [BeautifulSoup](https://www.crummy.com/software/BeautifulSoup/bs4/doc/) for HTML parsing
- `urllib` for HTTP requests

## Usage

1. **Clone the repository**
   ```sh
   git clone https://github.com/joncaudill/disney-attractions-scraper.git
   cd disney-attractions-scraper
   ```

2. **Install dependencies**
   ```sh
   pip install beautifulsoup4
   pip install notebook
   ```

3. **Run the notebook**
   - Make sure you have Jupyter Notebook installed (`pip install notebook`).
   - You can run the notebook in your browser with:
     ```sh
     jupyter notebook
     ```
   - Open `web_scraping_notebook.ipynb` in your browser and run all cells to perform the scraping and save the CSV.
   - **Alternatively:**  
     Jupyter Notebooks can also be run directly inside [Visual Studio Code](https://code.visualstudio.com/) using the [Jupyter extension](https://marketplace.visualstudio.com/items?itemName=ms-toolsai.jupyter).  
     Just open `web_scraping_notebook.ipynb` in VS Code and run the cells interactively.

4. **Output**
   - The script will create `disney_attractions.csv` in the project directory.
   - The CSV contains columns for each table header and rows for each attraction.

## File Structure

- `web_scraping_notebook.ipynb`: Main notebook with all scraping and parsing code.
- `disney_attractions.csv`: Output file with the scraped data.

## Notes

- The scraper is tailored to the current Wikipedia table structure. If the page layout changes, the code may need updates.
- Only the first large attractions table is parsed.
- Commas are removed from data fields to ensure CSV integrity.

