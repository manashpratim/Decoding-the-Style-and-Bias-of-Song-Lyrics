# Decoding-the-Style-and-Bias-of-Song-Lyrics
The central idea of this project is to gain a deeper understanding of song lyrics computationally. We focus on two aspects: style and biases 
of song lyrics. All prior works to understand these two aspects are limited to manual analysis of a small corpus of song lyrics. In 
contrast, we analyzed more than half a million songs spread over five decades. We characterize the lyrics style in terms of vocabulary, 
length, repetitiveness, speed, and readability. We have observed that the style of popular songs significantly differs from other songs.
We have used distributed representation methods and WEAT test to measure various gender and racial biases in the song lyrics. We have 
observed that biases in song lyrics correlate with prior results on human subjects. This correlation indicates that song lyrics reflect 
the biases that exist in society. Increasing consumption of music and the effect of lyrics on human emotions makes this analysis important.
This is the official codebase of the paper[1].

# Dependencies
1) Python3
2) NLTK
3) Gensim
4) fastText

# Datasets
For style analysis, we created two datasets: Billboard (BB) and Million Song Dataset (MSD). For both the datasets, we obtained the song 
lyrics by scraping through the user-generated content on multiple websites such as MetroLyrics (www.metrolyrics.com)and LyricsMode 
(www.lyricsmode.com). The BB dataset contains top 100 songs for each year (1965 to 2015) from the Billboard Hot 100 list
(www.billboard.com/charts/hot-100). We consider these 5100 songs as popular songs. The original million song dataset only provides
audio features and song metadata [2]. It does not provide song lyrics. Out of all songs listed in the original million song dataset,
we could obtain lyrics only for 451,045 songs. We ensured that our BB and MSD datasets had no songs in common. Thus total songs
in our analysis are around half a million. We had to do extensive data cleaning and preprocessing to use the scraped lyrics.
We can not publicly distribute our datasets as it might infringe copyright of the artists. However, our datasets are available upon request.

# Conclusion
We have analyzed over half a million lyrics to understand the style and prevalent biases. As compared to other songs, we have observed
that popular songs have several distinguishing characteristics that can be expressed in terms of the style of lyrics. Lyrics can capture
human biases quite accurately. This work can be extended further by investigating music genre-specific style and biases.
