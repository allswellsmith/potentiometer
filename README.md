const int potentiometerPin = 4;

void setup() {
  Serial.begin(115200); // Start serial communication at 115200 baud
}

void loop() {
  int value = analogRead(potentiometerPin); // Read analog input from pin 4
  Serial.print("Potentiometer Value: ");
  Serial.println(value); // Print the value to the serial monitor
  delay(1000); // Wait for 1 second before the next reading
}
