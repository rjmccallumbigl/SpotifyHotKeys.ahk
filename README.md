# SpotifyHotKeys.ahk

Shortcuts to add currently playing songs to particular playlists or seek forward/backwards using media button keys on my keyboard. Tested with the [Spotify Windows App](https://www.microsoft.com/en-us/p/spotify-music-and-podcasts/9ncbcszsjrsb?silentauth=1&wa=wsignin1.0&activetab=pivot:overviewtab) version.

## Instructions
1. Download https://github.com/CloakerSmoker/Spotify.ahk
2. Place this script in the same folder
3. In Windows settings, set .mp3 association to Spotify Windows App (Spotify.exe) by right clicking an mp3 file, selecting Open With -> Choose another app -> Look for another app on this PC -> find Spotify.exe. If you don't do this, Windows might open Windows Media Player or another media app whenever you press a media key. More info: https://community.spotify.com/t5/Desktop-Windows/Keyboard-media-launch-button/td-p/1736288
4. If you're using the Windows app, run this in PowerShell (as admin) to get exact location of Spotify.exe: "$((ls "C:\Program Files\WindowsApps\" | Where-Object { $_ -like "*spotify*"})[0].FullName)\Spotify.exe"
5. If Spotify updated, the folder changed and Windows Media Player or another app may open when you press your media keys. Redo the above two steps.
6. If you get an error message attempting to set Spotify to open mp3s, open Task Manager with CTRL + Shift + Esc, click File -> Open New Task, check "Create this task with administrative privileges", type Explorer, and press enter. Try it from there. Then close Explorer and see if the media keys work.
