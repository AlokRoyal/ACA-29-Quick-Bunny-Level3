# Quick Bunny — Level 3

A sprite-based browser game in which the bunny tries to reach a carrot while snakes appear across the playfield. This version adds local artwork and randomly positioned moving hazards.

## How to play

Use the arrow keys to move. Touching a snake returns the bunny to its lower-left starting point; reaching the carrot displays the win message.

## What the sketch does

preload() loads background, bunny, carrot, and snake images from images/. setup() creates the 600 × 600 canvas, player, target, and snake group. draw() handles movement, boundary bouncing, collisions, and rendering. generateSnakes() adds a snake periodically, gives it a random position and horizontal velocity, and removes it after a limited lifetime.

## Run locally

Open index.html in a browser with images/, CSS/, and lib/ in their existing locations. No npm installation or build command is provided.

## Stack

HTML5, CSS, JavaScript, p5.js, and p5.play. This is a local browser game prototype with no backend or persistent score.