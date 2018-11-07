Many people has been asking, what is ScrapperMin?

ScrapperMin is basically a linux/mac/windows executable that receives a script in text file and a set of arguments then return the web automation process the script is used for

Example
1. I have a script call OpenLoad.txt that uploads file to Video Hosting service call openload.co (just like youtube)
2. The file requires username, password and the path of the video file to upload
3. The script returns the shared url of the video

>ScrapperMin.exe OpenLoad.txt -file=args.txt

If you notice, we have a args.txt file which is the arguments required by OpenLoad.txt, inside this file is :
[param]
email@email.com
[param]
password
[param]
C:\example\test.mp4

the syntax is actually equal with
>ScrapperMin.exe OpenLoad.txt email@email.com password "c:\example\test.mp4"

ScrapperMin is a useful software that you can write script for it to interact with any websites in the world even the website does not have API. It uses plain HTTP protocol with URL/Multipart encoded to upload text, files, download files, login, logout, posting, etc.

It can automate many web related things without having to use a browser and manually clicking on the browser, but instead it acts as a headless browser and allowing interacting with the web directly without loading any interface.

It is 1000 times faster compare to headless browser because it hacks directly into the end point of the website by passing the need to load any javascript.

Developer of scripts need to learn ScrapperMin language, and its standard library.

ScrapperMin has 3 versions
1. .NET
2. Java supported by Android
3. Go

With ScrapperMin moving to Go language, it embarks to a new journey of being a single independent piece of software without any need of installing extra runtime.
