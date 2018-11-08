Support
1. Windows (amd64 : ScrapperMin.exe)
2. Linux (amd64 : ScrapperMinLinux64, arm : ScrapperMinLinuxArm, 386 : ScrapperMinLinux386)
3. Mac (amd64 : ScrapperMinDarwin64, 386 : ScrapperMinDarwin386)

In deployment setting, determine the processor architecture and OS and use the file for it and includes the Scripts folder.
Scripts folder must be at the level of the executable.

To test
>ScrapperMin.exe DownloadFile.txt

Note : in Linux/Mac both the executable and the scripts name is case sensitive

And you will get a mp3 file which the ScrapperMin downloads for you instructed by downloadfile.txt script residing in Scripts folder
