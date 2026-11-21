# Quick Bunny — Level 3

![JavaScript](https://img.shields.io/badge/JavaScript-p5.js-FB7D24?logo=p5dotjs&logoColor=white)
![Game](https://img.shields.io/badge/type-browser%20game-4C8EDA)

A sprite-based browser game in which the bunny tries to reach a carrot while randomly positioned snakes cross the playfield. This iteration adds local artwork and generated moving hazards.

## Play

Use the arrow keys to move. Touching a snake sends the bunny back to its starting position. Reach the carrot to display the win message.

## How it works

preload() loads the background, bunny, carrot, and snake images from images/. setup() creates the 600 × 600 canvas and initializes the sprites. During draw(), the sketch handles movement, edge bouncing, snake generation, collisions, and rendering. Snakes receive randomized positions and horizontal velocities and are removed after a short lifetime.

## Architecture

Keyboard input → bunny sprite → generated snake group → collision/reset or carrot win → canvas rendering

## Start locally

Open index.html in a browser with images/, CSS/, and lib/ in place. No npm install or build command is provided. Use a local static server if local file loading is restricted.

## Project layout

- index.html — browser entry point
- sketch.js — gameplay and sprite logic
- images/ — background, bunny, carrot, and snake artwork
- CSS/ — stylesheet
- lib/ — game libraries

## Limitations

There is no saved progress, score tracking, backend, or automated test suite.