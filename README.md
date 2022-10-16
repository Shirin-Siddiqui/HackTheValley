# HackTheValley

## Inspiration
My main aim is to enlighten the visually impaired people and help them learn about their surroundings in the same way as a normal person does. I have incorporated various solutions together to make a complete product to educate the blind and help him/her understand the variety of things the world has to offer and help them learn the same.

## What it does
Face recognition 
IDEA - This system will detect and recognize a person who is known to the visually impaired with help of a camera module fitted on his blind goggles.

Object Detection- 
IDEA - The system will detect and recognize objects placed in front of it through the camera module and notify the blind person.

Image to text to speech conversion- 
IDEA - The text present in front of the camera module will be extracted using OCR, then will be converted into speech and will be audible to the blind person which will simulate reading activity.

3. Blind Stick and Smart Band.
IDEA - Blind Stick- The stick will detect obstacles, water puddles, potholes and notify the blind person through a buzzer mounted on the stick. With the help of this, the blind person will be able to climb stairs up and down, will be notified if there is a pothole/water puddle/obstacle ahead.

IDEA - Smart Band- All the operations provided by the system will be managed by a wrist band which will be worn by the visibly impaired person. The band will have buttons for each operation mentioned above, by the press of a particular button the user would be able to perform that particular operation. This will reduce the over usage of the processor and controller and will in turn reduce the complexity as well as overwhelming the user with too many instructions. The band will also have an SOS button which will alert the users helper ( Any close family member or friend) in case of an emergency.



## How we built it
Face Recognition - Tech Explanation -  The Processor detects faces using HOG algorithm, finds 68 specific points on a face and persons affine transformations. Encodes faces using CNN  and checks the database for getting the name of the person.

Object Recognition - Tech Explanation -  System uses YOLO Object Detection which was first introduced in 2015 and is capable of super real-time object detection, obtaining 45 FPS.
YOLO is able to achieve a large number of object detections by performing joint training for both object detection and classification. Using joint training the model YOLO9000 is trained simultaneously on both the ImageNet classification dataset and COCO detection dataset. The result is a YOLO model, called YOLO9000, that can predict detections for object classes that don’t have labeled detection data.

Image to text to speech - Tech Explanation -  System captures image, converts it into grayscale, extracts text from image using OCR tool, it reads the embeddings using pytesseract.

Smart blind stick and smart band are two integrations I will demo as a prototype on VR since I did not have the hardware components to implement it.

## Challenges we ran into

Challenges that I ran into were getting to increase the accuracy and performance of the models.
Researching which is the best model to use for object recognition.
Had trouble with a few errors in live monitoring and speech rendering, There was a lot of lag in the system and everything hanged all together.
Could not integrate google text to speech since ive already reached a limit on my account with their number of projects i can create with google, thats why use OS library of python to directly run terminal command say to make linux talk back from text speech.

## Accomplishments that we're proud of

Making the model run well enough with image, with a page of a book, a PDF and a Quote.
Error solving and debugging, Faced a alot of errors while implementing these models. issues with libraries, keys, internal linux libraries etc.
But managed to solve all of them.

## What we learned

Learnt how to collect facial data of a person and train the model in order to recognize the persons face.
Object detection in live video camera using YOLO Object detection
Text extraction from image

## What's next for The Visually Impaired

What is next is building an entire hardware system with the smart blind stick and the handy band.
With further enhancements and building at a production level in the market to start helping the visually impaired people.
