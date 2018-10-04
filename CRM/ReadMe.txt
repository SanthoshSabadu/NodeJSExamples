Download NodeJs from nodejs.org (Installer/zip)
	NodeJS installation gives both the node and npm 

MongoDB installation without Admin rights:  (Installer/zip)
	msiexec /a mongodb-win32-x86_64-2008plus-ssl-4.0.2-signed.msi /qb TARGETDIR="C:\MongoDB"   

Install VisualStudio Code 
	Run commands from View -> Terminal
	Test node and npm installed with commands node -v npm -v

Set the path for both Node and MongoDB, only when zip is downloaded instead of installer.
	>set path=%PATH%;%CD%
	>setx path "%PATH%"

Rest APIs with NodeJS, ExpressJs, MongoDB
	Creating new nodejs project --> Create new folder CRM
	cd CRM > npm init ---> initialize a new package.json, and we use package.json to install express.
	** Entrypoint is important. we use only index.js (default), All others are default.
	within CRM --> (If the node_modules/package.json are exist, will try to build existing from that list only )
		Adding Express --> npm i --save express
		MongoDB --> Window is just installation (Given window link), Mac it is using brew update (Check officical MongoDB site for steps) 
		npm i --save mongoose --> It will save mongo into project.json 
		mongod --> will start the mongo db installed 
		npm i --save nodemon --> refreshes the application automatically.
		npm i --save-dev babel-cli babel-preset-es2015 babel-preset-stage-0   (bablejs.io) babel tool is used to setup ES6 without any issues to make sure without any compilation server.