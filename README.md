# Text-Classification-and-Generation

This project contains multiple python scripts for sourcing song lyric data, classifying songs into genres, and generating songs based on user input.

For the full research paper view Text_Classification_Generation_Report in the repo

Below describes a simple way to get started and use the tool, without using massive amounts of data.

*Install/Download
  - This project utilizes Jupyter Notebooks and various Python Modules please download as needed
 
 Process
1.	Clone Repo

2.	Data Collection 

                a.	Go to https://genius.com/developers and get an API key

                b.	Navigate to the Try_it  folder in the github repo

                c.	Change the SampleArtistGenreData.csv file to artist/genre pairs you are interested in using and save

                d.	Open the GeniusAPIScript.ipynb in the same folder and input your Genius key from step one

                e.	Run the script, this will save a file called LyricsData.csv which will be used in the next steps

3.	Data Cleaning

                a.	Run Lyrics_Parser.ipynb to clean the data and prepare it for NLP Classification this will save a file called cleaned_lyrics.csv which will be used in the next step

4.	Classification
  
                a.	Run Model_Builder.ipynb to build to run some NLP feature engineering and build a Multinomial Logistic Classification Model and a Random Forest Classification Model

                b.	Results from the previous are saved in CSV’s (logistic_metrics.csv and forest_metrics.csv)

5.	Generation
  
                a.	Text Generation is a little bit more complicated and takes longer to train feel free to play around in Text_Generation.ipynb and used the cleaned lyrics data from before 

                b.	Navigate to the Full research report from above in order to learn more about our generative models and results
