Here's a plain-language summary you can use for website copy:

How Nailometry measures your nails

The user opens the app and photographs each finger — one at a time — with a US quarter or credit card in frame as a physical scale reference. The app guides alignment in real time and auto-captures when the shot is stable.

The photo is sent to a server that runs a two-part computer vision pipeline:

Reference object detection — The server precisely detects the coin or card using Hough circle transforms, radial gradient refinement, and ellipse fitting. This establishes an exact pixel-to-millimeter scale, and the coin's geometry is used to correct for any phone tilt angle.

Nail plate segmentation — Using SAM 2 (Meta's Segment Anything 2 AI model), the server isolates the finger from the background, then precisely segments just the nail plate. It runs three slightly jittered attempts and takes the median measurement to ensure stability. Classic OpenCV techniques (Canny edges, minAreaRect, ellipse fitting) then extract the nail's true width in pixels.

The pixel width is divided by the calibrated pixel-per-mm scale to produce a measurement in millimeters. Every result gets a confidence score (high/medium/low) based on tilt angle, segmentation quality, and measurement consistency — low-confidence shots prompt the user to retake.

Output: nail width in mm per finger, to 0.1mm precision, with no calipers or professional equipment needed.

Key tech talking points for the website:

Uses AI segmentation (SAM 2) + classical computer vision together
Works with any smartphone camera — no special hardware
A physical reference object (coin or card) eliminates camera distortion
Self-corrects for phone tilt
Confidence scoring ensures only reliable measurements are saved