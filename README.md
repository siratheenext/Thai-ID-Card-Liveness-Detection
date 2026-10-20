# Thai ID Card Liveness Detection

Internship project at InDistinct — a system that checks whether a submitted Thai national ID card is a genuine physical card, or a reproduction (printed paper / photo of a screen), using a normal photo plus a flash photo of the same card.

## What it does

- User uploads two photos of the same ID card: one taken normally, one with the camera flash on
- The system compares the image itself and how the light response changes between the two photos to classify the card as genuine / paper / screen
- Combines several independent checks into one overall confidence score, with each check's individual result shown separately so the verdict stays interpretable rather than a single black-box number

## Demo

![Card Liveness result — genuine card detected with 88% confidence](demo.png)

*Example result: a genuine Thai ID card correctly classified, with 88% overall confidence broken down across the independent checks. Personal details in the card photos are redacted.*

## Tech stack

FastAPI backend, Angular frontend, Python computer vision (YOLO + image/light analysis)

## Note

This is a company project built during my internship at InDistinct. The production code is private company IP and is not included here — this repository documents the project and its result only, shared with my team's approval.
