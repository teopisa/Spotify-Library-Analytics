# Spotify Library Analytics

This is a personal project made with the scope of creating a personal standing of my favorite songs! since I have in my library more than 2000, I'm just starting to select the top 25% using a Tkinter interface.
This project aims to analyze a music dataset from your Spotify library and create a graphical user interface (GUI) to classify songs into two categories: **Top 500** or **Scarti (Discarded)**. The analysis includes examining genre popularity, release date trends, song popularity, and more. A machine learning model using SVM (Support Vector Machine) and data embedding techniques (such as t-SNE and PCA) is used to identify music preferences.

## Table of Contents
- [Installation](#installation)
- [Dataset](#dataset)
- [Analysis](#analysis)
- [GUI Application](#gui-application)
- [Future Improvements](#future-improvements)
- [License](#license)
- [Contributing](#contributing)
- [Acknowledgments](#acknowledgments)
- [Contact](#contact)
- [Final Notes](#final-notes)

## Installation

### Prerequisites
- Python 3.x
- Libraries listed in the `requirements.txt` (to be created)

### Steps to Install
1. Clone the repository:
    ```bash
    git clone https://github.com/your-username/music-data-analysis.git
    cd music-data-analysis
    ```
2. Create and activate a virtual environment (optional but recommended):
    ```bash
    python3 -m venv venv
    source venv/bin/activate
    ```
3. Install the required packages:
    ```bash
    pip install -r requirements.txt
    ```

## Dataset

### Data Description
The dataset used in this project is based on Spotify tracks and their audio features. You can retrieve the data using Spotify's Web API. The dataset contains the following key features:
- Danceability: How suitable a track is for dancing based on tempo, rhythm stability, beat strength, etc.
- Energy: The intensity and activity of a track.
- Valence: The positivity or happiness of a track.
- Tempo: The speed of the track in beats per minute (BPM).
- ... [List other relevant features]

### Fetching the Data
To fetch the data from Spotify, you will need to set up your Spotify Developer account and generate your API keys. Once you have your credentials, follow the instructions in the `data_fetcher.py` file to pull in the data.

Set up your credentials in a `.env` file:

## Analysis

The analysis is conducted in the `analysis.ipynb` Jupyter Notebook. In this notebook, we:

- Clean and preprocess the data.
- Perform exploratory data analysis (EDA) to identify key trends and insights.
- Build machine learning models to classify songs based on their audio features.
- Evaluate model performance using various metrics like accuracy, precision, recall, and F1 score.

### Key Findings

- Tracks with higher energy and tempo tend to be classified as more "danceable."
- Valence shows a moderate correlation with the perceived positivity of a song.

### Visualizations

Several visualizations are provided in the notebook, including:

- Histograms of audio features.
- Pairwise correlations between different features.
- Visual representations of the classification boundaries for machine learning models.

## GUI Application

This project includes a graphical user interface (GUI) that allows users to classify if they are in your top best 500 or not, by showing you the name of the song, age, album and artist and the % of song that you have selected for the moment. For the moment only the index is flagged to filter then

### Running the GUI

To launch the GUI application:

1. Ensure you have installed the required dependencies listed in the `requirements.txt`.
2. Run the GUI script:
    ```bash
    python gui_application.py
    ```

### GUI Features


The GUI is built using the `tkinter` library in Python, providing a simple and intuitive interface.

## Future Improvements

Several areas for future development include:

- **HAve the df of the best 500**: first I need to listen all of them ahah 
- **Music tournament**: Create a better interface, for the final tournament schedule, maybe using Streamlit

## License


## Contributing

Contributions are welcome! If you have suggestions for improvements, feel free to create a pull request or open an issue. Please make sure to follow the project's code of conduct.

## Acknowledgments

- Spotify API for providing song data and audio features.
- Scikit-learn for machine learning models.
- Matplotlib and Seaborn for data visualization.

## Contact

For any questions or suggestions, please feel free to reach out:

- Email: matteo.pisati99@gmail.com
- LinkedIn: https://www.linkedin.com/in/matteo-pisati-b27153225/

## Final Notes

Feel free to explore the code and adapt it to your needs. We hope this project helps you gain insights into your music data and have fun classifying your favorite tracks!
