# Crossroads-Phantom Opera

"Crossroads-Phantom Opera" is an experimental performance that combines augmented reality technology with opera performance. It explores the possibilities of integrating cutting-edge technology with traditional performances, based on the classic Chinese Peking opera "Crossroads". In this performance, AR technology is used to recreate one of the core characters as a virtual phantom, who interacts with real opera actors during rehearsals and performances.

## Introduction

The"Crossroads"  is a traditional Peking Opera played by martial artists.The context of this play was a fight in the dark inn, which meant that even when facing each other, the two performers needed to act as if they were unable to see each other.

In our project, we deliberately made performer not wear the ar headset, so that he could not see the virtual phantom, which just right restored the status and relationship between the two in the original play. Additionally, performer needed to memorize the whole set of movements of both parties and realize the interactions during this "cross-reality" performance.

<img width="1300" alt="Screenshot 2024-10-08 at 22 20 11" src="https://github.com/user-attachments/assets/444be00b-a2f1-4c25-a320-9944d17a69e0">

![9月3日(1)](https://github.com/user-attachments/assets/9af07cd3-fcc5-4ced-aedd-0d562ea4d7b1)

## Production

### Time Synchronization

Performance need to ensure the consistency of the opera image in the eyes of all audience. In addition, we cannot expect and ask all our participants to open the program at the same time to realize this precise requirement.

<img width="650" alt="Screenshot 2024-04-28 at 16 17 16" src="https://github.com/user-attachments/assets/ff24c17e-dd14-4d3b-8f05-f5c53e3a528d">
<img width="650" alt="Screenshot 2024-04-28 at 16 59 28" src="https://github.com/user-attachments/assets/361033ae-a799-4985-8be5-3e82c5fcd174">

### Spatial Synchronization

Immersal which is a spatial scanning technique is utilized to build the venue information of the performance into the project in advance. In our tests we used a simple pedestal with highly recognizable patterns as the basis of scanning to ensure maximum stability of spatial recognition. Ultimately, Spatial synchronization is achieved when all devices are based on one accurate spatial information.

<img width="1364" alt="Screenshot 2024-04-02 at 22 27 54" src="https://github.com/user-attachments/assets/a59d5a71-b831-4247-9de8-7829e4fb9ef0">

#### Spatial Technology Stability Testing

It is possible to achieve almost no error in the stationary standing state, but there is a drift under movement, and this drift increases with movement, with a maximum variation of about 4cm. It takes 3-4 seconds to auto-calibrate after a drift. Moreover, instability occurs at roughly 6m from the center of stage. And it has been tested that having radar on the phone will improve the stability.

<img width="907" alt="Screenshot 2024-09-21 at 22 24 35" src="https://github.com/user-attachments/assets/773d5683-d918-44ed-af87-39a2cbe250af">

### Character Animation

#### First testing

Using Movie One to capture the movements of people, then the application provided us the skeletal animation through AI recognition.

<img width="909" alt="Screenshot 2024-09-21 at 22 24 24" src="https://github.com/user-attachments/assets/7c91fb5d-ed6e-44f7-8f7a-20f59fc19cfa">

Drawback: This application only support 1 minute record, making the actors cannot perform coherently.

#### Second testing

Uploading the existing videos to the Racical which is an AI recognition website to gain a skeletal animation. After that, the model should be rigged with the skeleton with that animation manually.
<img width="1512" alt="Screenshot 2024-04-07 at 13 54 18" src="https://github.com/user-attachments/assets/48b80980-e4aa-490e-91f8-c19d22d4bf12">

<img width="912" alt="Screenshot 2024-09-21 at 22 24 04" src="https://github.com/user-attachments/assets/ca6e4ee8-7570-49cf-bfd7-9bf755b083a8">

Drawback: This website is only able to recognise 1 minute video.

<img width="914" alt="Screenshot 2024-09-21 at 22 23 56" src="https://github.com/user-attachments/assets/eb4b671a-af31-4842-ae11-53f7f157613a">

Drawback: The capture was not strict accurate and the whole position of human drifted to a certain extent. what's more, the actor's changes of height cannot be recognised, which is a key part of this project.

#### Final testing

Using Xsens motion capture technology to obtain the skeletal animation. Unlike optical motion capture, Xsens' device fixes sensors directly on the motion capture suit which can recognize the acceleration rate and orientation of each sensor to track the exact position of the skeleton. We recorded the movements of the two dancers separately, but made sure that all the movements in the second recording exactly matched the movements in the first recording.

![9月3日(2)](https://github.com/user-attachments/assets/269a819f-606a-45bd-ad86-8212f58febf3)

![微信图片_202404261124181](https://github.com/user-attachments/assets/47ede650-0716-463f-a036-4a00f0e1748d)
<img width="925" alt="Screenshot 2024-09-21 at 22 23 48" src="https://github.com/user-attachments/assets/cc97734f-03dd-4e4a-a5e5-93fd544e8fb4">

### Weapon

Import the weapon model into unity and bind the weapon model to the right hand palm bone of the character through code, and ensure that the position and rotation of the weapon are synchronized with the hand in real time.

<img width="750" alt="Screenshot 2024-06-18 at 12 33 22" src="https://github.com/user-attachments/assets/f6ee97dd-c486-4c2a-bb48-c3df0336a8b8">

<img width="571" alt="Screenshot 2024-05-09 at 14 50 45" src="https://github.com/user-attachments/assets/eb45f8f4-4b08-477f-8c0c-b8ebeb79e891">

## Rehearsal and problems

Programs run with dropped frames, resulting in multiple devices being unable to synchronize their performances. The solution is to configure VSync to set the target frame rate to 30fps, which is lower than the default 60fps running frame rate of cell phones.

<img width="398" alt="Screenshot 2024-09-21 at 22 39 48" src="https://github.com/user-attachments/assets/9619c336-ae13-4cd4-a2db-035098e91b1b">

Real-time detection of engineering operation frame rate

<img width="500" alt="Screenshot 2024-06-18 at 12 26 03" src="https://github.com/user-attachments/assets/c1bd73de-ee78-494b-a72c-3c6e7aa695bf">
<img width="500" alt="Screenshot 2024-06-15 at 16 53 11" src="https://github.com/user-attachments/assets/e88ea6b2-5f2d-4521-8a39-453d053825ea">

Music is added in project to assist performers in rehearsals.

<img width="544" alt="Screenshot 2024-06-18 at 12 25 56" src="https://github.com/user-attachments/assets/eeb485cf-6f78-4657-979a-15a18aa47527">

Even using AR Occlusion in Unity, occlusion is still the biggest problem visually.

<img width="996" alt="Screenshot 2024-09-21 at 23 26 25" src="https://github.com/user-attachments/assets/722910f8-0da6-4790-b2bc-ff5244981b1c">

## Visual Appearance

Build a 3D model based on the image from the original opera and import it into unity, then use vfx and shader to create special effects with ghost characteristics. In addition, the weapons are restored to the original opera image.

<img width="699" alt="Screenshot 2024-09-21 at 23 35 29" src="https://github.com/user-attachments/assets/bba1d318-0d48-4731-a330-9331619a9e85">

## Performance

![WechatIMG1221](https://github.com/user-attachments/assets/c036a201-1830-426f-bc6f-57c1d11cd281)

![9月3日(12)](https://github.com/user-attachments/assets/2017bc83-c246-4a06-9248-b367dd251e5b)

![9月3日(9)](https://github.com/user-attachments/assets/631abe0f-6f43-4d48-a1f4-b668ff21af7b)

<img width="1300" alt="Screenshot 2024-09-21 at 23 37 44" src="https://github.com/user-attachments/assets/5ffa93e5-3e95-4c9b-9171-4d71ea22ae0d">

## Requirements

This project aims to build an app runs on iOS device.

1.Unity 2023.2.1f1

2.Xcode 15.2

3.iPhone with lidar capability
