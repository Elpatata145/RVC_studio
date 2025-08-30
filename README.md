# Easy Cover Maker

This project provides a Google Colab notebook for creating AI-powered song covers using Retrieval-based Voice Conversion (RVC) models. The notebook automates the entire process, from downloading a song from YouTube to separating the vocals, converting them with your RVC model, and remixing the final track.

## Features

-   **YouTube Song Downloader:** Download any song directly from a YouTube URL.
-   **Vocal Separation:** Uses MDX-Net to separate the instrumental, main vocals, and backing vocals.
-   **RVC v2 Integration:** Convert the vocals using your own RVC v2 model.
-   **Automatic Remixing:** Combines the instrumental with the converted main and backing vocals.
-   **User-Friendly Interface:** A simple Gradio UI to manage the entire process.
-   **Colab Ready:** Designed to run seamlessly in a Google Colab environment.

## How to Use

1.  **Open in Google Colab:**
    -   You can open the `Easy_Cover_Maker.ipynb` notebook directly in Google Colab by uploading the file.

2.  **Run the Notebook Cells:**
    -   Execute the cells in the notebook in order.
    -   **Cell 1: Install Dependencies:** This cell will install all the necessary libraries. It may take a few minutes to complete.
    -   **Cell 2: Import Libraries and Define Helper Functions:** This cell defines all the functions needed for the cover generation process.
    -   **Cell 3: Launch the Gradio Web UI:** This cell will start the Gradio application. Click the public URL (usually ending in `.gradio.live`) to open the UI in a new tab.

3.  **Create Your Cover:**
    -   In the Gradio UI, paste the YouTube URL of the song you want to cover.
    -   Upload your RVC model file (must be a `.pth` file).
    -   Click the "Create Cover" button.
    -   The process will take some time, and you can monitor the progress in the Colab notebook logs.
    -   Once complete, the generated cover song will appear in the audio player on the right. You can listen to it and download it from there.

## Dependencies

This project relies on the following key libraries:

-   `gradio`
-   `yt-dlp`
-   `rvc-python`
-   `audio-separator`
-   `torch`
-   `pydub`
-   `soundfile`

## License

This project is licensed under the MIT License.
