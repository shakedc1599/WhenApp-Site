# WhenApp
we have created a site "inspired" by WhatsApp for multi platform communication.

### Preview
<img src="https://user-images.githubusercontent.com/92931230/164974162-bfb6b82e-ffaa-4ef6-874c-aa6e72c4ee8a.png" width="1000">
<img src="https://user-images.githubusercontent.com/92931230/164974175-2a0fd857-3ee9-4827-869b-dd7363a85131.png" width="1000">

### Development
The web site was created using React JS, and server side using ASP.NET.
Also used axios and signalR libraries. 

### Features
1. supports registration and login.
2. great design.
3. responsive server.
4. we have added a rating page.
5. You can search ratings by name or by text.

### Creators
this site was created by noam cohen, shaked cohen and roi avraham.

## How To Run
for this project you need to clone 3 repos:
  1. [Web Site (react)] https://github.com/NoamCohen48/whenapp2.git
  2. [Server (ASP WebAPI)] https://github.com/NoamCohen48/WhenApp3.git
  3. [Rating page (ASP MVC)] https://github.com/Roi-Avraham/webClientEx2.git

for running the react client:
1. install dependencies using `npm i`
2. run site using `npm start`
3. open `http://localhost:3000/` with a browser
4. change in ustils/globals the paths so servers:
   thisServer - API server (the server in https://github.com/NoamCohen48/WhenApp3.git)
   ratingServer - MVC server (the server in https://github.com/Roi-Avraham/webClientEx2.git)
- **to run 2 or more clients, run each in a separate browser because this app uses cookies**

for running the api server:
1. make sure to install mariadb with username root and password toor.
2. delete db called WhenUpDB if exist.

> you can skip those 2 steps by changing the db settings in `WhenAppContext`
> ![Screenshot_1](https://user-images.githubusercontent.com/92931230/169861142-caac3fb0-8244-4c7c-a4b3-6d7413e2cf57.png)

3. delete migration folder.
4. in package manager run `Add-Migration init` and `Update-Database`.
5. run the server

for the rating server:
1. delete migration folder.
2. in package manager run `Add-Migration init` and `Update-Database`.
3. run the server

> if needed, install EntityFrameworkCore by entering int Package Manager Console  
> `Install-Package Pomelo.EntityFrameworkCore.MySql -Version 6.0.1`  
> `Install-Package Microsoft.EntityFrameworkcore.Tools -Version 6.0.1`  

### Dependencies
this project uses:
- react
- react router - `react-router-dom`
- bootstrap - using cdn
- ASP.net
- Axios
- SignalR
