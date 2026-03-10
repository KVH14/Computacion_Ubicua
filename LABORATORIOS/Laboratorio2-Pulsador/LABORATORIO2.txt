int PULSADOR = 2;
int LED = 3;
int ESTADO = LOW;

void setup() {
  pinMode(PULSADOR, INPUT_PULLUP);
  pinMode(LED, OUTPUT);
}

void loop() {
  while(digitalRead(PULSADOR) == HIGH) {
  }

  ESTADO = digitalRead(LED);
  digitalWrite(LED, !ESTADO);

  while(digitalRead(PULSADOR) == LOW) {
  }
}