# chat_app
A commandline chat application which runs on the network designed in CP341 Computer Networking.

## Introduction
This C project provides an example application that works on the custom CP341 network.
- `chat.c` is an example CLI that makes use of the applictation layer to interactively send and receive chat messages on the network.

## Building and Running
This code depends on our nic_app library, which is available [here](https://github.com/tonydoesathing/nic_app). To compile and run the code, run the following commands:  
git clone https://github.com/tonydoesathing/nic_app
cd chat_app  
./library_script.sh  
./src/chat

Note: in order to make network calls, the router from [nic_net](https://github.com/Jessicat-H/nic_net) must be running on the computer you wish to run the application on.

## Data Structure
This application calls the sendMessage function of the [nic_app](https://github.com/tonydoesathing/nic_app) library, passing it a destination to send the message to, a string of text recieved from the user, the length in bytes of that text, and the app id defined for this application.

## Authors
The following code was written by [Jessica Hannebert](https://github.com/Jessicat-H), [Dylan Chapell](https://github.com/dylanchapell), and [Tony Mastromarino](https://github.com/tonydoesathing).
