# Pre-work - *Memory Game*

**Memory Game** is a Light & Sound Memory game to apply for CodePath's SITE Program. 

Submitted by: **Anoushka Erram**

Time spent: **3** hours spent in total

Link to project: (https://glitch.com/edit/#!/cultured-prong-jelly?path=README.md%3A1%3A0)

## Required Functionality

The following **required** functionality is complete:

* [x] Game interface has a heading (h1 tag), a line of body text (p tag), and four buttons that match the demo app
* [x] "Start" button toggles between "Start" and "Stop" when clicked. 
* [x] Game buttons each light up and play a sound when clicked. 
* [x] Computer plays back sequence of clues including sound and visual cue for each button
* [x] Play progresses to the next turn (the user gets the next step in the pattern) after a correct guess. 
* [x] User wins the game after guessing a complete pattern
* [x] User loses the game after an incorrect guess

The following **optional** features are implemented:

* [ ] Any HTML page elements (including game buttons) has been styled differently than in the tutorial
* [ ] Buttons use a pitch (frequency) other than the ones in the tutorial
* [ ] More than 4 functional game buttons
* [ ] Playback speeds up on each turn
* [ ] Computer picks a different pattern each time the game is played
* [ ] Player only loses after 3 mistakes (instead of on the first mistake)
* [ ] Game button appearance change goes beyond color (e.g. add an image)
* [ ] Game button sound is more complex than a single tone (e.g. an audio file, a chord, a sequence of multiple tones)
* [ ] User has a limited amount of time to enter their guess on each turn

The following **additional** features are implemented:

- [ ] List anything else that you can get done to improve the app!

## Video Walkthrough

Here's a walkthrough of implemented user stories:
![http://g.recordit.co/xsaXG4Nsj9.gif](http://g.recordit.co/xsaXG4Nsj9.gif)


## Reflection Questions
1. If you used any outside resources to help complete your submission (websites, books, people, etc) list them here. 
[None]

2. What was a challenge you encountered in creating this submission (be specific)? How did you overcome it? (recommended 200 - 400 words) 

[This project was definitely out of my comfort zone and I have never coded in HTML, JavaScript, or CSS before so it was a bit tricky at first. Initially, I had to get used to the difference in syntax and recognize how even the smallest space can make a difference in how the program is interpreted by the compiler. The first error that I encountered was that my buttons were not lighting up when the user clicked them and I double and triple checked my code to make sure I had not made any obvious coding errors. Once I started combing through each line, I realized that the issue was that a single space between #button1: and active. This pushed me to be extra careful when coding the rest of the project and understand that the small things do matter in javascript unlike in java. The second challenge I encountered was when I clicked start and received the first clue. Whether I entered the correct sequence or not, I was not receiving the Game Over message nor was I being given a second sequence to continue the game. I then realized that the issue was with the guess(btn) function. I had originally tried to code it myself without using the given function, but I had failed to call the playClueSequence() in the first else statement. While it was a very silly mistake, I figured it out by checking where each function I had created was called and when I saw that playClueSequence() had only been called once when the game started, I quickly realized that it had to be called in the guess function. I double checked with the code that was provided and fixed my error immediately and the game was working!]

3. What questions about web development do you have after completing your submission? (recommended 100 - 300 words) 

[Throughout my career in computer science I have studied various languages, methods, and avenues to go from an idea to a finished product. And much of my education thus far has been learning the fundamentals of these languages and their various applications. My large question and interest in web development is creating a polished project that a user can enjoy. Furthermore, I would like to learn how to optimize user experience and aesthetic, and new techniques on accomplishing that as well. How can I as a designer create an interface that people will want to use? I aim to join the industry, and having this knowledge would help me achieve my goal of being able to create better, more user friendly products that are accessible on all platforms and can be put to great use.]

4. If you had a few more hours to work on this project, what would you spend them doing (for example: refactoring certain functions, adding additional features, etc). Be specific. (recommended 100 - 300 words) 

[If I had a few more hours to work on this project, I would definitely spice up the game as a whole and make it more challenging for users. I would create an easy, medium, and hard mode of the game and the user would be able to choose which level of difficulty they want. The easy mode would essentially be the same as the base project for our submission. The medium mode would have an additional block and a certain number of guesses before the user loses the game. I would do this by creating another block in the index.html file and style it in the style.css file. For the guess count, I would create a function that keeps track of how many guesses the user has taken, and use an if statement to tell the program that when the number of guesses has exceeded 3, call the loseGame() function. In addition to the features from the medium mode, I would increase the difficulty of hard mode by creating another block(total of 6 blocks), decreasing how long each clue plays for and the time between each clue, and add a timer that gives you about 5-10 seconds to enter your guess. I would change the time of how long each clue plays by editing the clueHoldTime constant and reduce the cluePauseTime to make the clues run faster. This will push the user to be more attentive when the sequences are being played. To be completely honest, I am unsure how to implement a timer into the game, but I do know that I would create a block in the upper right corner and would implement the setInterval method to create a 10 second timer that would begin counting down as soon as the clue sequence ended.]


## License

    Copyright [Anoushka Erram]

    Licensed under the Apache License, Version 2.0 (the "License");
    you may not use this file except in compliance with the License.
    You may obtain a copy of the License at

        http://www.apache.org/licenses/LICENSE-2.0

    Unless required by applicable law or agreed to in writing, software
    distributed under the License is distributed on an "AS IS" BASIS,
    WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
    See the License for the specific language governing permissions and
    limitations under the License.
