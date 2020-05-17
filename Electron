const electron = require('electron');
const{ app, BrowserWindow, globalShorcut } = electron;

let mainWindow;

var e2c = require('electron-to-chromium');
var versions = e2c.fullChromiumVersions;
var chromeVersion = e2c.electronToChromium('2.4.11');

app.on('ready', () =>{
	mainWindow = new BrowserWindow({
		width: 1200,
		height: 800,
		fontSize: 120.0
	});

	mainWindow.setTitle('UNCode');
	mainWindow.loadURL('https://meet.google.com/');
	mainWindow.on('closed', () => {
		mainWindow = null;
	});
});