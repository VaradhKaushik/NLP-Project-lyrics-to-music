# NLP Project: Lyrics to Music Generation

## Project Overview
This repository explores the innovative intersection of Natural Language Processing (NLP) and music generation. By analyzing lyrical content through advanced NLP techniques, this project generates music that mirrors the emotional and thematic subtleties of the input lyrics using the MusicGen model.

## Technical Features
- **APIs and Data Collection**: Utilizes the Genius API for lyrics and the Spotify API for song metadata, enriching the dataset with diverse musical characteristics.
- **Sentiment Analysis and Keyword Extraction**: Employs the TextBlob library for sentiment analysis and the RAKE algorithm for extracting keywords, enhancing the understanding of lyrical content.
- **Topic Modeling**: Implements Latent Dirichlet Allocation (LDA) using the Gensim library to discover latent themes within lyrics, which inform the music generation process.

## System Architecture
1. **Data Preprocessing**: Parses MIDI files from the Lakh MIDI Dataset to align musical data with extracted lyrical themes.
2. **Prompt Construction**: Combines sentiment, keywords, Spotify metadata, and topics into structured prompts that guide the music generation.
3. **Music Generation**: Uses Facebook's MusicGen models conditioned on constructed prompts to produce music that corresponds with the lyrical analysis.

## Setup and Execution
1. **Installation**:
   ```bash
   git clone https://github.com/VaradhKaushik/NLP-Project-lyrics-to-music.git
   cd NLP-Project-lyrics-to-music
   pip install -r requirements.txt
   ```
2. **Running the Notebooks**:
   Start Jupyter Notebook and run the provided notebooks to process data and generate music:
   ```bash
   jupyter notebook musicGen_inference.ipynb
   ```

## Dataset
The project harnesses approximately 1,830 songs from diverse genres, ensuring a comprehensive analysis and generation process. This subset was selected for its rich metadata and clear MIDI structuring.

## Future Directions
- **Model Fine-Tuning**: Enhance MusicGen's adaptation to lyrical prompts for improved fidelity in music generation.
- **Expand Genre Coverage**: Include a wider array of genres to study genre-specific music generation.

## Contributions
We encourage contributions to refine algorithms, expand the dataset, and improve documentation.

## License
Distributed under the MIT License.
