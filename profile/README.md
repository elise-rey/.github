[![Osiris-NFT-Banner.png](https://i.postimg.cc/wxSf2Kps/Osiris-NFT-Banner.png)](https://postimg.cc/14rrRj49)

Osiris is a platform where anyone can generate, share and/or sell NFTs in order to help small creators and beginners post their creations by giving them a very friendly and guided user experience.

## Architecture
The application follows a microservices architecture by running multiple small services on the cloud and have a full and automated CI/CD pipeline. Every repository represents one service that is fully independant from others. Osiris NFT is only available on Android.

## Workflow
Every services have their own unique GitHub Action script that builds and pushes their images into a docker repository. A repository dispatch triggers the GitHub Action of the *Deployment* repository composed with multiple configuration and testing files, deploys the updated application on Google Cloud, and then runs multiple tests on each API endpoints.

## Credits
*Authors: Yoann Renard ( Backend ) - Elise Rey ( Frontend ) - Yanis Benhalima ( NFTs ) - Timmy Villeminot ( Authentication )*

*School project, ***ISEN Yncrea Méditerranée, Toulon**.**

## Demo
![Osiris_NFT_demo](https://user-images.githubusercontent.com/76184223/186477812-1af388da-3fb0-4146-841e-abf2bf88de87.gif)
