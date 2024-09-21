# Crossroads-Phantom Opera

"Crossroads-Phantom Opera" is an experimental performance that combines augmented reality technology with opera performance. It explores the possibilities of integrating cutting-edge technology with traditional performances, based on the classic Chinese Peking opera "Crossroads". In this performance, AR technology is used to recreate one of the core characters as a virtual phantom, who interacts with real opera actors during rehearsals and performances.

## Introduction

The"Crossroads"  is a traditional Peking Opera played by martial artists.The context of this play was a fight in the dark inn, which meant that even when facing each other, the two performers needed to act as if they were unable to see each other.

In our project, we deliberately made performer not wear the ar headset, so that he could not see the virtual phantom, which just right restored the status and relationship between the two in the original play. Additionally, performer needed to memorize the whole set of movements of both parties and realize the interactions during this "cross-reality" performance.

## production

### Time Synchronization

Performance need to ensure the consistency of the opera image in the eyes of all audience. In addition, we cannot expect and ask all our participants to open the program at the same time to realize this precise requirement.

<img width="650" alt="Screenshot 2024-04-28 at 16 17 16" src="https://github.com/user-attachments/assets/ff24c17e-dd14-4d3b-8f05-f5c53e3a528d">
<img width="650" alt="Screenshot 2024-04-28 at 16 59 28" src="https://github.com/user-attachments/assets/361033ae-a799-4985-8be5-3e82c5fcd174">

### Spatial Synchronization

Immersal which is a spatial scanning technique is utilized to build the venue information of the performance into the project in advance. In our tests we used a simple pedestal with highly recognizable patterns as the basis of scanning to ensure maximum stability of spatial recognition. Ultimately, Spatial synchronization is achieved when all devices are based on one accurate spatial information.

<img width="1364" alt="Screenshot 2024-04-02 at 22 27 54" src="https://github.com/user-attachments/assets/a59d5a71-b831-4247-9de8-7829e4fb9ef0">

#### Spatial Technology Stability Testing

It is possible to achieve almost no error in the stationary standing state, but there is a drift under movement, and this drift increases with movement, with a maximum variation of about 4cm. It takes 3-4 seconds to auto-calibrate after a drift. Moreover, instability occurs at roughly 6m from the center of stage. And it has been tested that having radar on the phone will improve the stability.

<img width="455" alt="Screenshot 2024-07-12 at 11 17 35" src="https://github.com/user-attachments/assets/0be7192c-dfa0-437c-be4f-9eeda08d09e8">
<img width="455" alt="Screenshot 2024-07-12 at 11 17 35" src="https://github.com/user-attachments/assets/028ccbd2-61c2-4289-802e-fc604451f97c">

<img width="632" alt="Screenshot 2024-07-12 at 11 17 35" src="https://github.com/user-attachments/assets/aacce019-205e-4e5d-aab6-2410915c6246">
<img width="277" alt="Screenshot 2024-07-12 at 11 17 35" src="https://github.com/user-attachments/assets/e2b62859-989d-4108-9f2c-79d74d75d5e0">

### Character Animation

#### First testing

Using Movie One to capture the movements of people, then the application provided us the skeletal animation through AI recognition.

<img width="456" alt="Screenshot 2024-07-12 at 11 17 35" src="https://github.com/user-attachments/assets/da423ceb-7005-4e68-9f75-060cbda2ef06">
<img width="454" alt="Screenshot 2024-07-12 at 11 17 35" src="https://github.com/user-attachments/assets/b7c79f7d-66b1-4cfc-92dc-42c18072bfb3">

Drawback: This application only support 1 minute record, making the actors cannot perform coherently.

#### Second testing

Uploading the existent videos to the Racical which is an AI recognition website to gain a skeletal animation. After that, the model should be rigged with the skeleton with that animation manually.

<img width="1512" alt="b8746d75fc60efeba90bab1ed4a46e2" src="https://github.com/user-attachments/assets/2b5ff1e2-9a2b-4970-8c79-e11121febda9">

<img width="457" alt="Screenshot 2024-07-12 at 11 17 35" src="https://github.com/user-attachments/assets/9c7128a5-2113-4297-ae24-1aeabd6c4d83">
<img width="457" alt="Screenshot 2024-07-12 at 11 17 35" src="https://github.com/user-attachments/assets/a9110297-4560-4980-9387-6910dd339b83">

Drawback: This website is only able to recognise 1 minute video.

<img width="457" alt="Screenshot 2024-07-12 at 11 17 35" src="https://github.com/user-attachments/assets/98029276-282a-445b-822f-164b2c092101">
<img width="457" alt="Screenshot 2024-07-12 at 11 17 35" src="https://github.com/user-attachments/assets/c9d5b0a8-bff4-432e-9d9b-37a7168224a7">

Drawback: The capture was not strict accurate and the whole position of human drifted to a certain extent. what's more, the actor's changes of height cannot be recognised, which is a key part of this project.

#### Final testing

Using Xsens motion capture technology to obtain the skeletal animation. Unlike optical motion capture, Xsens' device fixes sensors directly on the motion capture suit which can recognize the acceleration rate and orientation of each sensor to track the exact position of the skeleton. We recorded the movements of the two dancers separately, but made sure that all the movements in the second recording exactly matched the movements in the first recording.

![9月3日(2)](https://github.com/user-attachments/assets/269a819f-606a-45bd-ad86-8212f58febf3)

![微信图片_202404261124181](https://github.com/user-attachments/assets/47ede650-0716-463f-a036-4a00f0e1748d)

<img width="463" alt="Screenshot 2024-07-12 at 11 17 35" src="https://github.com/user-attachments/assets/8cf4cef0-42f8-47c2-ba38-94c38963da0a">
<img width="463" alt="Screenshot 2024-07-12 at 11 17 35" src="https://github.com/user-attachments/assets/773f1d67-4363-4bb2-a3bb-efdb88d93f1b">

### weapon

Import the weapon model into unity and bind the weapon model to the right hand palm bone of the character through code, and ensure that the position and rotation of the weapon are synchronized with the hand in real time.

<img width="1020" alt="Screenshot 2024-06-18 at 12 33 22" src="https://github.com/user-attachments/assets/f6ee97dd-c486-4c2a-bb48-c3df0336a8b8">

