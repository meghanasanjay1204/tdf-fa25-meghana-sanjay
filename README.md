# TDF Weekly Progress Reports
## Hey, I'm Meghana (Megzu) 🌻
### I’m maintaining this journal to document my process through the Technology Design Foundation class, which is a mix of electronics and digital fabrication. Very excited to learn, experiment, and do fun stuff along the way!
# Week 1  | 02.09.2025 - 09.09.2025 
## Electronics 🔌
In the first week, we were introduced to the syllabus and the general direction of TDF. I am in the Directed section with Prof. Sudhu Tewari and Chris Mayers, where the emphasis is on creating feasible things over simply visible or desirable ones, a refreshing shift in perspective. We received our toolkits, which was really exciting and made the course feel tangible right from the start. Although I’ve previously overseen projects that involved microcontrollers and electronics. Prof. Tewari also shared useful resources for brushing up on Arduino basics, which I’ve started exploring.
## Resources
https://github.com/loopstick/ArduinoTutorial?tab=readme-ov-file#exercise-2
https://learn.adafruit.com/ladyadas-learn-arduino-lesson-number-0?view=all
## Experiments
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
} ```
3. Built-in + External Blink: Tried to connect both at the same time and it worked.
Blink_13.mp4

## Assignment - Hello World with LED Blinking

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
} ```





