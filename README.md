# TDF Weekly Progress Reports
Hey, I'm Meghana (Megzu) 🌻
I’m maintaining this journal to document my process through the Technology Design Foundation class, which is a mix of electronics and digital fabrication. Very excited to learn, experiment, and do fun stuff along the way!

# Week 1  | 02.09.2025 - 09.09.2025 
## Electronics 🔌
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

**Note:** *GitHub README files don't support embedded video playback. Click the links below to view videos in a new tab.*

📹 **[Task 1 - Arduino Blink Demo](https://github.com/meghanasanjay1204/tdf-fa25-meghana-sanjay/raw/main/task%201.mp4)**

📹 **[Blink Bulb Demo](https://github.com/meghanasanjay1204/tdf-fa25-meghana-sanjay/raw/main/blink%20bulb.mp4)**

📹 **[Blink 2 Bulbs External Pin 8](https://github.com/meghanasanjay1204/tdf-fa25-meghana-sanjay/raw/main/blink%202%20bulbs_ext%208.mp4)**

📹 **[Built-in LED Blink (Pin 13)](https://github.com/meghanasanjay1204/tdf-fa25-meghana-sanjay/raw/main/Blink_13.mp4)**

## Digital Fabrication 🛠️
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
<p><img src="WhatsApp Image 2025-09-11 at 12.51.49.jpeg"></p>

#### Iteration 2
To improve the design:
- Decreased the diameter of the ring for a tighter fit.  
- Added a second ring to stack together for stability.  
- Increased the height of the projection on the ring so the stopper could hold properly.  
- Reduced the length of the blades to make it more wearable.
<p><img src="WhatsApp Image 2025-09-11 at 12.51.43.jpeg"></p>

#### Iteration 3 (Final!)
In the last version:
- Decreased the blade length even further.  
- Gave the blades a slight curved edge for smoother motion.  
- Sanded the whole piece for a clean finish.
<p><img src="WhatsApp Image 2025-09-11 at 12.51.33.jpeg"></p>
📹 **[Spinning Ring Demo](https://github.com/meghanasanjay1204/tdf-fa25-meghana-sanjay/raw/main/WhatsApp%20Video%202025-09-11%20at%2012.51.33.mp4)**

And *yayy!* my cute little fidget toy was ready to fly.  
It fits perfectly on the hand, turns smoothly, and feels like a playful blend of wings and helicopter blades. Here are the 3 genz together!
<p><img src="WhatsApp Image 2025-09-11 at 12.51.32.jpeg"></p>

# Week 2  | 10.09.2025 - 15.09.2025 
## Electronics 🔌
In Week 2, we followed tutorials in class and were introduced to using an LDR (Light Dependent Resistor) sensor along with an RGB LED (3-in-1). It was exciting to see how the RGB LED could mix colors based on sensor input, opening up creative ways to play with light and interactivity. Later, I experimented on my own with a few variations, trying out different sensor responses and LED patterns, which gave me a better grasp of how analog inputs can control multi-channel outputs.

📹 **[RGB LED with LDR Sensor Demo](https://github.com/meghanasanjay1204/tdf-fa25-meghana-sanjay/raw/main/PXL_20250910_020313575.mp4)** 

### Classwork
1. RGB LED (3-in-1)
2. Blinking LEDs in intervals / patterns


add the one light fade in out image/vidz

``` int led = 9; 
int sensorValue = 0;
void setup()
{
  Serial.begin(9600);
  pinMode(led, OUTPUT);  
}
void loop()
{
  sensorValue = analogRead(A0);
  Serial.println(sensorValue);

int ledValue = map(sensorValue, 0, 1023, 0, 255); 
analogWrite(led, ledValue);

delay(200);        
}
```

experimented by chngaging few valeus and adidng 2nd lighy






