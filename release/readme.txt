Support
1. Windows (amd64 : ScrapperMin.exe)
2. Linux (amd64 : ScrapperMinLinux64, arm : ScrapperMinLinuxArm, 386 : ScrapperMinLinux386)
3. Mac (amd64 : ScrapperMinDarwin64, 386 : ScrapperMinDarwin386)
4. Android (ScrapperMinAndroid.aar and ScrapperMinAndroid-sources.jar)
5. C-Library for Windows (ScrapperMinShared)

In deployment setting, determine the processor architecture and OS and use the file for it and includes the Scripts folder.
Scripts folder must be at the level of the executable.

To test
> ScrapperMin.exe DownloadFile.txt

To run on linux having amd64 processor architecture
> chmod +x ScrapperMinLinux64
> ./ScrapperMinLinux64 DownloadFile.txt

Note : in Linux/Mac both the executable and the scripts name is case sensitive

And you will get a mp3 file which the ScrapperMin downloads for you instructed by DownloadFile.txt script residing in Scripts folder
