#### Please add your answers to the ***Analysis of  Algorithms*** exercises here.

## Exercise I

a) This is O(n), because it loops as many times as n until a is n^3


b) This code is O(n). It loops n times, and does 2-3 things inside this loop. ( Does `while` count as a step? )


c) I believe this one is also O(n), because it recursively loops until n reaches 0

## Exercise II

This could be found with a binarty search function, I believe. 
Go to the middle of n and if the egg breaks, we'd go to the middle of the lower half etc etc, if the egg doesn't break we'd go up. The difference is that we'd wnat to keep a stored value of the last non-egg-breaking floor in case we end up going to far up


eggsthrown = 0
brokeneggs = 0
non-egg-breaking-floor = none
floors = list of the range of n

while length of floors > 0:
    throw egg halfway
    if egg breaks:
        floors = bottom half
    if egg doesn't break:
        non-egg-breaking-floor  = current floor
        floors = top half

return non-egg-breaking-floor 
