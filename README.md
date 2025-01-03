# YouTube Playlist Downloader Script

This script automates the process of downloading YouTube playlists as audio files. It uses `yt-dlp` to fetch and download the playlist while providing a dynamic progress bar and displaying the current song being downloaded.

---

## Features

- Downloads audio files from YouTube playlists.
- Displays a dynamic progress bar indicating download progress.
- Shows the name of the current song being downloaded.
- Supports downloading multiple playlists from a file.
- Hides unnecessary `yt-dlp` output for a cleaner user experience.

---

## Requirements

1. **yt-dlp** 
2. **FFmpeg**

---

## Usage

### Basic Syntax

```bash
./script.sh [-p url] [-f file] [-h]
```

### Options

- `-p url`:
  Download a single playlist from the specified URL.

- `-f file`:
  Download multiple playlists from a file. The file should contain lines in the format:

  ```
  PlaylistName https://playlist_url_here
  ```

- `-h`:
  Display the help message and usage instructions.

---

## Examples

### Download a Single Playlist

To download a playlist from a URL:

```bash
./script.sh -p "https://www.youtube.com/playlist?list=YOUR_PLAYLIST_ID"
```

### Download Multiple Playlists

To download multiple playlists listed in a file:

```bash
./script.sh -f playlists.txt
```

Example `playlists.txt`:

```
MyPlaylist1 https://www.youtube.com/playlist?list=PLAYLIST_ID_1
MyPlaylist2 https://www.youtube.com/playlist?list=PLAYLIST_ID_2
```

---


## Troubleshooting

- **yt-dlp Command Not Found**:
  Ensure `yt-dlp` is installed and available in your `PATH`.

- **FFmpeg Issues**:
  If audio extraction fails, verify that `ffmpeg` is installed and working correctly.

- **Permission Errors**:
  Ensure you have write permissions for the directory where the script is executed.

---

## License

This script is provided "as is" without warranty of any kind. You are free to modify and distribute it as needed.

---

## Acknowledgments

This script leverages the powerful capabilities of `yt-dlp` and `ffmpeg` to provide a seamless playlist downloading experience.

