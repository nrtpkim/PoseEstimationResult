# PoseEstimationResult
## video
- resolution Full HD(1920 x 1080) 
- 30 fps

## structure of resource
- 1 value in list = 1 frame
```
[
    {
        'pose_landmark':
            {
                'NOSE':{'x':x,'y':y,'z':z},
                'LEFT_EYE_INNER':{'x':x,'y':y,'z':z},
                ...
                'RIGHT_FOOT_INDEX':{'x':x,'y':y,'z':z}
            },
        'right_hand_landmark':
            {
                'WRIST':{'x':x,'y':y,'z':z},
                'THUMB_CMC':{'x':x,'y':y,'z':z},
                ...,
                'PINKY_TIP':{'x':x,'y':y,'z':z}
            },
        'left_hand_landmark':
            {
                'WRIST':{'x':x,'y':y,'z':z},
                'THUMB_CMC':{'x':x,'y':y,'z':z},
                ...,
                'PINKY_TIP':{'x':x,'y':y,'z':z}
            }
    },
    {
        ...
    },
    {
        ...
    },
]
```

## More information about pose estimation
- Pose landmark 33 points
- Right-hand landmark 21 points 
- Left-hand landmark 21 points.
- 1 point consists of [x,y,z]: 
### _Pose Landmark_

[![N|Solid](https://google.github.io/mediapipe/images/mobile/pose_tracking_full_body_landmarks.png)](https://google.github.io/mediapipe/images/mobile/pose_tracking_full_body_landmarks.png)

### _Hands Landmark_
right hand and lest hand is same. 
[![N|Solid](https://google.github.io/mediapipe/images/mobile/hand_landmarks.png)](https://google.github.io/mediapipe/images/mobile/hand_landmarks.png)