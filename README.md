# MP3Z-Player

Download .APK file for Andoid app 
I dont know how to make a nice download button, click the view raw button to download and then 
transfer to your phone and open it with a package installer (it should pop up automatically)

Download .AIA file if you want to build from where I stopped (for use with MIT App Inventor)

An MP3 player app made by ZM with the MIT app Inventor only for Android 
When I was making this app the main struggle I had was setting up how to route through the filing systems on Android,
specifically on my own android and I'm ignorant if other android os's on other phones have different route file systems
so I have no idea if they will work or not, but I do know that this will not work on IOS as I know it has a diffrent
route filing system, though, I'm sure since I'm giving you the code right here and you can easily ask a chatbot how
the IOS filing system works, that you'd need only change 5 blocks to get it to work :)


What I'm talking about here is when you pick a folder you are using the storage access framework, the android will
return a content URI, which is an address specific to android.
But we want a normal file path (so the filetools extension can use it), so imagine we have :
content://com.android.externalstorage.documents/tree/primary%3AMusic
We just want the name of the folder [Music] all the way at the end there, and then replace the rest with a normal file 
path that filetools can use which would be an address like /storage/emulated/0/Music.
This is kind of like getting the global file path on windows (C:Users/***...).
Anyway yeah thats really all it is, you could easily change this if you want to, I'll link my MIT app invetor link
if you want to play around with it and make it work on your own phone or even make it better than I could,
which I have no doubt you could.

------------------------------------------------------- IMPORTANT-----------------------------------------------------

I hope I pointed it out in the video but to get the app to actually play the songs, the folder with all the songs 
needs to be in the Main Storage folder, again this is linked with getting the /storage/emulated/0/Music route.
If I coded it up correctly the name of your folder can be whatever you choose, and you can have as many as you want
there to be, as long as it situated in this directory. 
-->  I did this in case you want to have specific playlists to choose from, I see people like this feature so yurwelcom
If another folder with songs is inside this "music" folder, the app will still work but the songs inside this second 
music folder will still not be able to be played for the same addressing reason.

I do not know why but it seems only MP3 files are able to be played by the android audio player, if they are not mp3 
files they will not show up. (This may be a simple oversight on my part, if so I'm sorry)

But the most important part (seeing as your here), I hope you find this app useful and above all more conveniant than
the other stuff out there, I know I did, but I understand that people appreciate the easiness in having someone share
their playlist without needing to plug two phones together, or having an end of the year music rewind, that's ok.

  All I wanted was to listen to music with as little distraction as possible, and I made it as I dreamt it up to be.
  In using this app I hope you do too

