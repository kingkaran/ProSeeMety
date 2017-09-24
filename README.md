# ProSeeMety
ProSeeMety is an attachment for glasses that would help navigate blind people. This project was made at EngHacks 2017.

The DevPose can be found here: https://devpost.com/software/proseemety

## Inspiration
We are inspired by traffic safety for people with disabilities, especially deaf people. We realized that Canada allows people with certain disabilities to operate an automobile, but they can run into potential dangers since their field of view is limited to what they can see. So we are inspired by the idea of equity in Canada, because everyone has the right to come home safe.

## What it does
It allows deaf people to have a more comprehensive view of their surroundings. ProSeeMety is a companion that is always there for them to alert them of any noises around them.

It has 3 LED lights on top of each lens of the glasses to alert the user about potential dangers. The red, yellow, and green LEDs, each indicating a critical level. Red being very loud, and potentially dangerous noises, such as a car honk, or police vehicles. Yellow being moderate noises, such as a bike bell. Green being everyday noises such as people jogging, or people simply talking. It incorporates sound recognition to bring them only relevant information and alerts.

## How we built it
We used an iPhone's microphones and sound recognition. We made an app that integrated ACRCloud, a music/audio fingerprinting API, for accurate and fast sound recognition. We put simple LEDs on each side of the sunglasses provide by Capital One, and connected them into Arduino 101, a microprocessor, to control the LEDs. Our phone connects to the Arduino using Bluetooth Technology (BLE) and incorporates CoreBluetooth from Swift in XCode to send commands to the Arduino's onboard Bluetooth module identified by UUID to trigger certain LEDs depending on the categorized sound it receives.

## Challenges we ran into
Since this is the Engineering Hackathon we have made a last minute decision on what kind of project should we develop. Even though we knew from the very beginning that this project would be very challenging since 3 of us have never dealt with hardware and 1 of us has just finished the first engineering year. After conducting a research on how people with different impairments travel around city, we have decided that our project will involve signal processing, which would involve high/low pass filters, sound fingerprinting and acoustic localization by analyzing the time that it takes for the sound to travel. However, we were not able to complete acoustic localization since an oscilloscope was not available and we only had 3 operational amplifiers which was not enough (3 for amplifying microphones and 2 for comparitors). In addition, there were no soldering stations so we had to come up with creative ways to connect wires using a lighter. And due to lack of time, we decided to use an existing API for soung fingerprinting.

## Accomplishments that we're proud of
This is one of the hardest projects we attempted as a team, and 2 of our members are first time hackers. They contributed greatly for the project by conducting comprehensive research in the market for aids for people with disabilities, and ran tests for our product. We are proud of being in Canada, where everyone should be treated with equity, we are also proud of our idea and our ability to work as a team to learn over 4 skills each to build this product's prototype.

## What we learned
We learned to use Swift for Bluetooth, and using the Arduino boards to integrate remote control modules. 3 of our team members have not touched Arduino, and are able to learn it in such a short amount of time. We also learned to work with what we have, and coming up with clever and efficient engineering decisions for problems described in "Challenges we ran into" section

## What's next for ProSeeMety
Of course the prototype is far from perfect, in terms of speed, accuracy, and aesthetics. We hope to integrate our own sound recognition software that is built to analyse and recognize sounds more accurately and in real-time. We also hope to design this product to be easily accepted by everyone, and to build the product using eco-friendly materials that are durable and aesthetically pleasing. We also want to make our software opensource, so everyone can integrate it into their apps, or products. For example, car manufacturers can integrate their sensors using our software to push alerts directly into the glass module the driver is wearing. Of course there are infinite possibilities that our product can achieve. This is the first and vital step to solving traffic safety for people with disabilities.
