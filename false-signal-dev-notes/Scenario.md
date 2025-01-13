#code
This can be things like [[Plane]] scheduled to [[Depart]] or [[Building]] at [[POI]]s the [[Open world]] that are now open. 

## Implementation
A scenario is a monoBehavior applied to a gameObject. It contains a list of UnityEvents, which can be added to in the inspector. It has a trigger time, and when that trigger time is reached, those UnityEvents will be triggered.