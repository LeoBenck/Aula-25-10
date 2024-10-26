# Aula-25-10
Exercício 1:

void setup()
{
  pinMode(LED_BUILTIN, OUTPUT);
}

void loop()
{
  delay(1000);
  digitalWrite(LED_BUILTIN, LOW);
  delay(1000);
  digitalWrite(LED_BUILTIN, HIGH);
}


Exercício 2:

void setup()
{
  pinMode(LED_BUILTIN, OUTPUT);
}

void loop()
{
  delay(1000);
  digitalWrite(LED_BUILTIN, LOW);
  delay(1000);
  digitalWrite(LED_BUILTIN, HIGH);
}


Exercício 3:

int tempo = 0;

void setup()
{
  pinMode(LED_BUILTIN, OUTPUT);
  tempo = 1000;
}

void loop()
{
  delay(tempo);
  digitalWrite(LED_BUILTIN, LOW);
  delay(tempo);
  digitalWrite(LED_BUILTIN, HIGH);
}


Exercício 4: 

int tempo = 0;

void setup()
{
  pinMode(LED_BUILTIN, OUTPUT);
  pinMode(12, OUTPUT);
  tempo = 1000;
}

void loop()
{
  delay(tempo);
  digitalWrite(LED_BUILTIN, LOW);
  delay(tempo);
  digitalWrite(LED_BUILTIN, HIGH);
  delay(tempo);
  digitalWrite(12, LOW);
  delay(tempo);
  digitalWrite(12, HIGH);
}


Exercício 5:

int tempo = 0;

void setup()
{
  pinMode(LED_BUILTIN, OUTPUT);
  pinMode(12, OUTPUT);
  tempo = 1000;
}

void loop()
{
  delay(tempo);
  digitalWrite(LED_BUILTIN, LOW);
  delay(tempo);
  digitalWrite(12, HIGH);
  delay(tempo);
  digitalWrite(LED_BUILTIN, HIGH);
  delay(tempo);
  digitalWrite(12, LOW);
}


Exercício 6:

int tempo = 0;

void setup()
{
  pinMode(13, OUTPUT);
  pinMode(12, OUTPUT);
  pinMode(11, OUTPUT);
  tempo = 1000;
}

void loop()
{
  digitalWrite(13, HIGH);
  delay(tempo);
  digitalWrite(13, LOW);
  digitalWrite(11, HIGH);
  delay(tempo);
  digitalWrite(11, HIGH);
  digitalWrite(12, HIGH);
  delay(tempo);
  digitalWrite(12, LOW);
}


Exercício 7: 

int i = 0;

void setup()
{
  pinMode(11, OUTPUT);
}

void loop()
{
  for (i = 0; i <= 255; i += 5) {
    analogWrite(11, i);
    delay(50);
  }
}


Exercício 8:

void setup()
{
  pinMode(11, OUTPUT);
  pinMode(10, OUTPUT);
  pinMode(9, OUTPUT);
}

void loop()
{
  digitalWrite(11, 255);
  delay(1000);
  digitalWrite(11, 0);
  delay(1000);
  digitalWrite(10, 255);
  delay(1000);
  digitalWrite(10, 0);
  delay(1000);
  digitalWrite(9, 255);
  delay(1000);
}


Exercício 9:

int luminosidade = 0;

void setup()
{
  pinMode(A0, INPUT);
}

void loop()
{
  luminosidade = analogRead(A0);
  Serial.println(luminosidade);
  delay(10);
}


Exercício 10:

int luminosidade = 0;

void setup()
{
  pinMode(A0, INPUT);
  pinMode(LED_BUILTIN, OUTPUT);
}

void loop()
{
  luminosidade = analogRead(A0);
  if (luminosidade < 750) {
    digitalWrite(LED_BUILTIN, HIGH);
  } else {
    digitalWrite(LED_BUILTIN, LOW);
  }
  delay(10);
}
