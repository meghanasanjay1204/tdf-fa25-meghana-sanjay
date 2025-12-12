# TDF Weekly Progress Reports
Hey, I'm Meghana (Megzu) 🌻
I’m maintaining this journal to document my process through the Technology Design Foundation class, which is a mix of electronics and digital fabrication. Very excited to learn, experiment, and do fun stuff along the way!

# Journal Index  

- [Week 1](#week-1)  
- [Week 2](#week-2)  
- [Week 3](#week-3)  
- [Week 4](#week-4)
- [Week 6](#week-6)
- [Week 7](#week-7)
- [Week 8](#week-8)
- [Week 9](#week-9)
- [Week 10](#week-10)
- [Week 11](#week-11)
- [Week 12](#week-12)
- [Week 13](#week-13)
- [Week 14](#week-14)
- [Week 15](#week-15)

---

# Week 1   
## Electronics 🔌| 02.09.2025 - 09.09.2025
In the first week, we were introduced to the syllabus and the general direction of TDF. I am in the Directed section with Prof. Sudhu Tewari and Chris Mayers, where the emphasis is on creating feasible things over simply visible or desirable ones, a refreshing shift in perspective. We received our toolkits, which was really exciting and made the course feel tangible right from the start. Although I’ve previously overseen projects that involved microcontrollers and electronics. Prof. Tewari also shared useful resources for brushing up on Arduino basics, which I’ve started exploring.
### Resources
[https://github.com/loopstick/ArduinoTutorial?tab=readme-ov-file#exercise-2]\
[https://learn.adafruit.com/ladyadas-learn-arduino-lesson-number-0?view=all]
### Experiments
1. Built-in Blink: I ran the classic blink sketch that makes the onboard LED at pin 13 turn on and off every second.
2. External LED Blink: I connected an LED to pin 8 with a resistor and made it blink at one-second intervals, similar to the built-in LED.
``` int externalLED = 8;   // external LED connected to pin 8

void setup() {
  pinMode(externalLED, OUTPUT);  // set pin 8 as output
}

void loop() {
  digitalWrite(externalLED, HIGH);  // turn LED ON
  delay(1000);                      // wait 1 second
  digitalWrite(externalLED, LOW);   // turn LED OFF
  delay(1000);                      // wait 1 second
}
```
3. Built-in + External Blink: Tried to connect both at the same time and it worked.


### Assignment - Hello World with LED Blinking

``` int ledPin = 13;  // Built-in LED on pin 13

void setup() {
  pinMode(ledPin, OUTPUT);     // Set LED pin as output
  Serial.begin(9600);          // Start serial communication at 9600 baud
}

void loop() {
  // Turn LED ON
  digitalWrite(ledPin, HIGH);
  Serial.println("Hello World! LED is ON");
  delay(1000);                 // Wait 1 second

  // Turn LED OFF
  digitalWrite(ledPin, LOW);
  Serial.println("Hello World! LED is OFF");
  delay(1000);                 // Wait 1 second
}
```
### Media
#### Images
<p><img src="with bulb.jpeg"></p>

#### Videos

https://github.com/meghanasanjay1204/tdf-fa25-meghana-sanjay/blob/main/task%201.mp4 \
https://github.com/meghanasanjay1204/tdf-fa25-meghana-sanjay/blob/main/blink%20bulb.mp4 \
https://github.com/meghanasanjay1204/tdf-fa25-meghana-sanjay/blob/main/blink%202%20bulbs_ext%208.mp4 \
https://github.com/meghanasanjay1204/tdf-fa25-meghana-sanjay/blob/main/Blink_13.mp4 \

## Digital Fabrication 🛠️ | 04.09.2025 - 11.09.2025
In the first week of digital fabrication, we were introduced to the **laser cutter**. Chris Mayers gave us a training session on how to properly operate the equipment. We covered not only what to do but, most importantly, what *not* to do when handling the machine. Safety and precision were key themes, which helped set the tone for how powerful and delicate this tool can be.  

### Assignment - Personality Ring
For our first assignment, we were asked to experiment with **Adobe Illustrator** and design a ring that reflects our personality. When I first came here, I was told to “go fly.” That thought stayed with me, and I wanted to create wings. But then I imagined something more playful, the blades of a helicopter! That idea shaped my experiment, and I began designing a small hand-held spinning toy.

#### Iteration 1
I quickly sketched a drawing of a large fan-like structure with three blades and a central hole.  
The design included a ring with a pointed extrusion on top to pass through the blades, and a stopper to hold it in place.  
After making the first prototype, I realized:
- The blades were too long — uncomfortable to wear on the hand.  
- The blades were too thin — prone to breakage.  
- The ring fit was loose.  
- A single ring wasn’t strong enough to support the structure.  
- The projection on the ring was too short to hold the cap securely.  
*(I also struggled with the software a little, but with help from buddies and Chris, I managed to get it done.)*

https://github.com/user-attachments/assets/ad9cbafc-0c7b-40bf-b54a-b06f98a691e8
<p><img src="WhatsApp Image 2025-09-11 at 12.51.49.jpeg"></p>

#### Iteration 2
To improve the design:
- Decreased the diameter of the ring for a tighter fit.  
- Added a second ring to stack together for stability.  
- Increased the height of the projection on the ring so the stopper could hold properly.  
- Reduced the length of the blades to make it more wearable.
- 
https://github.com/user-attachments/assets/badf731b-d3d2-4213-93a7-4ad2b3cbcd02
<p><img src="WhatsApp Image 2025-09-11 at 12.51.43.jpeg"></p>

#### Iteration 3 (Final!)
In the last version:
- Decreased the blade length even further.  
- Gave the blades a slight curved edge for smoother motion.  
- Sanded the whole piece for a clean finish.
<p><img src="WhatsApp Image 2025-09-11 at 12.51.33.jpeg"></p>

https://github.com/user-attachments/assets/24edfe98-5d22-4944-9e8e-d217384ff71d

And *yayy!* my cute little fidget toy was ready to fly.

https://github.com/user-attachments/assets/ad9a2e65-1eec-4ec5-87cb-d4c90dae7514

It fits perfectly on the hand, turns smoothly, and feels like a playful blend of wings and helicopter blades. Here are the 3 genz together!
<p><img src="WhatsApp Image 2025-09-11 at 12.51.32.jpeg"></p>

# Week 2  
## Electronics 🔌 | 09.09.2025 - 16.09.2025 
In Week 2, we followed tutorials in class and were introduced to using an LDR (Light Dependent Resistor) sensor along with an RGB LED (3-in-1). It was exciting to see how the RGB LED could mix colors based on sensor input, opening up creative ways to play with light and interactivity. Later, I experimented on my own with a few variations, trying out different sensor responses and LED patterns, which gave me a better grasp of how analog inputs can control multi-channel outputs.

### Classwork
1. RGB LED (3-in-1)

https://github.com/user-attachments/assets/e6ed1c32-4381-49e1-b8bb-3d1a6d130027

2. Blinking LEDs in intervals / patterns


https://github.com/user-attachments/assets/7ff346b7-fb1f-41c0-9aed-614b1199ccff

https://github.com/user-attachments/assets/e8a3721f-9686-4974-af95-b619fdc6b610



### Experiments

1. Learned how to capture values from the LDR sensor and view them through the Serial Monitor: analogRead()

https://github.com/user-attachments/assets/d3c8dc08-d85d-4d12-b392-993664350c39

2. Experimented with PWM to dim and brighten an LED smoothly: analogWrite()


https://github.com/user-attachments/assets/9f72e960-a1b6-43d2-99b2-f767a83418ff

https://github.com/user-attachments/assets/79ec3b90-d784-4a1b-95d2-589550d2df2a


3. Connected the LDR sensor with an LED so that the light intensity controlled the LED state.


https://github.com/user-attachments/assets/e4e4e5bf-0841-440a-85ad-22b36de0d72c


4. Added a button for manual control and experimented with simple on/off states.


https://github.com/user-attachments/assets/4f97f130-ed0d-490d-92b0-0558d0a0635e


5. Used a potentiometer to vary LED brightness and understand analog input scaling.


https://github.com/user-attachments/assets/2c30ec93-b305-4a25-86b1-91ffb42f3fb8

## Digital Fabrication 🛠️ | 11.09.2025 - 18.09.2025

In the second week, we moved from 2D to 3D by learning Fusion 360. This was my very first time using the software, so it took some time to get comfortable, but it opened up new ways to think about form and structure.

### Assignment

We had two assignments this week.

1. Recreate the personality ring in 3D — I modified my helicopter blades slightly, and once printed, the ring spun so smoothly.
![WhatsApp Image 2025-09-18 at 10 13 27 (1)](https://github.com/user-attachments/assets/9fb2a80c-a07e-409f-963e-1a70f7263454)
![WhatsApp Image 2025-09-18 at 10 13 21](https://github.com/user-attachments/assets/8d1b58e7-2147-4fca-88c1-3c98afa033d1)

https://github.com/user-attachments/assets/b9a7dd8b-e348-4536-99c1-46e18e205e96

2. Create a new design — I started working on an ambigram structure that reads “meg” from one side and “fly” from the other. I’ve created a base for it and am yet to mount and test how it works.

![WhatsApp Image 2025-09-18 at 10 13 27](https://github.com/user-attachments/assets/86ebcfb5-c5ad-40bb-96f5-5d1c7fba54d2)

https://github.com/user-attachments/assets/3bd30e7d-6c98-40b8-adfb-f4b97a256522

![WhatsApp Image 2025-09-18 at 22 59 04](https://github.com/user-attachments/assets/4eed6b14-d018-4d4d-8da4-83aa697f0468)
![WhatsApp Image 2025-09-18 at 22 59 05](https://github.com/user-attachments/assets/e0e1af93-c555-4a8e-848f-0fca3576440d)
![WhatsApp Image 2025-09-18 at 22 59 05 (1)](https://github.com/user-attachments/assets/d2f0f922-eba6-41fb-a4bf-b095c13248ac)


# Week 3  

## Electronics 🔌+ Digital Fabrication 🛠️ | 16.09.2025 - 18.09.2025 

In class this week, we learned how to use a servo motor. First, I made it move back and forth on its own with a simple program. Then, we connected a knob (potentiometer) so that turning it could change the angle of the servo. It was fun to see how something I controlled by hand could directly move the motor showing how inputs and outputs can work together.

```
#include <Servo.h>

Servo myservo;

void setup() {
  myservo.attach(9);  // servo signal on pin 9
}

void loop() {
  // sweep from 0 to 180
  for (int pos = 0; pos <= 180; pos++) {
    myservo.write(pos);
    delay(15);   // adjust for speed
  }

  // sweep back from 180 to 0
  for (int pos = 180; pos >= 0; pos--) {
    myservo.write(pos);
    delay(15);
  }
}
```

https://github.com/user-attachments/assets/ac7a2274-ae0c-405d-85aa-ca5c4ed82329
 
https://github.com/user-attachments/assets/efdd251c-7e68-4dd2-b1f7-be9ed6a7600a

We were also introduced to our project brief on emotive origami. In class, we practiced a few simple folds with paper and cardboard, and were shown some example videos of what’s possible. For my first test, I tried folding a flying bird to check the quality of the paper I chose and to see how much motion I could create. This was my starting point for exploring how movement and form can work together.

![PXL_20250920_163121741 MP](https://github.com/user-attachments/assets/3aa87399-844c-40cb-bdc0-814be96d79e7)

https://github.com/user-attachments/assets/02bce0e5-5dd9-4138-839d-b806a62c3ca9

# Week 4  

## Electronics 🔌 + Digital Fabrication 🛠️| 18.09.2025 - 25.09.2025 

### Process

For the project, I began by exploring a few origami folds, using reference books and YouTube tutorials for guidance. I eventually chose the hyperbolic paraboloid, which has both a personal and technical significance for me. It connects back to the Param science center, a building I worked on earlier and still hold close to my heart. Mathematically, it’s a fascinating form where strength comes from geometry rather than mass, making it a sustainable and efficient structure.
![PXL_20250920_190441859 MP](https://github.com/user-attachments/assets/309a77d6-fd72-4b58-89e0-32d715a56ede)
![PXL_20250922_234249056 MP](https://github.com/user-attachments/assets/d070a2c5-518d-4afc-b5c2-fd6bc587941e)
![PXL_20250923_033931478 MP](https://github.com/user-attachments/assets/b8222e99-bd7f-4ab3-b871-d7750728d86f)

https://github.com/user-attachments/assets/e4fe48b1-13bd-4408-82ba-4066547ed957


I first folded paper models to understand the geometry and then started thinking about how to animate the form. My initial idea was to create a two-way 180° twisting motion, but after sketches and discussions with Cody and Chris, I realized it would be mechanically complex. I then shifted the idea to a horizontal sliding motion along the X-axis.

![ideation sketch 1](https://github.com/user-attachments/assets/18c8f3a3-9d5b-422a-990b-8274cc566e14)
![ideation sketch 2](https://github.com/user-attachments/assets/e0a60355-57d0-4465-b305-7332c6263323)

Below are the 2 other motions that I tried out before arriving at the final one.

https://github.com/user-attachments/assets/e1e9191b-a7a5-4f68-8bfe-6734769323d4

https://github.com/user-attachments/assets/320bb984-ce6a-4a3b-a6b4-20198a427858

### Iterations

Rack & Pinion Setup – With Lauryn’s suggestion, I tried using a rack and pinion to move the piece. I 3D-printed a set and attempted to mesh it with the motor. Nikhil helped me out with this!
![PXL_20250924_055455343](https://github.com/user-attachments/assets/20d5e026-7ce8-4617-ab93-bf22f255e47b)
![PXL_20250924_033406082](https://github.com/user-attachments/assets/7058a90e-1e2a-4a1f-8f46-3ec948bca196)

https://github.com/user-attachments/assets/c8b03078-6c7e-4f21-907e-a0d6de007831

Materials - For prototyping, I used simple materials like pens, paper clips, and scrap laser-cut circles to quickly test connections and motions before moving to sturdier setups.
Once the idea felt promising, I mounted the system inside a cardboard box, cutting a diagonal slit to hold the form. Two bamboo skewers were attached to adjacent sides of the shape—one fixed inside the box and the other connected to the rack—so that only one side would move.

https://github.com/user-attachments/assets/75c09a88-2f78-4cb1-bc2b-aba8e85fff56

Guiding Tracks – The rack kept slipping, so I added two wooden sticks as rails to keep the motion straight.
![PXL_20250925_162652009](https://github.com/user-attachments/assets/a93ea983-1925-4414-925e-7cd35829956d)
Final Working Model – With some duct tape fixes and funny little add-ons, I managed to get the piece moving smoothly.

https://github.com/user-attachments/assets/4cd7ae23-b1fd-4910-b1b2-853d89f97b4a

Bloopers from the late night studios!
![PXL_20250924_205159963](https://github.com/user-attachments/assets/e695739c-e3f1-42a5-b8c0-5d1f117a1ed8)

### Challenges & Learnings

- The first challenge was purely mechanical—getting the motion smooth and consistent.
- Simple adjustments (like slits, tape, or skewers) can make the difference between a stuck system and one that moves smoothly.
- The next challenge came from the coding side. The sweep code and LDR sensor code didn’t seem to work together, and the serial monitor kept showing a value of 0.
- Eventually, I used ChatGPT to generate an alternative code, which worked. Roopa helped me out with this! That moment of seeing the mechanism finally move felt amazing.
- Coding is never one-and-done; debugging is part of the process, and exploring alternative solutions often opens up new directions.

### Final Outcome 

Circuit Diagram

![circuit diagram](https://github.com/user-attachments/assets/395bc1d1-9ae7-4fba-bb9d-571d718e287b)

Process Diagram
![process diagram](https://github.com/user-attachments/assets/6f71c40d-2878-4062-9e6f-7fa6f1477650)

```
#include <Servo.h>

#define TRIG_PIN 11
#define ECHO_PIN 12

Servo myservo;
long duration;
int distance;
int pos = 0;

void setup() {
  Serial.begin(9600);
  pinMode(TRIG_PIN, OUTPUT);
  pinMode(ECHO_PIN, INPUT);
  myservo.attach(9);  // servo on pin 9
}

void loop() {
  // --- Trigger the ultrasonic pulse ---
  digitalWrite(TRIG_PIN, LOW);
  delayMicroseconds(2);
  digitalWrite(TRIG_PIN, HIGH);
  delayMicroseconds(10);
  digitalWrite(TRIG_PIN, LOW);

  // --- Measure echo pulse ---
  duration = pulseIn(ECHO_PIN, HIGH, 60000); // timeout 60ms
  distance = duration * 0.034 / 2;           // convert to cm

  Serial.print("Distance: ");
  Serial.print(distance);
  Serial.println(" cm");

  // --- Check condition ---
  if (distance > 0 && distance < 10) {
    // sweep servo from 0° → 180° → 0°
    for (pos = 0; pos <= 180; pos += 1) {
      myservo.write(pos);
      delay(15);
    }
    for (pos = 180; pos >= 0; pos -= 1) {
      myservo.write(pos);
      delay(15);
    }
  }

  delay(500); // wait before next reading
}
```

### Reflections
Presenting the working prototype in class, especially with the golden hour shots, was rewarding—it felt like my first proper breakthrough in this project.

https://github.com/user-attachments/assets/5ac4b307-0ca4-4e50-b4bf-8da490913de1

![PXL_20250926_001851614 MP](https://github.com/user-attachments/assets/e0063d49-27d9-4931-8485-f530a291aeb6)

https://github.com/user-attachments/assets/ac54ac85-e233-4e25-b6e1-35feb3123039

While this prototype gave me the satisfaction of solving mechanical and coding issues, I still feel drawn to my initial idea of creating a full motion. I want to revisit that direction in future iterations, exploring a more natural and expressive movement. This week showed me the joy of “making it work,” but I also want to push myself!

# Week 6
# 28.09.2025 - 04.10.2025
### Overview
This week, we were introduced to our next project — Expressive Mechanics. The goal was to design a kinetic mechanism that could interact with camera input, making it responsive and expressive through movement. It was an exciting shift, blending physical motion with digital sensing.
## Electronics 🔌
This week’s electronics sessions introduced us to open programming and p5.js — both completely new to me. I started experimenting in class, playing around with some simple sketches and creating a few cute illustrations.

https://github.com/user-attachments/assets/7e75d41f-cfca-45ed-a201-195a26d48f70

![PXL_20251001_011442116 MP](https://github.com/user-attachments/assets/7bedb0c4-e525-4a87-84ac-9b5f151fc02b)

https://github.com/user-attachments/assets/8e9a44b2-6f26-4bd0-90b0-f71cabe7c4a7

We also learned how to integrate a potentiometer with p5.js and serial communication, making physical input control digital visuals. It was quite interesting to see how turning a small knob could bring motion and interactivity to the screen.

https://github.com/user-attachments/assets/3524af56-ce84-4e64-a1d0-57aeee1c1d08

## Digital Fabrication 🛠️

I was inspired by some of the examples shown in class but wanted to understand the process by building something from scratch rather than replicating existing designs.
![PXL_20251001_012030688 MP](https://github.com/user-attachments/assets/97fe6714-b5ad-4dbc-bcde-b9adbeb011ab)
![PXL_20251001_011911773 MP](https://github.com/user-attachments/assets/8f594a7d-eab8-419f-b193-44ece0112577)

I began by 3D printing a cam mechanism found online to study how the parts interact, but the attempt wasn’t successful — the components fused together due to adhesive issues and couldn’t move as intended. It was a useful learning experience in understanding tolerances and assembly techniques.
![PXL_20251004_175119554 MP](https://github.com/user-attachments/assets/00d18c47-15a5-4b3e-bab1-85c5cbe5317c)
![PXL_20251003_154824508 MP](https://github.com/user-attachments/assets/6d3fefc3-7aea-427c-abf4-92e8bcf83deb)
![PXL_20251003_021008848 MP](https://github.com/user-attachments/assets/43f9ce9c-d5a2-4e9d-89c0-def38b6643d4)

After that, I decided to explore the umbrella mechanism, intrigued by its simple yet effective motion. I studied a few reference videos and began designing a laser-cut version. I found and 3D printed a few versions of a six-connector hub to test with quarter-inch dowels available in the studio, but the fittings didn’t align properly. I plan to refine these connections and continue developing the system next week.

Reference Video Link : https://www.youtube.com/shorts/FFWDxpNXd2E
![PXL_20251006_210953134 MP](https://github.com/user-attachments/assets/6c01286b-5909-4908-bc53-21d05d6dffdd)

# Week 7
# 05.10.2025 - 11.10.2025
## Overview ☂️
By this week, I had a clear idea of what I wanted to accomplishm, a linkage mechanism that opens and closes in the air like an umbrella, held together at the center by a rod. The setup involved two hubs: one fixed at the top of the stick and another movable one that would slide along it.
The concept was to create an interactive system where the default state on screen shows a bright, daylight scene. When the camera detects a person’s face, a rain animation would play, simultaneously triggering the umbrella mechanism to open, symbolizing the connection between human presence and environmental change.

## Digital Fabrication 🛠️
I focused on laser-cutting and prototyping the linkage arms and hinge mechanism. I began by sketching and testing the geometry in Illustrator, then iterated through three rounds of laser cutting to achieve the correct lengths and motion range.
![PXL_20251006_220430589 MP](https://github.com/user-attachments/assets/68657b9b-b7ff-4c6e-8b59-35ce41258330)
![PXL_20251007_003956083 MP](https://github.com/user-attachments/assets/23d2b992-8412-42e5-9bb1-8023227ed24e)

I made six sets of linkages and assembled them, keeping the system modular really helped during testing. In parallel, I also laser-cut a box structure to support the mechanism and keep it upright during assembly and testing.


https://github.com/user-attachments/assets/bffcd69d-104b-4a13-89a2-922d142a303a
https://github.com/user-attachments/assets/ee66e950-3e75-43df-a2ec-989e59a7c697
![PXL_20251006_224919826 MP](https://github.com/user-attachments/assets/db4fe387-bf60-4dd5-bc05-38e4ffd3602a)
![PXL_20251007_153344184 MP](https://github.com/user-attachments/assets/6bf94df3-6b83-422f-ae99-a694b06a5611)

Soon, I realized that the hub needed to be designed precisely for my setup rather than using a generic one from online sources. So, I modeled it in Fusion 360. 
  
![PXL_20251006_235007879](https://github.com/user-attachments/assets/673237c8-c4b9-4d85-bde8-698afac5b0c1)
![PXL_20251008_025722609 MP](https://github.com/user-attachments/assets/49574a71-7e50-4521-a9ba-53ea73ecf7cd)
![PXL_20251008_200014261 MP](https://github.com/user-attachments/assets/ce7f0d38-718f-4f8f-ac64-df8e61a3e7f9)

But of course, the first print didn’t go as planned — I hadn’t accounted for 3D printing shrinkage, so the center hole wasn’t wide enough. To make things worse, the screw holes on the sides didn’t align with the laser-cut linkages (another silly mistake!). After some advice and help from a friend, I redesigned the part more accurately, and finally, on the third 3D print, it worked perfectly. With a little sanding on the rod (thanks to Chris’s tip on how to smooth it properly), the hub fit beautifully, and the mechanism started functioning as intended.

![PXL_20251008_070320744 MP](https://github.com/user-attachments/assets/8e60bd6c-4590-479f-b74f-1dc0f7b05ecd)

https://github.com/user-attachments/assets/b34c0f4c-b43b-492f-8981-fa94ac0023fb

![PXL_20251008_065638586 MP](https://github.com/user-attachments/assets/0f399d4e-e020-4837-8205-b67f7c070073)

At this stage, I hadn’t yet considered the motor aspect, which I now realize I should have planned earlier. I decided to use a servo with a rack-and-pinion setup, similar to my first project — but this time with stronger rails and better fixtures. Unfortunately, I hadn’t designed it specifically for this setup, which led to several challenges with gear alignment and keeping the system stable at a consistent height. A frustrating but valuable learning experience.
![PXL_20251009_033414482 MP](https://github.com/user-attachments/assets/5944e065-0451-4b9c-a7ba-473f064eab4e)
![PXL_20251009_033036670 MP](https://github.com/user-attachments/assets/997c9a08-f576-4564-8817-9860b1740659)
![PXL_20251009_001859123 MP](https://github.com/user-attachments/assets/a0cc8ac3-786b-4566-aad1-a83508a248b8)

## Electronics 🔌
For the electronics part of this project, I used a servo motor connected to a gear to drive the umbrella’s motion. Initially, I used the base code shared by Prof Sudhu, but I struggled for quite some time because I was running it in a different p5.js link. Only later did I realize that the library HTML files were preloaded in his link, which is why the code worked there and not in mine. Lesson learned.

After sorting that out, I used ChatGPT to write a few variations of the code and animation. In the first version, the system reacted backward, it started raining when I moved far away and turned into daylight when I came closer. Fixing this logic took a bit of tweaking.

https://github.com/user-attachments/assets/9b57af1d-86f4-4a16-a96e-a202a2712da2

Then came another issue: the servo motor was moving abruptly from 0° to 180° instead of transitioning smoothly. Adjusting the motion speed and delay finally made the umbrella open gracefully.

https://github.com/user-attachments/assets/dedc0197-cff3-4ab2-8926-d64632c2b5c3

For the final setup, I added a cute animation of a person walking with a stick (representing the umbrella). When someone comes close to the screen, it starts raining, and the person on screen raises the stick — mimicking the action of opening an umbrella, which simultaneously triggers the real kinetic umbrella mechanism behind the laptop.\

https://github.com/user-attachments/assets/1d2a3fcb-0331-4fba-b358-c4b1c02f53e8


### p5.js code
https://editor.p5js.org/loopstick/sketches/MWZxoSNoP

### Arduino code
```
#include <Servo.h>

Servo myServo;
int servoPin = 7;

int currentAngle = 0;   // current servo position
int targetAngle = 0;    // target position received from p5.js
int stepDelay = 10;     // delay in ms between small steps

void setup() {
  Serial.begin(115200);
  myServo.attach(servoPin);
  myServo.write(currentAngle);  // start at 0° (daylight)
}

void loop() {
  // Check for serial input
  if (Serial.available() > 0) {
    int angle = Serial.parseInt();
    if (angle >= 0 && angle <= 180) {
      targetAngle = angle;  // update target
      Serial.print("Target angle set to: ");
      Serial.println(targetAngle);
    }
    // Clear leftover serial bytes
    while (Serial.available() > 0) {
      Serial.read();
    }
  }

  // Smooth transition to target
  if (currentAngle < targetAngle) {
    currentAngle++;
    myServo.write(currentAngle);
    delay(stepDelay);
  } 
  else if (currentAngle > targetAngle) {
    currentAngle--;
    myServo.write(currentAngle);
    delay(stepDelay);
  }
}
```

### System Architecture Diagram
![sys_arch diagram](https://github.com/user-attachments/assets/b02f4000-f3c1-48a2-9013-3333b4850d24)

### Mechanical Linkage Diagram
![mech linkage diagram](https://github.com/user-attachments/assets/f876fa41-f387-4b5d-906c-01d5ddc709b1)

### Camera Input Diagram
![camera input](https://github.com/user-attachments/assets/804ddcc4-a9ea-401d-80a4-61bfdb3ec213)

## Reflection 💭

Keeping the setup modular turned out to be extremely helpful — it allowed me to troubleshoot one part at a time. Working with a simple mechanism but refining it thoroughly taught me the importance of precision over complexity.
![PXL_20251009_214840186 MP](https://github.com/user-attachments/assets/210df4e8-6d87-458a-bd7a-38d71194a5fd)

If I were to redo this project, I’d spend more time designing each part to fit together precisely, instead of relying on tape or glue for quick fixes — they’re very ad hoc and end up wasting time. Overall, this project helped me better understand how to link physical and digital motion meaningfully. Also the aspect of storytelling worked out well!

![PXL_20251010_181224890](https://github.com/user-attachments/assets/fd690b94-cf5d-46bb-ac07-72aa6b2b77c3)
![PXL_20251010_190608392 MP](https://github.com/user-attachments/assets/04e83896-12f4-4132-b6ec-c1dc74668237)

https://github.com/user-attachments/assets/de685112-5d46-4572-a77b-ce241ee6c8be

# Week 8
# 12.10.2025 - 18.10.2025
## Overview 
This week, we were introduced to the Ambient Display Project, which focuses on creating subtle, interactive displays that respond to environmental or personal data. In class, we saw several examples of quick 3D printing prototypes and other tangible interfaces that helped us understand the potential for merging physical and digital interactions.
![PXL_20251017_005721115 MP](https://github.com/user-attachments/assets/a8525e9d-d433-4f10-b0c6-bc02588585a4)

### Hardware Exercise: ESP32 & Soldering

For our project, we decided to use the ESP32 microcontroller to connect our display to an API. This required soldering the components, which was a great hands-on exercise in preparing our hardware for real-time data communication. I also made a tiny mistake by cutting off one extra pin from the long row we received hence had to add a last pin manually.
![PXL_20251015_213946425 MP](https://github.com/user-attachments/assets/c37274bd-3d23-40c9-a956-9d324b757881)
![PXL_20251015_213944195 MP](https://github.com/user-attachments/assets/d80fb408-92e7-4539-a950-bc4f9429c94a)
![PXL_20251015_214341434 MP](https://github.com/user-attachments/assets/58979117-5ead-40b3-8595-121d5ce6b4d3)

### Assignment: Getting the Onboard NeoPixel Working

As part of the weekly assignment, we had to get the onboard NeoPixel on the ESP32 working using live weather data from Jacobs. Thanks to Roopa’s awesome tutorial, I was able to:

- Connect the ESP32 to the API and fetch real-time weather data
- Program the onboard NeoPixel to display colors corresponding to different weather conditions

This exercise was really helpful for understanding how data can be translated into visual and ambient feedback.


https://github.com/user-attachments/assets/e19ddcee-45c5-47af-a1fb-5a79871ffefb

![PXL_20251024_012630775 MP](https://github.com/user-attachments/assets/02748086-799f-4ac2-9924-fed0a984fba1)

https://github.com/user-attachments/assets/79f17661-65a7-40cd-b0e1-f830626d0ea4


### Concept Development

I started brainstorming ideas with my teammate Edna, focusing on the theme of overstimulation and calming routines. We explored concepts that could:

- Visualize the process of overstimulation throughout the day
- Provide a wind-down experience at the beginning and end of the day

Our goal is to create an ambient display that subtly guides the user’s emotional and sensory experience at different points in the day. Here are some initial sketches from our discussions.

![IMG_7397](https://github.com/user-attachments/assets/6d9f1b4e-b089-42e4-9c06-809510744040)
![PXL_20251018_013539633 MP](https://github.com/user-attachments/assets/fc48d74a-aab5-48ae-ad77-772af83b8a58)

# Week 9
# 19.10.2025 - 25.10.2025
## Overview 

After much thought, we decided to move forward with a thread unspooling mechanism. We wanted something simple yet meaningful—a way to represent how a thread unwinds, reminding the person to unwind after a long day or after the overstimulation of digital experiences.
![IMG_7389](https://github.com/user-attachments/assets/4a02bc94-5627-4558-8ee8-94731e125adc)
![IMG_7393](https://github.com/user-attachments/assets/a3dc4d72-b388-4b0f-b2e8-5f0596e0ce29)

https://github.com/user-attachments/assets/0e346440-d98e-4e89-bbf6-b1583a1840ae

### Prototyping

We started by sketching multiple prototype ideas to visualize how the mechanism could function. Once we had a rough concept, we prepared the laser-cut files, assembled the model, and conducted a first manual test to see how the thread unspooled.

![PXL_20251021_173409553 MP](https://github.com/user-attachments/assets/f01fed6c-87fd-4f67-b026-62b6acc628bd)

https://github.com/user-attachments/assets/f0ee95ed-adc2-4708-818d-7a4bdf3a6b02

https://github.com/user-attachments/assets/18fe5af1-8ebf-4280-b1a9-c2f64f623a60

https://github.com/user-attachments/assets/37579928-5871-46f2-a68b-e14eeaf349eb

### Insights and Next Steps

From this first prototype, we realized a few important things about the mechanism. The kind of mechanism we were aiming for required two continuous servo motors:
1. One for the top dowel to spin
2. Another for the bottom disc, which collects the spool, to rotate at the same speed to form a spiral
The synchronized movement of both motors is essential for a smooth, consistent unspooling

With the mechanical concept clarified, we are now planning to explore form designs—considering aesthetics, materials, and how the visual spiral can convey the calming, unwinding experience we want for the user.
![IMG_7415](https://github.com/user-attachments/assets/c4d813c2-637a-404a-af46-7eb6acd40250)
![PXL_20251023_055725398 MP](https://github.com/user-attachments/assets/0e62899d-dc25-4941-9257-692752df5f6b)

### API Triggers

We decided to use sunset and sunrise as the perfect API calls for this project as these are the best times of the day to put you in a calm mood, and we might even sync it with a few different time zones to see how the ambient effect changes across contexts. We used this to trigger the onboard NeoPixel on the ESP32. This experiment helped us explore how the device could respond to daily natural cycles, tying back to our theme of winding down at the start and end of the day.

![PXL_20251024_012630775 MP](https://github.com/user-attachments/assets/f32ae00c-ab6c-46da-99b9-77a4939bfa5f)

https://github.com/user-attachments/assets/e60ba91e-7a45-432e-8b78-8bab7999a45e

### Form Exploration & 3D Printing

We began 3D printing the form we had sketched earlier using white PLA. The idea was to start shaping the physical structure that would hold our mechanism and electronics while maintaining a clean, minimal aesthetic. We printed a few initial parts, including:

1. The frame, which supports the entire setup
2. The bowl, where we planned to set up all our electronic components
3. A disc on top, where the unspooled thread would gently fall and form patterns
![PXL_20251024_023443513 MP](https://github.com/user-attachments/assets/72914bb8-170e-43f7-b90a-32cbd389cbdf)
![IMG_7435](https://github.com/user-attachments/assets/06b659eb-0295-48f6-bcd4-81ebaf6cb625)
![IMG_7438](https://github.com/user-attachments/assets/2c5486e2-8d0c-4aa0-9905-7e55a8d028b7)
![IMG_7432](https://github.com/user-attachments/assets/bf377504-6615-43c1-86f4-7da9a0b74815)
![IMG_7441](https://github.com/user-attachments/assets/82f89747-b536-44f4-bd8a-17f0416e3d07)
![IMG_7512](https://github.com/user-attachments/assets/a142946b-661f-481b-b78c-9d50ba21ff30)

### Mechanism Testing with Gears

Alongside printing, we also laser cut some gears to quickly test if two interlocking gears could create a smooth rotational motion. In this setup:

- One gear connects to a servo motor mounted vertically at the bottom of the bowl
- This gear touches another gear connected to a dowel, mounted at the center of the bowl’s base
- As the servo rotates, it drives the second gear, causing the dowel to spin, which in turn would rotate the disc on top
![IMG_7513](https://github.com/user-attachments/assets/f6a999c8-6068-4388-a4d2-bf1e65a477d7)
![IMG_7443](https://github.com/user-attachments/assets/365865d1-c60f-4010-8d8a-93ae92c86189)
![IMG_7444](https://github.com/user-attachments/assets/6157c644-e737-4632-b5a2-791a03214d0d)

https://github.com/user-attachments/assets/03ace71e-bcf5-4fe3-a253-17932377d706
![IMG_7521](https://github.com/user-attachments/assets/874f625d-6f9a-40e3-959b-dbefd45bf6ce)

https://github.com/user-attachments/assets/6c43b2e3-d96f-4052-852c-f162f474c7c8

This test helped us understand how we could translate the servo’s motion into a stable, synchronized rotation for the unspooling mechanism.

### Soldering the NeoPixel

We also spent some time soldering the NeoPixel, using the helping hands tool to keep everything steady while making clean connections. After soldering, we tested the circuit, and it worked perfectly.
To create the right mood for our ambient display, we used ChatGPT to generate code that would produce a soft sunrise glow a light yellow-to-bright orange gradient that subtly shifts in intensity, reflecting the calm and warmth of morning light.
![PXL_20251025_184918742 MP](https://github.com/user-attachments/assets/024ba36c-f61b-4404-a5b5-c275f78bd802)

https://github.com/user-attachments/assets/2d30b1a6-6a7c-46c6-adea-7a80edf982a1

# Week 10
# 26.10.2025 - 01.11.2025
## Overview 

This week marked the final stretch of our Ambient Display project. We focused on refining all our printed components, integrating electronics neatly, and making sure the final setup worked seamlessly. Many small details that were missing or misfitted in earlier prototypes had to be corrected — including supports, servo fitting dimensions, and wiring routes.

### Refining the 3D Form

In our previous prototype, we realized which parts needed adjustments. We fixed those dimensional errors, added mounting holes, and reprinted the necessary components. The frame was updated to include a pocket for the servo, allowing it to sit securely inside the structure. The disc on top was also modified with holes for screws and wire routing.
![IMG_7558](https://github.com/user-attachments/assets/ee4574df-19d8-4ffc-a740-c8e4a913c5bb)
![IMG_7560](https://github.com/user-attachments/assets/f1717016-bd7e-4f1e-84c9-5441497ae34e)
![IMG_7562](https://github.com/user-attachments/assets/a2041b73-0cdd-4753-a41e-a3f7ee41e0c3)
![IMG_7583](https://github.com/user-attachments/assets/08a8b7fd-d1be-4a71-bbcd-d25fc3c9248f)

https://github.com/user-attachments/assets/c8c2ae1c-a95d-4f04-84e1-143f333fa9c8

### Moving to ESP32 Integration

Up until this point, we had been using the Arduino to test and control the servos. This week, we transitioned everything to the ESP32, allowing us to power and control all components from a single board. This made the setup more compact, reliable, and network-ready for API integration.
![IMG_7595](https://github.com/user-attachments/assets/6cdbf23e-e133-4f15-a803-678702cf587a)
![IMG_7596](https://github.com/user-attachments/assets/d0dd66dc-785c-4c92-8b80-0fb6c4510f38)


### NeoPixel Setup & Color Logic

We decided to replace the NeoPixel stick with a RGB LED NeoPixel strip, which gave a softer and cleaner lighting effect inside the circular disc. Using this setup, we programmed two color transitions:

- Sunrise: light yellow → warm yellow → bright golden orange

- Sunset: warm yellow → orange → pink → deep purple

These color transitions represent daily rhythms—helping users wind up and wind down in sync with natural light cycles.
![IMG_7586](https://github.com/user-attachments/assets/df3c3757-bee6-4d07-bcaf-dc0f4092b415)

https://github.com/user-attachments/assets/0ec1f46a-17a5-40dd-9ce2-d65b2ccfa966

https://github.com/user-attachments/assets/fefcfdc1-011e-49c3-976e-91326f1b44d9

https://github.com/user-attachments/assets/084f15ba-242c-431b-a6ba-4c2600e38926

### Final Testing at the Bus Stop (Yes, Really!)

For our final prototype test, we decided to have a bit of fun and ran it at the bus stop because we were too late , tapping into the sunset time of Honolulu via API. The system worked perfectly — both servos triggered in sync, the lights responded to the real-time API call, and the full ambient experience came to life.
![IMG_7602](https://github.com/user-attachments/assets/7a088e9e-d796-4573-8d75-61ba6d691b40)


### Final Product

Our Ambient Display is finally complete — a poetic reminder to unwind at the beginning and end of each day. It can even be synced with multiple time zones, connecting users to places close to their heart or home.

- The servo motors rotate clockwise to unwind the thread and anticlockwise to coil it back up.

- This motion repeats gently over the course of five minutes, aligning with sunrise and sunset durations.

- The light transitions add a calming, atmospheric layer to the interaction.

https://github.com/user-attachments/assets/f0eff56e-e7e1-47d2-8159-a993ee9b2b47

https://github.com/user-attachments/assets/bbc6a605-7310-4299-af58-2c9956476c48

### Data Flow Diagram
![Copy of Blank board](https://github.com/user-attachments/assets/184baf47-cde0-4865-8251-dfce013ffdd2)

### Hardware Architecture Diagram

![Copy of Blank board (1)](https://github.com/user-attachments/assets/13f13aec-2a95-4528-b202-cbeff0db3cf1)


### Reflections & Learnings

This project was a huge learning experience — technically, creatively, and collaboratively.

#### What worked well:

- Early testing of individual components made it easier to assemble everything later.

- Collaborating with a partner (Edna!) helped in sharing ideas and problem-solving.

- Seeing all new components — servos, ESP32, NeoPixel, API calls — come together smoothly was incredibly rewarding.

#### What could improve:

- Exploring different types of threads could make the unspooling mechanism smoother, as it occasionally got stuck.

- Further form refinement could make the product more cohesive.

- I realized the need to upskill in certain software tools for faster prototyping and iteration.

- Clearer communication and schedule alignment in teamwork would help streamline the process even more.

Overall, this project was a blend of learning, fun, and experimentation, and it beautifully captured the spirit of creating something subtle yet meaningful — an object that reminds us to pause, breathe, and unwind.

![IMG_7645](https://github.com/user-attachments/assets/8dfa40fe-2e03-4f4c-be5a-7d26319c488c)

# Week 11
# 02.11.2025 - 09.11.2025
## Overview 

This week we teamed up and started working towards our final project. A tangible, poetic system for emotional connection across space.

ELO explores how touch, movement, and subtle haptic cues can connect people across long distances—without screens, digital messaging, or spoken communication. Instead of notifications or sound, ELO creates a soft, embodied language of emotion through gentle vibration patterns and expressive motion.

The system consists of paired objects.
When one person interacts with their device—through a touch, press, hold, or approach—the paired object elsewhere responds with slow kinetic movement or haptic feedback, offering a wordless reminder of presence.

### Goals
- Build an emotionally expressive system using haptic feedback and gentle motion
- Translate human gestures into poetic, sensory responses
- Create a non-screen-based method of long-distance connection
- Develop a shared tactile “language” that conveys comfort, calm, or presence

### Core Components

- Tactile Inputs: touch, press, squeeze
- Presence Inputs: short-range proximity detection
- Feedback: vibration patterns, kinetic movement
- Internal Mechanisms: custom gears, soft actuators
- Paired Devices: exchanging physical gestures through simple wireless communication
- Interaction Language: mapping gestures → emotional responses

### System Architecture Diagram
![el1](https://github.com/user-attachments/assets/3a176529-1910-4220-bf76-e66fa0230f0b)

### Sequence Diagram
![el2](https://github.com/user-attachments/assets/d0abada0-2169-472a-a01f-2228d5dde14a)

### Form Exploration & Gamification
We explored organic, hand-held forms that feel soft, approachable, and naturally invite touch. Early sketches played with pebble-like and pod-shaped silhouettes that users could cradle, press, or rest their hands on. We also experimented with gamifying the interaction—imagining a small token or pawn that the user moves or places to initiate an emotional action. This allowed the object to feel playful yet intimate, turning gesture into a quiet ritual rather than a button press.

![el3](https://github.com/user-attachments/assets/8b200f40-c2b2-4ab0-a45d-cb91d70284e9)

### Electronics & Communication
We decided to use MQTT as our primary communication protocol. MQTT is a lightweight publish–subscribe messaging system designed for IoT devices, making it perfect for low-power, low-bandwidth interactions. Each device acts as a client that either publishes signals or subscribes to specific topics. A central broker manages this exchange, ensuring that only the intended paired device receives the interaction. This allows our emotional cues to feel instant, synchronized, and reliable across distance.

Underneath this, MQTT relies on TCP (Transmission Control Protocol)—a foundational internet protocol that ensures data arrives in the correct order and without errors. TCP establishes a stable connection, numbers and tracks packets, and retransmits any lost ones, giving us a dependable channel for subtle tactile interactions.

Together, MQTT + TCP provide a stable, low-overhead system that enables two objects to quietly communicate emotional gestures in real time.


https://github.com/user-attachments/assets/3cdc2ed6-f8d2-4aba-8852-62ce00fe7340

https://github.com/user-attachments/assets/677b2346-009a-44e8-8169-043cb746c0b2

https://github.com/user-attachments/assets/c077b1f6-88aa-4e04-b2e8-b3a13a42cb65

# Week 12
# 10.11.2025 - 17.11.2025
## Overview
This week focused on building the full physical–digital foundation of the project. Mechanically, we explored gear-driven movement with magnets, tested organic form prototypes, and refined tolerances through multiple 3D prints. Electronically, we integrated sensor-based interaction, established device-to-device communication through Berkeley IoT, and tuned the responsiveness of the LDR to create an intentional touch interaction. By the end of the week, both the physical mechanism and the communication pipeline were functioning together in early prototypes.

### Digital Fabrication 
#### Gear Mechanism Prototyping

* Designed and 3D-printed a conical gear pair to allow smooth perpendicular rotation.
* The small conical gear attaches to the servo; the larger gear receives the motion.
* Printed multiple iterations to test mesh alignment, flexibility, and friction.
* Established a stable rotation system that will translate sensor input into gentle movement.
* Added magnets into the gears to achieve the desired effect.
<img width="864" height="721" alt="image" src="https://github.com/user-attachments/assets/f63bb584-1c61-411e-a7a2-62be34bb649c" />
<img width="960" height="720" alt="image" src="https://github.com/user-attachments/assets/cad41e6e-14b5-47c7-8ce4-5e7d7fbbba0d" />

#### Organic Form Development
* 3D-printed shell prototypes to test material flexibility + comfort in hand.
* Ensured the form could house: entire gear mechanism, servo + mount, wiring + sensors, ESP32
* Adjusted wall thickness and interior supports based on test prints.

#### Structural Integration
* Printed early “test shells” to ensure internal components fit cleanly.
* Checked alignment between form, gears, and sensor locations.

### Electronics & Communication 

#### Sensor Interaction (LDR Touch Input)
* Integrated an LDR sensor as the main input for intimate, intentional interaction.
* Original threshold (2500) caused false triggers.
* Tuned input threshold down to 1000, activating only when a finger touches the LDR.
* Enabled soft “touch → movement” behavior.

#### ESP32 Device-to-Device Communication
* Each ESP32 has a unique MAC address, requiring separate login credentials.
* Registered both devices individually on Berkeley IoT, using two different passwords.
* Established reliable communication between paired devices.
* Enabled “emotion trigger → remote kinetic response” behavior.

#### System Integration

Tested real-time communication between:
* LDR sensor → ESP32 sender
* ESP32 receiver → servo + gear motion
Verified that the physical motion activates only on intentional touch events.

# Week 13
# 18.11.2025 - 25.11.2025
## Overview


# Week 14
# 26.11.2025 - 03.12.2025
## Overview


# Week 15
# 04.12.2025 - 09.12.2025
## Overview











