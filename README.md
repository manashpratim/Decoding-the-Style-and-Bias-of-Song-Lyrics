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
lyrics by scraping through the user-generated content on multiple websites such as MetroLyrics (www.metrolyrics.com) and LyricsMode 
(www.lyricsmode.com). The BB dataset contains top 100 songs for each year (1965 to 2015) from the Billboard Hot 100 list
(www.billboard.com/charts/hot-100). We consider these 5100 songs as popular songs. The original million song dataset only provides
audio features and song metadata [2]. It does not provide song lyrics. Out of all songs listed in the original million song dataset,
we could obtain lyrics only for 451,045 songs. We ensured that our BB and MSD datasets had no songs in common. Thus total songs
in our analysis are around half a million. We had to do extensive data cleaning and preprocessing to use the scraped lyrics.
We can not publicly distribute our datasets as it might infringe copyright of the artists. 

# Instructions
The notebooks Lyrics Analysis and Lyrics Analysis II contain the codes for the style analyis of songs. Lyrics Analysis contains codes for analysis of swear words content, length of songs etc. Lyrics Analysis II contains codes for the readability tests and repetitiveness. The notebook word cloud contains code to create the word clouds. Word Rank notebook contains the code for the word rank comparison. The WEAT notebook contains the code for the Word Embedding Association Test[3] to measure bias.

# Conclusion
We have analyzed over half a million lyrics to understand the style and prevalent biases. As compared to other songs, we have observed
that popular songs have several distinguishing characteristics that can be expressed in terms of the style of lyrics. Lyrics can capture
human biases quite accurately. This work can be extended further by investigating music genre-specific style and biases.

# References
[1] MP Barman, A Awekar and S Kothari "Decoding the Style and Bias of Song Lyrics"- arXiv preprint arXiv:1901.05227, 2019.

[2] T. Bertin-Mahieux, D. P. Ellis, B. Whitman, and P. Lamere. 2011. The million song Dataset. In Proceedings of the 12th International Conference on Music Information Retrieval (ISMIR 2011).

[3] Aylin Caliskan, Joanna J. Bryson, and Arvind Narayanan. 2017. Semantics derived automatically from language corpora contain human-like biases. Science 356 (2017), 183–186.

