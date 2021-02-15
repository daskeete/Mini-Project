# Mini-Project

[My_Video](https://youtu.be/WvwwMrgAgHQ)

## Was your social distance detector effective at detecting potential violations? Are you able to describe how the distance detector is applying its calculations of either being safe or noting a violation?

It was effective to an extent but there were many instances where it failed to highlight visually obvious violations. It seems to be using a range where the variable 'dist' should not fall between: (0 < dist < 0.25). Anything falling within this range is a violation and anything outside this range 'dist > 0.25' is not a violation.



## Do you think this approach would be effective for estimating new infections in real time? 

I think it may be useful in contact tracing as it would help identify people who were inclose contact and violated social distancing requirements. 
I dont think this approach would be effective for estimating new infections in real-time as not everyone who violates social distance requirements is necessarily in close contact with someone who carries the virus. If this were used in a way where all violators were marked as potential new infections, it may end up inflating the estimated infection numbers which is bad. 

## How would you implement such an approach in response to the COVID-19 pandemic we are currently experiencing?
If i had to use this approach i would modify the script so that violators would be highlighted red only if they are in close contact with each for a minimum time limit e.g. (1-5 minutes). As it is right now the detector highlights potential violators immediately which to me isn't a practical design.


## What limitations or improvements might you include in order to improve your proposed design?

I would limit the detector from painting a box red unless a set minimum time limit has been met.
It is not very good at recognizing people standing in a straight line so miltiple camera angles would be a necessary addition to improve the detector's performance. It is also not very good at detecting violations when people are standing very close to the camera whether it's a small or large group. To remedy this cameras should be placed adequately far away enough from pedestrian traffic in a way that no person/group can get too close to the camera.
