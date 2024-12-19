# YouTube Video Summarizer with Streamlit and Google Gemini

This Streamlit app extracts the transcript of a YouTube video, summarizes it using Google Gemini AI, and provides detailed notes. The summarized points aim to capture key ideas from the video in a concise, easy-to-read format.

## Features
- **Transcript Extraction**: Retrieves transcript data directly from YouTube.
- **AI-Powered Summarization**: Uses Google Gemini Pro to generate a summary.
- **Concise Output**: Presents a 250-word summary with key points.

## Installation

1. **Clone the Repository**:
   ```bash
   git clone https://github.com/your-repo-name/youtube-summarizer.git
   cd youtube-summarizer
2. **Install Dependencies**:
   ```bash
   pip install -r requirements.txt
3. **Set up API Keys**:
   - Obtain an API key from [Google Cloud](https://cloud.google.com/) for `google.generativeai`.
   - Replace `your-google-api-key` in `main.py` with your API key.

4. **Run the App**:
   ```bash
   streamlit run main.py
## Usage

1. **Enter YouTube Video Link**:
   - **Paste the URL of the YouTube video you want to summarize into the app.**
2. **Generate Summary**:
   - **Click Get Detailed Notes to extract the transcript and generate a summary.**
## Code Overview

- **extract_transcript_details**: Fetches transcript data using YouTubeTranscriptApi.
- **generate_gemini_content**: Uses google.generativeai to generate a summary based on a specified prompt.
- **Streamlit UI**: Displays the YouTube video thumbnail and the generated summary.
