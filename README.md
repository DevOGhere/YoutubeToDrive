# YouTube Video Segment Downloader and SNR Calculator

This project allows you to download specific segments of YouTube videos, calculate the Signal-to-Noise Ratio (SNR) for the audio, and determine the sampling rate. It uses `yt-dlp` for downloading videos and `ffmpeg` for trimming and converting audio. The results are saved in a CSV file.

## Features

- 🎥 Downloads specified segments of YouTube videos.
- ✂️ Trims videos to the specified timeframe.
- 🔊 Converts video to audio and calculates the SNR.
- 📈 Extracts and stores the sampling rate of the audio.
- 📄 Saves the results in a CSV file.

## Requirements

- 🐍 Python 3.x
- 📥 `yt-dlp` (YouTube video downloader)
- 🎛️ `ffmpeg` (A complete, cross-platform solution to record, convert and stream audio and video)
- 🐼 `pandas` (Data analysis and manipulation library)
- 🔢 `numpy` (Fundamental package for scientific computing with Python)
- 🔬 `scipy` (Library used for scientific and technical computing)

## Installation

1. Install Python from [python.org](https://www.python.org/).
2. Install `yt-dlp`:
    ```bash
    pip install yt-dlp
    ```
3. Install `ffmpeg`:
    - Windows: Download from [ffmpeg.org](https://ffmpeg.org/download.html) and add to PATH.
    - macOS: Install via Homebrew:
      ```bash
      brew install ffmpeg
      ```
    - Linux: Install via package manager:
      ```bash
      sudo apt-get install ffmpeg
      ```
4. Install other required Python libraries:
    ```bash
    pip install pandas numpy scipy
    ```

## Usage

1. Prepare a CSV file with YouTube video links and timestamps. The CSV file should have the following format:

    | Video link | Timestamp   |
    |------------|-------------|
    | link1      | 00:10 - 00:20 |
    | link2      | 01:00 - 02:00 |
    
    Ensure the CSV file is in the same directory as the script.

2. Run the script:

## Output

The results are saved in a CSV file named `results.csv` in the specified output directory. The CSV file contains the following columns:

- `Video Link`: The YouTube video link.
- `Timestamp`: The specified timestamp range.
- `Sampling Rate (Hz)`: The sampling rate of the audio.
- `SNR (dB)`: The Signal-to-Noise Ratio of the audio.

## Future Work

This script can be further developed into a web application, providing a user-friendly interface to input video links and timestamps and receive the processed results. The web app can leverage Flask or Django in Python to handle user requests and perform background processing.

## License

This project is open-source and available under the [MIT License](LICENSE).

## Acknowledgements

- [yt-dlp](https://github.com/yt-dlp/yt-dlp)
- [ffmpeg](https://ffmpeg.org/)
- [pandas](https://pandas.pydata.org/)
- [numpy](https://numpy.org/)
- [scipy](https://www.scipy.org/)

Feel free to contribute to this project or report any issues. Happy coding!
