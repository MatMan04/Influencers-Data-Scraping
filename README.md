# Instagram Reels Views Scraper

This project is a Python script that extracts Instagram Reels views for a list of influencer usernames provided in a CSV file. The script utilizes Selenium for web automation and includes stealth features to minimize detection.

## Features
- **Manual login support**: Securely log in to Instagram before scraping.
- **Automated scrolling**: Loads more reels for better data extraction.
- **Randomized delays**: Avoids bot detection by simulating human-like behavior.
- **Data storage**: Saves extracted views to `output.csv`.
- **Progress tracking**: Logs processed usernames in `progress.txt`.

## Requirements
- Python 3.x
- Google Chrome
- Chrome WebDriver
- Required Python packages (install using `pip install -r requirements.txt`):
  ```bash
  selenium
  ````

## Installation
1. **Clone the repository**:
   ```bash
   git clone https://github.com/your-repo-name.git
   cd your-repo-name
   ```
2. **Install dependencies**:
   ```bash
   pip install -r requirements.txt
   ```
3. **Download Chrome WebDriver**:
   - Ensure your Chrome version matches the WebDriver version.
   - Download from [Chrome WebDriver](https://sites.google.com/chromium.org/driver/).
   - Place the driver in the project directory or set it in the system PATH.

## Usage
1. **Prepare your CSV file**:
   - Create a file named `influencers-filters.csv` with usernames in the first column.
2. **Run the script**:
   ```bash
   python script.py
   ```
3. **Manual login**:
   - The script will open Instagram's login page.
   - Log in manually and press Enter to continue.
4. **View results**:
   - Extracted views are saved in `output.csv`.
   - Processed usernames are logged in `progress.txt`.

## Output
- `output.csv`:
  | Username | Views | Minimum Views |
  |----------|-------|--------------|
  | user123  | [100K, 200K, 150K] | 100K |
- `progress.txt`:
  ```
  user123
  user456
  ```

## Notes
- The script uses **random delays** to reduce bot detection risk.
- **Do not close** the browser while the script is running.
- Running this script frequently may lead to **Instagram rate limits**.

## License
This project is licensed under the MIT License.
