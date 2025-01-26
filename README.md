# Expo Camera Initialization Bug

This repository demonstrates a common error encountered when using the Expo Camera API: attempting to access camera features before the camera has properly initialized.  This results in null pointer errors because the camera object isn't fully ready yet.

The `bug.js` file shows the erroneous code, while `bugSolution.js` provides a corrected version that safely handles camera initialization.

This issue is particularly relevant for developers who are new to Expo or haven't fully grasped the asynchronous nature of the Camera API.  The solution uses a simple state variable to track camera readiness.

## How to reproduce:
1. Clone this repository.
2. Run `npm install`.
3. Run `expo start`. 
4. Observe the error in the original `bug.js` file and compare to the fixed implementation in `bugSolution.js`.