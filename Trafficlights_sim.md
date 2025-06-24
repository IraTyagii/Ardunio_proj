# Traffic lights simulator

### I've made my first simulator using arduino , and used this code on arduino software

In this the green led will first blink for 5 seconds followed by yellow for 2 seconds and then by red for 5 seconds and this continues in a loop
```cpp
const int redLED = 2;
const int yellowLED = 3;
const int greenLED = 4;

void setup() {
  pinMode(redLED, OUTPUT);
  pinMode(yellowLED, OUTPUT);
  pinMode(greenLED, OUTPUT);
}

void loop() {
  // Green light ON for 5 sec
  digitalWrite(greenLED, HIGH);
  digitalWrite(yellowLED, LOW);
  digitalWrite(redLED, LOW);
  delay(5000);

  // Yellow light ON for 2 sec
  digitalWrite(greenLED, LOW);
  digitalWrite(yellowLED, HIGH);
  digitalWrite(redLED, LOW);
  delay(2000);

  // Red light ON for 5 sec
  digitalWrite(greenLED, LOW);
  digitalWrite(yellowLED, LOW);
  digitalWrite(redLED, HIGH);
  delay(5000);
}
```

### I have used :-
| Component        | Quantity |
| ---------------- | -------- |
| Arduino Uno/Nano | 1        |
| Red LED          | 1        |
| Yellow LED       | 1        |
| Green LED        | 1        |
| 220Ω Resistors   | 3        |
| Breadboard       | 1        |
| Jumper Wires     | \~8      |

### Breadboard Connections

| LED Color | Arduino Pin | Resistor | To Breadboard GND |
| --------- | ----------- | -------- | ----------------- |
| Red       | D2          | 220Ω     | Yes               |
| Yellow    | D3          | 220Ω     | Yes               |
| Green     | D4          | 220Ω     | Yes               |


Important:

Connect Arduino's GND pin to the breadboard GND (negative rail).





