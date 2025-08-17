# Spotify-Songs-Analysis
Two things that intrigue me the most are Music and Data. Taking inspiration from that, I chose to build a project analyzing my Spotify Liked Songs.

Using Spotify’s Spotipy API and the current_user_saved_tracks endpoint, I was able to access my saved/liked songs, a total of 2,709 tracks. Before accessing any endpoint, I had to authorize myself to grant the required permissions needed to pull my own data.

Unfortunately, Spotify has restricted access to several endpoints, including Get Audio Analysis and Get Audio Features, which provide audio details such as acousticness, danceability, energy, valence, and speechiness. This is likely because it could allow others to build proprietary recommendation models using Spotify’s data.
List of all deprecated endpoints as of November 2024: Spotify API Changes

My project includes various attributes including (but not limited to):
- Song Name
- Song ID
- Song Popularity
- Release Date
- Artist ID
- Artist Name
- Artist Popularity
- Artist Followers
- Artist Genre

I did a deep dive to understand my music taste, favorite artists, top genres, and more. 


# Breakdown of songs by era
<br> <img width="480" height="480" alt="output_52_0" src="https://github.com/user-attachments/assets/9414430e-bc77-43b1-a2eb-16fdba768973" />

Of my 2,709 songs, ~16% are from the 90s, with the oldest being from 1952: La Vie en Rose – Single Version by Louis Armstrong, who has around 3M followers on Spotify. Many of these songs come from the late 90s, including Bollywood, classic rock, Hindi pop, rock, ghazals, and more.

<br> <img width="1000" height="1000" alt="1952 to 2025 Song Count" src="https://github.com/user-attachments/assets/94c51d1c-b123-492f-ab76-4045b854bbf5" />

With 59 songs from 2025, Ushuaia by Chestford is a highly underrated track and a must-listen if you’re into upbeat dance and electronic music. And just like every teenager who grew up in India in the early 2000s, my list would be incomplete without popular hits from Himesh Reshammiya, Akon, KK, Shankar–Ehsaan–Loy, Vishal–Shekhar, Eminem, and many others. It looks like my taste in music leans more towards songs released from 2011 onwards, while still including plenty of classics.

## Analyzing Listening Habits: Timeline view of the # of songs added/saved since April 2020

<br> <img width="1000" height="1000" alt="Timeline of Saved Songs" src="https://github.com/user-attachments/assets/da6936f9-8589-4a9b-a35b-3c5ffd779260" />

For a period of 4 months from January 2024 to April 2024, I was pretty consistent in adding ~50 new songs a month and similar patterns of consistency can be seen across other areas of the graph. However, I was on a listening high in January 2023 (122 songs) and April 2025 (147 songs added) unlike when I started using Spotify back in April 2020 where I averaged around 1 song a month. My introduction to some indie pop and rock bands such as The Postal Service, Spiritualized, Creedence Clearwater Revival, Eagles, Neil Young, and others came pretty late in 2025.

# Artists
The top 15 artists in my library span a wide range of styles, with Deborah De Luca leading at 57 songs, followed by Pritam (38), and then Kishore Kumar, Lane 8, and Post Malone covering everything from Bollywood classics to rock, pop, techno, and indie pop and others
<br> <img width="300" height="300" alt="image" src="https://github.com/user-attachments/assets/eb963401-2010-4ca1-8114-dc0aac8487e7" />

# Genres
Although Spotify does not collect genre data for each individual song, it does assign genres at the artist level using metadata from labels, algorithmic audio analysis, co-listening patterns, and more. Based on that, I listened to 286 unique genres, with Bollywood at the top followed by techno, Hindi pop, desi, acid techno, and hard techno. On the other hand, some of my least listened-to genres include Indonesian Indie, Heavy Metal, Afrobeat, and 3-step. The data isn’t fully representative since not all artists had genre information, but it still provides a useful picture of my listening habits.

<br> <img width="300" height="300" alt="image" src="https://github.com/user-attachments/assets/8ff45399-67c2-4442-9683-2b88ad2c288b" />

# Song and Artist Popularity 
Spotify also provides song popularity scores ranging from 0-100, based on signals like total streams, recency of plays, engagement, and skip rates. Most of my songs range between 32–65, with only 9 songs above 90 and 322 songs below 10, suggesting that I often explore underrated or niche tracks, not just mainstream hits.

<br> <img width="544" height="420" alt="image" src="https://github.com/user-attachments/assets/21d668c5-94cf-4e8e-8fec-4feb60af31b4" />

For my analysis, I defined a “Popular” song as popularity ≥50, otherwise “Not Popular.” The split came out almost even: 51% Popular vs. 49% Not Popular. Some famous songs that intuitively feel popular, such as Aa Chal Ke Tujhe and Zindagi Ka Safar by Kishore Kumar, scored below 50. Other notable examples include Pulaski at Night by Andrew Bird, Runaway by AURORA, and Don’t Look Now by Creedence Clearwater Revival.
On average, my songs score around 46.7 on the Song popularity scale. Similarly, when looking at artist followers and artist popularity, some of my artists have huge fan bases while others are relatively unknown, confirming that my taste is a blend of global stars and underground artists.

<br> <img width="1789" height="590" alt="output_141_0" src="https://github.com/user-attachments/assets/010af0a6-9a3b-4f61-a325-f2a2be55ac5e" />

The graph above shows the breakdown of count of Popular VS Not Popular Songs in each year from 1952-2025. Starting 2017, the grpah changes with more Not-Popular Songs than Popular songs.  


# Artists with 10+ Saved Songs

<br><img width="1990" height="989" alt="output_158_1" src="https://github.com/user-attachments/assets/3f6f3a03-e435-44b1-87e9-ea9f71fdeb0d" />

**Mean Song Popularity of an Artist = Average Popularity of all Songs Saved per Artist**. Interestingly, almost all the techno artists (Deborah de Luca, Charlotte de Witte, Ballarak, WhoMadeWho, Hozho, T78, Worakls) had much lower average popularity scores. Not sure why techno/EDM doesn’t flourish on Spotify and  maybe just a quirk of my dataset. Eminem, on the other hand, has the most popular songs on average in my library. Eagles, Creedence Clearwater Revival, Fleetwood Mac, and other rock bands are close behind, showing that artists within the same genre often have similar average popularity.

Overall, this project gave me a new way to look at my own listening habits and appreciate the blend of mainstream hits, classics, and underrated gems in my library. It was a fun way to bring together my love for music and data, and I look forward to exploring even more patterns in the future.

