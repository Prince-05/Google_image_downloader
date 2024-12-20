# Google Images Downloader

## Description
This is a Streamlit-based application that allows users to search and download images directly from Google Images. The app scrapes the images based on a user-provided query and saves them locally in a folder called `downloaded_images`. Users can specify the number of images to download and preview the downloaded images within the app.

## Features
- Search for images using a query.
- Specify the number of images to download (1-100).
- Images are saved locally in a folder named `downloaded_images`.
- Preview downloaded images within the Streamlit app.

## Prerequisites
Ensure the following dependencies are installed on your system:

- Python 3.7+
- Streamlit
- Requests
- BeautifulSoup4
- Pillow

## Installation
1. Clone or download this repository.
2. Navigate to the project directory.
3. Install the required dependencies by running:
   ```bash
   pip install streamlit requests beautifulsoup4 pillow
   ```

## Usage
1. Run the Streamlit app:
   ```bash
   streamlit run app.py
   ```

2. Open the local URL provided by Streamlit (e.g., `http://localhost:8501`) in your web browser.

3. Enter the type of images you want to download in the search box.

4. Specify the number of images to download (1-100).

5. Click the **Download** button to begin the process.

6. Once the download is complete, you can preview the downloaded images directly in the app.

## Project Structure
```
.
|-- app.py                # Main application script
|-- downloaded_images/    # Folder where images are saved (created dynamically)
|-- README.md             # Project documentation
```

## How It Works
1. **User Input:** The app takes a search query and number of images as inputs.
2. **Web Scraping:** It uses `requests` and `BeautifulSoup` to scrape image URLs from Google Images.
3. **Image Downloading:** The images are downloaded and saved locally using `Pillow`.
4. **Preview:** The app dynamically displays the downloaded images for user verification.

## Known Issues
- Google Images might block requests if too many images are downloaded in a short period.
- Some images may fail to download due to broken URLs or unsupported formats.

## Future Enhancements
- Add error handling for Google CAPTCHA.
- Support for downloading images in multiple formats (e.g., PNG, JPG).
- Option to choose a custom download directory.

## License
This project is licensed under the MIT License. See the LICENSE file for details.

## Acknowledgments
- [Streamlit](https://streamlit.io/) for providing an easy-to-use framework for building web applications.
- [BeautifulSoup](https://www.crummy.com/software/BeautifulSoup/) for web scraping capabilities.
- [Pillow](https://pillow.readthedocs.io/) for image processing.

