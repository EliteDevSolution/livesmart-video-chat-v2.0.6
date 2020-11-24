# livesmart-video-chat-v2.0.6
Live Smart Video Chat 
“LiveSmart Video Chat”
Created: 12/01/2019
By: Nikolay Hadjidimitrov
Email: info@new-dev.com

Thank you for purchasing my extension. If you have any questions that are beyond the scope of this help file, please feel free to email via my user page contact form here.

Table of Contents
Overview
Supported Browsers
Features
Usage
Industries
Quick Start Guide
Video Tutorial
Installation and FAQ
Overview - top
LiveSmart Video Chat is a standalone web application with video, audio, recording, screensharing and file transfer face-to-face communication channels and integrated chat. It has own push notification server, that is based on Socket.io or Rachet PHP websocket libraries. It does not require any additional installations or third party logins and accounts. The contact button can be set on your web site and give you information about your visitors. They can directly call you if you are online.

Supported Browsers - top
LiveSmart Video Chat is supported on all major browsers:

- Desktop PC. Microsoft Edge 12+, Google Chrome 28+, Mozilla Firefox 22+, Safari 11+, Opera 18+, Vivaldi 1.9+, IE 11 (Needs installation of Temasys plugin. You will be guided through the installation process)
- Android. Google Chrome 28+ (enabled by default since 29), Mozilla Firefox 24+, Opera Mobile 12+
- Chrome OS.
- Firefox OS.
- Blackberry 10.
- at least iOS 11. MobileSafari/Mac Safari. For legacy Safari (older than v.11) you will be prompted to install Temasys plugin.
Features - top
- Live video and/or audio chat;
- Multi user conference video sessions;
- Whiteboard;
- Broadcast to many;
- Configurable entry form available both with front end access (from the agent) or PHP and MySQL scripting;
- Own notification server, no third party software or accounts needed;
- File transfer;
- Record every aspect of your live stream - video, screen share, whiteboard and chat;
- Private rooms;
- Snapshot;
- URL shortener;
- Offline form so never miss a customer inquiry;
- Pure HTML5 Web chat;
- Chat history;
- Voice to chat module;
- Screen sharing. Supported on Chrome up to 71 with additional plugin (Your will be guided in the installation process), Chrome 72+, Firefox 52+ and MS Edge 17+ browsers are pluginless;
- Switch between front and back camera of your mobile;
- Notification system;
- Mobile friendly;
- Button for establishing a direct connection and a facility to track the presence of your visitors;
- Predefined buttons styling;
- Internationalization;
- Ability to set own video chat room;
- Meeting Scheduling;

You can check the User Guide section for a detailed description of all the features.

Requirements
- HTTPS (SSL certificate) needed;
- For server side scripts: at least Node 4.0 or PHP 5.4 needed;
- You can set own TURN server (recommended) or use the Google default STUN servers.
- No DB needed;
Usage
Possible usages:

- Set an online/offline contact button on your site and track and contact your visitors;
- Set a private room and share it with your contacts in order to establish a direct video call with screen sharing and file transfer;
- Switch between front and back camera of your mobile to make an outstanding demo for your customers;
- Use only chat for support and fun;

Check here available scenarios of usage!
Industries
- All kind that can use peer-to-peer video communication on most of the browsers;
- Tech support. Share screen or transfer files with your troubled customers;
- Health care consultations;
- Online sales;
- Real estate agents;
- Car resellers;
Quick Start Guide
For your back-end you need Node.js 8.0+, root access to your server and opened port 9001;
Now you can start with installation process. Copy all the files to your destination folder;
(optional) Move ws folder outsite the public one;
Edit /ws/server/config.json file so "sslKey": "../ssl/key.pem" and "sslCert": "../ssl/cert.pem" point to your actual certificates. Usually the key is in /etc/ssl/private/ or /home/USERNAME/ssl/keys and the certificate is in /etc/ssl/certs/ or /home/USERNAME/ssl/certs folders in your server file system:
After this, in /ws/server folder you need to run npm install.
For better service management install pm2 with npm install pm2 -g
Start the signaling server with pm2 start server.js in /ws/server folder
After you have your signaling server installed, open config/config.json file and edit YOUR_DOMAIN with your server;
Edit the sample HTML pages in the root of your folder, agent.html and client.html. Change YOUR_DOMAIN with your server too;
When done you can check if this is working. Open agent page and click on Generate Link button. It will open a new page in a popup and put in the clipboard the corresponding link, that you can open in a new browser or device. The other option is to open client.html and click on the button to open the popup from there;
Video Tutorials
Installation process
