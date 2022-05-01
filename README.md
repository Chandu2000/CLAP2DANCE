# CLAP2DANCE

🏆DOMAINS🏆
GODADDY: CLAP2DANCE.US

DOMAIN: CLAP2DANCE-WITH.TECH

💡Inspiration💡
Music is all around us, music makes us up. Human beings find delight in music and there are different songs and kinds of music for different scenarios. This inspiration for this project can be likened to this scenario: imagine a person full of joy and entered his/her home and tries to play music to celebrate and dance, he might have to go through the traditional process of putting on the music player and plating the choice song, this sometimes might take a while but what if the person with just a clap can automatically trigger and play song from a music player. This project is about giving people accesibility to music and also dance just at the time that they need it.

🏅USE CASE:🏅
Giving overall accessibilty to people who wish to play music according to mood using Handsfree Gestures
While Gyming or Running Athletes or Users do not have to stop their workout to pause the song or play the next song...using hand clap gestures you can change the songs or modify playlist as to your liking.
Useability for Parties and Hangouts and users can use it to create mixtapes!
❓What it does❓
It is an AI-based device that detects clap of hands and played music from a music player. To improve the functionality, it has security and also child control that the owner can activate, whenever this is activated, any attempt to play a song from the device by a third party will be reported to the owner via SMS notification and the owner can take steps accordingly.

🏗️How we built it🏗️
The device used in this project is the single board microprocessor computer Raspberry pi, it is equipped with an external loudspeaker and a microphone.

First, we trained the device to be able to recognize claps and not just any sound. Google cloud machine learning platform "Teachable Machine" was used in training the model. Samples of background noise were collected and samples of our clap audio were collected, after training the model, the model was exported as a TensorFlow Lite model. This model was used in the code to recognize claps. The Raspberry pi takes the clap input from the microphone and it output the music through the loudspeaker.

Twilio: To enable ease of use, two working modes were configured in the device: Open mode and locked mode. In open mode, it is assumed that the owner has direct use of the device at the moment and there is no need for security. At the lock mode, the owner presses a button on the device and any attempt to use the device will be reported to the owner, this is achieved using Twilio. The locked mode can be activated due to security and also child control reasons.

Twilio is also used for every Pause Song or Resume song or Change Playlist song like features like a bot so that it is easier for user to keep track of the song they listening too and change songs without phone touch.

CockroachDB: It was used to store the user data and creating a playlist for the User with every change in music. It also is updated with information like Artist of the Song, Loudness and Energy and Popularity so that Users can have easy access to information and choose accordingly which choice of song is to be considered. (Here Kaggle Dataset of Spotify Top 50 Songs is taken and replicated here for data entry purpose)

Coil: We have used coil in our site for easy transaction through web monitization for creating personal playlist or buying subscriptions to database of songs. Transactions with coil is quick and simple so we used it as a User friendly Transaction point forupkeep of Music Information and licenses bought.

🚧Challenges we ran into🚧
The first challenge was setting up TensorFlow on a Linux-based computer like the Raspberry pi. The code-based doesn't have enough support so we had to find a way and eliminate all problems encountered.

Another challenge is wiring up our main processor to the output device and input device which are loudspeaker and microphone respectively. We wanted the device to be flexible and opted for a Bluetooth connection between the three, we were able to connect the loudspeaker through Bluetooth after some troubleshooting but the microphone remained wired connection with the Raspberry pi.

🏅🏆ACCOMPLISHMENTS THAT WE ARE PROUD OF🏅🏆
For all the challenges listed above, an accomplishment is that we were able to overcome most of the problems in a limited time. Devices that do a similar thing to the one we build usually take voice input like "Hey Google, play music" but we are able to achieve it on a minimal level using clap, we are proud of this.

📚🙋‍♂️What we learned📚🙋‍♂️
This weekend has been a learning weekend for the team. We had to work in new domains, getting used to hardware and embedded systems programming. We had to learn from scratch how to use Google Cloud Machine Learning's Teachable Machine platform.
We had to learn how to work with music files using python and also a Linux terminal, we learned how to efficiently use Twilio API on raspberry pi and also importantly hardware setting up and connection.

⏱⌛⏳🏃‍♂️Time Management⏱⌛⏳🏃‍♂️
We had a tough time managing time this weekend with our participation in this Hackathon as we had to work on multiple things altogether. We lost a lot of hackathon time in brainstorming and team building yet we are proud that things went according to our plans. Fortunately, we could do this by distributing our work and focusing on multitasking. Extremely excited about all the learnings and teachings we got through this hack.

💭What's next for Clap2Dance💭
Making it more user-friendly but building a GUI interface and providing more clapping options. Adding more Features and Playlists so make it customer accessible and improve Customer satisfaction.
