# StatStream
## Status:
Alpha. The batches for this program may only run on Windows 10 due to the different PowerShell launch commands required for various OS versions, that microsoft have bizarly chosen to use for each OS, and may cause endless launch loop on other systems. Also: not progressing past initiation for main loop. Debug messages are implemented, at this stage, and things have been, tried and checked, next move would be to make a test script for, specific code involved or alternate methods of analysis to librosa. Leaving project for a bit, will revisit later.

## Description
`StatStream` is an advanced audio stream analyzer that provides real-time insights into audio stream data. It supports a variety of audio formats and offers detailed analysis including frequency, volume, and tempo. The program also features a dynamic ASCII art console interface for enhanced user interaction.

## Features
- **Support for Multiple Protocols and Formats**: Supports `.m3u`, `.pls`, `.mp3`, `.aac`, `.ogg`, `.flac`, as well as `rtsp` and `mms` protocols.
- **Real-time Frequency and Volume Analysis**: Calculates and displays dominant low, medium, and high frequencies, as well as volume levels categorized as quiet, normal, and loud.
- **Tempo Analysis**: Provides real-time Beats Per Minute (BPM) analysis.
- **Interactive Interface**: Allows users to control speed, input new URLs, or exit the program. Also supports keyboard input for additional controls.
- **Configuration Management**: Persistent speed settings managed through a YAML configuration file.
- **Robust Error Handling**: Comprehensive error handling for issues like stream fetching, timeouts, and more.


## INTERFACE
Output looks like this...

```
     _________ __          __   _________ __                                 
    /   _____//  |______ _/  |_/   _____//  |________   ____ _____    _____  
    \_____  \\   __\__  \\   __\_____  \\   __\_  __ \_/ __ \\__  \  /     \ 
    /        \|  |  / __ \|  | /        \|  |  |  | \/\  ___/ / __ \|  Y Y  \
   /_______  /|__| |____  /__|/_______  /|__|  |__|    \___ \|____  /__|_|  /
           \/           \/            \/                   \/     \/      \/ 


                               Speed: 1/2, Chunk: 21KB

                       Channels: 2, Bits: 16Bit, Rate: 44Khz
                          Quiet [ ], Normal [*], Loud [ ]
                            BPM: 145, BPM Range: 122-166
                       Low: 76Hz, Med: 9646Hz, High: 16078Hz


                               Press any key for Menu

```


## Usage
1. Clone the repository or download the script.
2. Run the script using `python StatStream.py` or click `StatStream.bat`.
3. Enter the URL of the audio stream when prompted.
4. View the real-time analysis of the audio stream's dominant frequencies.
5. Press any key to return to Main Menu.


## Requirements
- Python 3.7 or higher
- Internet connection
- URL linked to an audio stream

## Dependencies
- Python
- Windows (Optional).

## DISCLAIMER
This software is subject to the terms in License.Txt, covering usage, distribution, and modifications. For full details on your rights and obligations, refer to License.Txt.
