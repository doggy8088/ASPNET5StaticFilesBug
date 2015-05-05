# ASPNET5StaticFilesBug

## How To Reproduce

1. Clone this project
2. Open ASPNET5StaticFilesBug.sln using Visual Studio 2015 RC
3. Setup "Empty" as a startup project
4. Ctrl + F5
5. Browse to the "/Project_Readme.html" page.  It will show up "Hello World!".
6. Then switch back to Visual Studio 2015.  Setup "WebAPI" as a startup project.
7. Ctrl + F5
8. Then switch back to Visual Studio 2015.  Setup "Empty" as a startup project.
9. Ctrl + F5
10. Browse to the "/Project_Readme.html" page.  It will show up "Project_Readme.html" content.

## Problem Description

I don't include the "Microsoft.AspNet.StaticFiles" package in my "Empty" project.  The "Project_Readme.html" content should never be displayed.