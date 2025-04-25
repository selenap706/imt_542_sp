# IMT 542 I3

## Overview
This program takes a dataset of books from Goodreads with the various aspects like author, title, Goodreads genres, and publication date. The genre and publication date columns are cleaned up and put into a new dataframe for sorting by year. Then the program can make a wordcloud of the genres for any range of years. This can both numerically and visually display the trends in book genres over the years based on Goodreads data. The current copy of the code analyzes all books published in the year 2000, but it can be adjusted to any other year or range of years between 1980 and 2023. 

## Download Instructions
The repo has a jupyter notebook "imt542_i3.ipynb" that can be opened in Google Colab. Google Colab is linked to the notebook file in this repo, but the file itself can be downloaded or copied into Google Colab. Once Google Colab has the code, also download the dataset "goodreads_top100_from1980to2023_final.csv" in the i3 folder of this repo. This csv file must be manually uploaded into the code using the second cell. 

## Running Instructions
The first code block downloads/imports all the necessary modules and commands for the program. Then the csv dataset must be manually uploaded. Afterwards, the code can be executed as is to visualize the data in a bar graph form or a word cloud. The years analyzed can be changed in this section of the code

''' # Join together a year's worth of book genres into one string, cleaning it up so it's just words and spaces # Rename genre_text_2000 to match the year/years chosen to analyze # One issue I couldn't figure out how to resolve - if a genre tag is more than one word, it gets split up and can't be linked together # Like "Young Adult" becomes "Young" and "Adult" in the eyes of the code genre_text_2000 = " ".join(dfs_by_year[2000]['genres']) genre_text_2000 = genre_text_2000.replace("[", "").replace("]", "").replace("'", "").replace(",", "") print(genre_text_2000)'''
