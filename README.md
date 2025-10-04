# TDF Weekly Progress Reports
Hey, I'm Meghana (Megzu) 🌻
I’m maintaining this journal to document my process through the Technology Design Foundation class, which is a mix of electronics and digital fabrication. Very excited to learn, experiment, and do fun stuff along the way!

# Journal Index  

- [Week 1](#week-1)  
- [Week 2](#week-2)  
- [Week 3](#week-3)  
- [Week 4](#week-4)  

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













