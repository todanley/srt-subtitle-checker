# SRT Subtitle Checker

A free, in-browser tool for checking and cleaning `.srt` subtitle files. Nothing is uploaded: the file never leaves your browser.

## What it does

- Paste a subtitle or upload an `.srt` file
- Checks cue numbering, timestamp format, end-before-start errors, and overlaps
- Flags lines that exceed a character limit (default 42 for English, 16 for Chinese, Japanese or Korean, both editable)
- Flags cues whose reading speed is above a characters-per-second limit (default 21 English / 9 CJK, both editable)
- Converts Simplified Chinese to Traditional Chinese, or the other way, using an OpenCC character and phrase map bundled in the page ([OpenCC](https://github.com/BYVoid/OpenCC), Apache-2.0)
- Downloads a cleaned `.srt` with sequential numbers and normalized `HH:MM:SS,mmm` timestamps. Optional line wrapping and removal of empty cues
- The interface is available in English and 中文

## How to use

1. Open the tool and paste a subtitle, drop an `.srt` file onto the text box, or click **Load sample with issues**
2. Set line-length and reading-speed limits if your project uses different house rules
3. Choose a Chinese conversion if you need one
4. Review the issue list and click a row to jump to that cue
5. Click **Download fixed .srt**

The download always renumbers cues and normalizes timestamps. Tick **Wrap long lines** if you also want long lines broken to the current limits.

Made by Stanley J, 10+ years at top tech companies. Need custom subtitles, ASO or a small web tool? [Ko-fi](https://ko-fi.com/stanleyj) · [GitHub](https://github.com/todanley) · [Upwork](https://www.upwork.com/freelancers/~011fabd9dccfd03cd8)
