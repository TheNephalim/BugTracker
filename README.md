# BugTracker application

This project is part of ASP.NET Core. You can find samples, documentation and getting started instructions for ASP.NET Core at the [Home](https://github.com/aspnet/home) repo.
The equivalent MVC5 project is in [https://bitbucket.org/howarddierking/demo-katana-bugs]([https://bitbucket.org/howarddierking/demo-katana-bugs).

* Clone the repository

### Run the application on Helios:
* If you have Visual Studio 2015 Preview
    1. Open BugTracker.sln in Visual Studio 2015 Preview and run the application. 
* If you don't have Visual Studio 2015 Preview
    1. Open a command prompt and cd ```\src\BugTracker\```
    2. Execute ```kpm restore``` to restore all the necessary packages.
    3. Execute ```Helios.cmd``` to launch the app on IISExpress from command line (Application started at URL **http://localhost:5001/**).

### Run on WebListener/Kestrel:
* Open a command prompt and cd ```\src\BugTracker\```
* **[WebListener]:**
	4. Run ```k WebListener``` (Application started at URL **http://localhost:5002/**)
* **[Kestrel]:**
	5. Run ```k Kestrel``` (Application started at URL **http://localhost:5004/**)
* **[CustomHost]:**
	6. Run ```k run``` (This hosts the app in a console application - Application started at URL **http://localhost:5003/**)

### To run the sample on Mac/Mono:
* Follow [Home](https://github.com/aspnet/home) instructions to install mono, kvm on Mac
* Open a command prompt and cd ```\src\BugTracker\```
* Execute ``kpm restore```
* Try `k Kestrel` to run the application

### Note:
1. Application is started on different ports on different hosts. To change the port or URL modify ```Helios.cmd``` or project.json commands section in case of self-host and customhost.
