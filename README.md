# CarND-LaneLines-P1

# Reflection
1. Describe your pipeline. As part of the description, explain how you modified the draw_lines() function.

When I design the draw part. I am thinking about finding the desire slope of the line.
I first find that there may have some horizon line so that i use a filter to get ride of them (0.5< slope < 2)
After getting the desire slope of my part, the rest of the thing is the intercept of the line.
By getting all the parameter I need, I could average all the desire line by using the weight average method.
I use the line length as a weight to all line segments so as to reduce the noise affection.
Also,its hard to decide how long the line should extrapolate, so I set the y coordinates the line should extend.

For the challenge part, I think that i did not do well on it. The line would shake when the the vehicle enter the no line region.
I think that i need other parameter get it since the vehicle could not always rely on the road line.
