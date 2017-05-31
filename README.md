# CarND-LaneLines-P1

# Reflection
1. Describe your pipeline. As part of the description, explain how you modified the draw_lines() function.

When I design the draw part. I am thinking about finding the desire slope of the line.
I first find that there may have some horizon line so that i use a filter to get ride of them (slope < 0.5)
Then I find that I have to write 
