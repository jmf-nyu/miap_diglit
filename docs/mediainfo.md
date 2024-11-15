# mediainfo Command

## Summary 
`mediainfo` is a command line utility used to display information about audio/video files. From this command you can find general information on the title/author of the media file, date of creation, codec, aspect ratio, bitrate, channels, language. 'mediainfo' allows users to view this information in various formats and export it in txt, csv or html. 

## How to use it 
To use 'mediainfo' you would enter 'mediainfo' followed by the full name of the file in your server that you are looking for information on. For example, if you were looking for information on a video file called "Mi'at Wajeh Li Yawm Wahed (1972).mkv:" you would type 
        $ mediainfo Mi'at Wajeh Li Yawm Wahed (1972).mkv 
into your command line. 

## Supported File Types
'mediainfo' supports MKV, OGM, AVI, DivX, WMV, QuickTime, Real, MPEG-1, MPEG-2, MPEG-4, DVD (VOB), DivX, XviD, MSMPEG4, ASP, H.264, AVC, OGG, MP3, WAV, RA, AC3, DTS, AAC, M4A, AU, AIFF, SRT, SSA, ASS, SAMI file types. 

## Examples of specific ways to use mediainfo
Display aspect ratio
        $ mediainfo --Inform="Video;%DisplayAspectRatio%" Mi'at Wajeh Li Yawm Wahed (1972).mkv 
        $ mediainfo --Inform="Video;file://Video.txt" Mi'at Wajeh Li Yawm Wahed (1972).mkv 

Display aspect ratio and audio format
        $mediainfo --Inform="file://Text.txt Mi'at Wajeh Li Yawm Wahed (1972).mkv

        If Text.txt contains:

        - "Video;%DisplayAspectRatio%"
        Then the display aspect ratio is printed out. 

        -"Audio;%Format%"
        Then the audio format is printed out.
