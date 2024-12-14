# Social Links vs. Language Barriers: Decoding the Global Spread of Streaming Content

This repository contains dataset and codes from *Social Links vs. Language Barriers: Decoding the Global Spread of Streaming Content*. 

---

## Repository Structure

### Files and Notebooks

1. **`dataset.csv`**  
   The aggregated dataset used in this analysis. It includes details about user and content locations of 10 countries,  social connection from Facebook, language similarity metrics, and interaction data from three platforms: YouTube, Spotify, Netflix.

2. **`fig1.ipynb`**  
   A Jupyter Notebook that generates heatmaps intricating the numbers of shared trending content between countries.
   
3. **`fig2.ipynb`**  
   A Jupyter Notebook that generates scatterplot comparing the numbers of co-trending contents between countries by platform.
  
4. **`fig3.ipynb`**  
   A Jupyter Notebook that generates scatterplot of the correlation between the number of shared trending contents and two proxies of social similarity.

5. **`heatmap_matrix.pkl`**  
   A precomputed heatmap matrix that transforms the dataset (`dataset.csv`) into a format suitable for visualizing language and engagement patterns. This file is used in generating heatmaps within the analysis.


---

## Dataset Description

The dataset (`dataset.csv`) contains the following columns:

- **user_loc**: User's location (ISO Alpha-2 country code).
- **fr_loc**: Content's origin location (ISO Alpha-2 country code).
- **YouTube**: Numbers of common YouTube Trending content
- **ISO_1**, **ISO_2**: ISO 639-1 language codes for user and content locations, respectively.
- **LangName_1**, **LangName_2**: Full names of the primary languages in user and content locations.
- **LangSimilarity**: Language similarity score based on linguistic metrics.
- **Robustness**: Qualitative measure of the language similarity score's reliability. For details, please visit [UKC project](http://ukc.disi.unitn.it/index.php/lexsim/).
- **NewSimilarity**: Refined similarity score with language usage proportion.
- **fb_sci**: [Facebook Social Connected Index Score](https://dataforgood.facebook.com/dfg/tools/social-connectedness-index)
- **Spotify**: Number of shared songs in charts. You can find data at [Spotify Charts](https://charts.spotify.com/home).
- **Netflix Film**: Number of shared Netflix film. You can find data at [Netflix Tudum](https://www.netflix.com/tudum/top10)
- **Netflix TV**: Netflix TV show view counts. You can find data at [Netflix Tudum](https://www.netflix.com/tudum/top10)

---
---

## Citation

If you use this repository or its contents in your research, please cite the following paper:

> **"Decoding the Global Spread of Streaming Content: Social Links vs. Language Barriers"**  
> Available at: [https://arxiv.org/abs/2402.19329](https://arxiv.org/abs/2402.19329)

