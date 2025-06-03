# Spotify-Project-
Attempt at unsupervised learning project: clustering 100k+ Spotify tracks using audio features.
# Spotify Genre Clustering 

Unsupervised learning project exploring whether meaningful genre groupings could emerge from audio-only features and (a very simple algorithm in) K-Means CLustering, with no genre labels used during clustering.

---

##  What I Did
- Cleaned and explored 100k+ real Spotify tracks
- Scaled features like danceability, energy, tempo, valence, etc.
- Applied KMeans clustering and visualized with PCA
- Analyzed cluster contents by genre to interpret the results
- Evaluated structure using silhouette score and domain insight

---

##  Project Summary

This clustering certainly isn't 100% perfect, but there are several eye-catching groupings:

- **Cluster 1** has a strong Brazilian theme — Pagode, Sertanejo, Samba, MPB, Forró, and Brazil all show up. RNB and Spanish are also present, which fits, considering musical influences. However, Heavy Metal and Sleep also appear, which is rather odd and amusing.

- **Cluster 2** is full of Ambient, Sleep, New-Age, Piano, Opera, and Study. It also includes Anime, Disney, and Jazz, making this one of the most coherent clusters.

- **Cluster 3** contains House, EDM, Dance, Hip-Hop, Reggaeton, K-pop, Salsa, and Dubstep. A very energetic mix — lots of rhythm-heavy genres.

- **Cluster 4** includes Jazz, Folk, Acoustic, Country, Singer-Songwriter, and Bluegrass. A strong grouping of organic and melodic genres with shared history.

- **Cluster 5** features Punk, Rock, Grunge, J-Rock, J-Pop, Kids, Party, Power-Pop, and Ska. Chaotic, but very youth-focused and upbeat.

- **Cluster 6** is kind of aggressive and emotional — Comedy, Emo, Sad, Hardcore, Funk, Grindcore, and Metalcore. A peculiar, possibly the most inconsistent cluster.

- **Cluster 7** is packed with electronic genres — Minimal Techno, Detroit Techno, Techno, Trance, IDM, Trip-Hop, Drum-and-Bass. Also includes Black Metal, Death Metal, and Industrial, which is a bit odd but somewhat makes sense sonically (unlike Sleep and Heavy Metal being in Cluster 1).

---

##  Metrics

- **Silhouette score:** ~0.15  
  ↪ Low, indicating poor geometric separation.  
  ↪ But genre groupings still emerged — showing that even simple clustering can surface real structure.

---

##  Takeaway

This began as a light experiment out of curiosity, but turned into a thoughtful unsupervised exploration.  
Despite a low silhouette score, many clusters showed surprising genre consistency — and the project revealed both the strengths and limitations of using raw audio features for genre grouping.

---

##  Next Steps
- Try HDBSCAN or GMM
- Use deep embeddings or listener-based features
- Explore recommender systems based on clusters

---
**FINAL CONCLUSIONS**

Despite a relatively low silhouette score of 0.15, the clustering results reveal meaningful structure in the audio feature space. Several clusters group together genres with shared musical characteristics — such as:

    Techno subgenres and house styles

    Ambient, study, and sleep tracks

    Folk, jazz, and acoustic genres

    Overlaps between Latin, Spanish, and RnB

This indicates that even without explicit genre labels, a simple algorithm like KMeans was able to capture some degree of stylistic similarities in the data. However, the presence of genres like "Kids" or "Sleep" in multiple, unrelated clusters highlights the limitations of using purely audio-based features for genre classification.

Ultimately, the 0.15 silhouette score reflects the complexity and fuzziness of real-world music genre boundaries. While the clusters aren’t cleanly separable, the model does uncover some valuable patterns — suggesting that unsupervised learning, when combined with domain insight, can still yield practically useful groupings.


📎 *Notebook included in this repo.*
