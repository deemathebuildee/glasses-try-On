# Virtual Glasses Try-On

A live webcam try-on for prescription glasses that runs in the browser. Your face is tracked in real time, and a 3D pair of glasses follows your head as you move and turn.

Built during **AL-Qimmah camp by Tuwaiq club in UQU university, in October 2026.**

Live demo: https://deemathebuildee.github.io/glasses-try-On/ 

## The Problem

People buying prescription glasses online cannot see how a frame will look on their own face. They guess from product photos, which often leads to a poor fit and returns.

## The Solution

A virtual try-on in the browser. Turn on your camera, see yourself wearing the glasses live, and switch between frame styles with one click.

## Features

- Live webcam face tracking
- 3D glasses that follow head position and rotation
- Automatic sizing of each glasses model
- Switch between frame styles

## Built With

- HTML, CSS and JavaScript
- MediaPipe Face Landmarker (face tracking)
- Three.js (3D rendering)
- GLB 3D models from Sketchfab

## How to Run

1. Download or clone this repository.
2. Open the folder in VS Code and start it with the Live Server extension (right-click index.html, then Open with Live Server).
3. Allow camera access when the browser asks.

Note: the camera only works on localhost or on an https link, so opening the file by double-clicking will not work.

## Project Files

- index.html: the page and all of the code
- glasses.glb, glasses2.glb: the 3D glasses models

## How It Works

1. The webcam video is sent to MediaPipe every frame.
2. MediaPipe returns the head position and rotation.
3. Three.js draws the glasses on a transparent layer over the video.
4. The glasses are attached to the head's position, so they move with the face.

## Known Limitations

- The glasses position and size were tuned by hand on one face, so the fit may vary on other faces.
- The arms of the glasses do not disappear behind the ears.

## What Is Next

- Automatic fit for every face, using MediaPipe's 478 face landmarks
- Frame recommendations based on face shape and size
- AI style suggestions based on what the user likes
- Colour picker, snapshot button, and more frame styles

## Credits

- Glasses models: Glasses by C.U.V on Sketchfab, license: CC Attribution, [[link to model page](https://sketchfab.com/3d-models/glasses-05497943410d4a7388695190a5a68eac)]
- Face tracking: Google MediaPipe
- 3D rendering: Three.js
- Built with help from Claude, an AI assistant
  
## Author

Deema Saleh
