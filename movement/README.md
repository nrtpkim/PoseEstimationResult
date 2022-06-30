# PoseEstimationResult
## video
- resolution (960 x 540) 
- 30 fps

## Landmark
- Landmark_Movement_raw.json is ratio 0-1 (ค่าดิบ ที่เป็นอัตราส่วนของหุ่นต้นแบบ)
- Landmark_Movement_aligned_with_video.json is pixel(point) on video movement_video.mp4 (ค่า x และ y ที่นำไปคูณกับ resolution ของวิดีโอแล้ว)

if have any question or need more support please contact team!


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