# CODTECH_task3

"NAME" : LINGAM SREE KEERTHI


"COMPANY" : CODTECH IT SOLUTIONS


"ID" : CT04DF1246


"PROJECT BASED ON" : IOT


"DURATION" : 4 WEEKS


"PROJECT MENTOR" : NEELA SANTOSH


OVERVIEW OF THE PROJECT:

An IoT Security System is a smart surveillance and protection system that uses sensors, cameras, and internet connectivity to monitor and secure homes, offices, or public spaces. It can detect intrusions, send real-time alerts, capture images or video, and allow remote access through smartphones or web apps.
To build an automated security system that:


Detects motion using sensors (e.g., PIR sensor),

Captures images using a camera (e.g., webcam or Pi camera),

Sends instant alerts (via email, buzzer, or app notification).


COMPONENTS:

Arduino Uno

PIR motion sensor

LED (to simulate “capture” indicator)

220 Ω resistor

Breadboard & wires



#CODE USING TINKERCAD

const int pirPin = 2;
const int ledPin = 13;

void setup() {
  pinMode(pirPin, INPUT);
  pinMode(ledPin, OUTPUT);
  Serial.begin(9600);
}

void loop() {
  bool motion = digitalRead(pirPin);
  if (motion) {
    digitalWrite(ledPin, HIGH);
    Serial.println("Motion detected! Capturing image...");
    delay(1000);  // simulate snapshot delay
    Serial.println("💾 Image captured and alert sent!");
  } else {
    digitalWrite(ledPin, LOW);
  }
  delay(100);  // reduce CPU usage
}

OUTPUT ROUGH DESIGN


https://github.com/SreeKeerthi05/CODTECH_task3/issues/1#issue-3187613519
