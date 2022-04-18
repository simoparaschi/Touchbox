# Touchbox
Bringing people living with dementia and informal carers together through music and physical contact.

Project by PinkTomate - Beach Bagenal, Bente Vonk, Obafemi Omitiran & Simo Paraschi. Code by: Simo Paraschi

Touchbox is a connection & musical interface that invites a person with dementia (PwD) and their informal carer to sit together and generate music through physical contact. It is the result of a participatory design approach, where we discovered the relational challenge that dementia poses between the PwD and the informal carer.

# Tools required:
- 2 light-dependent resistor(LDRs)
- ESP 8266 | I used Adafruit's Feather HUZZAH ESP8266
- p5.js editor

# How it works
The LDRs are placed on top of the Touchbox. In order to start a song, they should be covered by the PwD and the informal carer. When the LDRs are covered, the signals are sent to the p5.js sketch via Wi-fi by the ESP8266 using using the MQTT protocol. When the p5.js receives the signals, a song is played.

p5.js code [Can be accessed here](https://editor.p5js.org/simoparaschi/sketches/JRa9bdV6x).
