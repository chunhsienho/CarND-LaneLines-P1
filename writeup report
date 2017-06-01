# **Finding Lane Lines on the Road** 

## Writeup Template

### You can use this file as a template for your writeup if you want to submit it as a markdown file. But feel free to use some other method and submit a pdf if you prefer.

---

**Finding Lane Lines on the Road**

The goals / steps of this project are the following:
* Make a pipeline that finds lane lines on the road
* Reflect on your work in a written report



### Reflection

### 1. Describe your pipeline. As part of the description, explain how you modified the draw_lines() function.

My pipeline consisted of 5 steps. First, I set the desire region. Secondly, I change the picture into grayscale. This would help me do the gaussian blur. I set a 9 on kernel size. Then I use the canny method and finally use hough_lines and weighted_img function to do the hough transform.

When I design the draw part. 
I am thinking about finding the desire slope of the line. I first find that there may have some horizon line so that i use a filter to get ride of them (0.5< slope < 2) After getting the desire slope of my part, the rest of the thing is the intercept of the line. 
By getting all the parameter I need, I could average all the desire line by using the weight average method. I use the line length as a weight to all line segments so as to reduce the noise affection. 
Its hard to decide how long the line should extrapolate, so I set the y coordinates the line should extend.

Try your lane finding pipeline on the video below. Does it still work? Can you figure out a way to make it more robust? If you're up for the challenge, modify your pipeline so it works with this video and submit it along with the rest of your project!

### 2. Identify potential shortcomings with your current pipeline
For the challenge part, I think that i did not do well on it. The line would shake when the the vehicle enter the no line region. Also, this method can not detect the curve line in the highway because the parameter in canny is only straight line.
Suggest possible improvements to your pipeline


### 3. Suggest possible improvements to your pipeline

The potential improvement I think is to set a if/else in the draw part for the horizon line. Or I could just let the line unchanged when there is no desire line on the movie. I think that i need other parameter get it since the vehicle could not always rely on the road line.
Optional Challenge
