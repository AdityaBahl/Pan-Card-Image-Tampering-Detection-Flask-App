# Wordle Game Using Node.js and APIs

![image](https://github.com/AdityaBahl/Wordle-Game/blob/main/sample.png)

## Technologies Used

1. **HTML**
2. **CSS**
3. **Vanilla JavaScript**
4. **Node.js**
5. **[Word Dictionary API](https://rapidapi.com/twinword/api/word-dictionary/)**
6. **[Random Words API](https://rapidapi.com/sheharyar566/api/random-words5/)**

## Getting Started

To start this project please go to **RapidAPI** to sign up for the [APIs](https://bit.ly/rapidapi-hub).

### `.env`

Now create a `.env` file in the root of your project with the following:

```
RAPID_API_KEY={your_rapid_api_key}
```

To run this project please type the following commands:

### `npm i`

This will install all the necessary dependencies.

### `npm run start:backend`

This will start the backend on [http://localhost:8000](http://localhost:8000).

### `copy the path to your index.html file`

Copy the path to this file and paste it in your browser to see the game and play.

To learn React, check out the [React documentation](https://reactjs.org/).

## Why Wordle?

**Wordle** is a web-based game that uses APIs (Application Programming Interfaces) and Node.js to provide users with a fun and interactive experience. APIs allow Wordle to access and retrieve data from external sources, such as a dictionary or thesaurus, and use that data to generate the words and challenges that players must solve. Node.js, a JavaScript runtime built on Chrome's V8 JavaScript engine, is used to execute the game's code and handle its server-side logic. By using APIs and Node.js, Wordle is able to provide a seamless and dynamic gaming experience for players.

## Algorithm

1. The game generates a grid of letters and displays it to the player.
2. The player selects a sequence of letters in the grid to form a word.
3. The game sends a request to a dictionary API to check if the word is a valid English word.
4. If the word is valid, the game updates the score and displays a new grid of letters to the player.
5. If the word is not valid, the game informs the player and allows them to try again.

This is just one possible approach to building a Wordle-like game. There are many other ways to design and implement such a game, and the specific algorithms and techniques used will depend on the desired features and functionality of the game.

## Challenges and Limitations

1. **Integrating with external APIs:** Depending on the APIs used, integrating with them can be a complex task. There may be issues with authentication, rate limiting, or handling unexpected responses.

2. **Managing the game state:** As the game progresses, the state of the game will change (e.g., new grids of letters will be displayed, scores will be updated). Care must be taken to ensure that the game state is properly managed and persisted, especially if the game is being played by multiple users concurrently.

3. **Ensuring performance:** A slow or unresponsive game can be frustrating for players. Careful optimization of the code and use of appropriate caching techniques can help ensure good performance.

4. **Testing and debugging:** As with any software project, testing and debugging are important tasks that must be undertaken to ensure that the game is functioning correctly. This can be especially challenging in a web-based game that involves interactions with external APIs.

5. **Maintaining security:** It is important to ensure that the game is secure and that user data is protected. This may involve implementing measures such as input validation and sanitization, as well as properly handling sensitive information such as passwords and API Keys.

## Conclusion

In conclusion, building a Wordle-like game using APIs and Node.js can be a challenging but rewarding project. By using APIs, the game can access and retrieve data from external sources, providing a rich and dynamic gaming experience for players. Node.js, a JavaScript runtime built on Chrome's V8 JavaScript engine, can be used to execute the game's code and handle its server-side logic. Some potential challenges that may arise include integrating with external APIs, managing the game state, ensuring good performance, testing and debugging, and maintaining security. By carefully designing and implementing the game, it is possible to create a fun and engaging Wordle-like game that players will enjoy.

### MIT Licence

**Copyright (c) 2023 Aditya Bahl**

Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
