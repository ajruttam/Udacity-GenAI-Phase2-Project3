# Udacity-GenAI-Phase2-Project3
AI Photo Editing with Inpainting

## Project Summary

In this project we are going to build a little app that allows you to select a subject and then change its background, OR keep the background and change the subject.

The process involves a user uploading an image and selecting the main object by clicking on it. The Segment Anything Model (SAM) is activated to create a mask around the selected object, choosing the most accurate mask generated. The user is shown this result to either accept it or refine the mask further with additional points. Once the mask is finalized, the user gives a text description (and possibly a negative prompt) to specify a new background for the selected object. An infill model then creates this new background, and the final image is displayed. Optionally, the user can choose to invert the mask and substitute the subject while keeping the background, as in the example above.

This little app can be used to swap backgrounds, swap subjects, remove objects, and more!

The main functionality of the app: calling the SAM model and processing its output, as well as using a text2image diffusion model to generate the new background or subject.

## Submission

Added samples with description in [Udacity-Project3-trails.pdf](Udacity-Project3-trails.pdf)

Description contains information of the image used, seed, prompts, negative prompts, clicks on input image for SAM to segment properly and if subject/background is infilled

**Sample 1:**
![trial 1](trail1.png)

**Sample 2 (First attempt):**
![trial 2.1](trail2.1.png)

**Sample 2 (Second attempt):**
![trial 2.2](trail2.2.jpg)

**Sample 3:**
![trial 3](trail3.3.jpg)
