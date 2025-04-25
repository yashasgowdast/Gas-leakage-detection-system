int gassensor-Al;

int buzzer-13;

I

int led=12;|

void setup()

{

pinMode (A1, INPUT);

pinMode (buzzer, OUTPUT);

pinMode (led, OUTPUT);

Serial.begin(9600);

}

void loop()

{

int sensorValue=analogRead(gasSensor);

Serial.print("GAS LEVEL:");

Serial.println(sensorValue);

delay(1000);

if (sensorValue>250)

Serial Monitor
{

digitalWrite(buzzer, HIGH);

digitalWrite(led, HIGH);
{
else
}
digitalWrite(buzzer, LOW);

digitalWrite(led, LOW);
}
