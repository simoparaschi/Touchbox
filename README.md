# Touchbox
Bringing people living with dementia and informal carers together through music and physical contact.

Project by PinkTomate - Beach Bagenal, Bente Vonk, Obafemi Omitiran & Simo Paraschi. Code by: Simo Paraschi

Touchbox is a connection & musical interface that invites a person with dementia (PwD) and their informal carer to sit together and generate music through physical contact. It is the result of a participatory design approach, where we discovered the relational challenge that dementia poses between the PwD and the informal carer.

# Tools required:
- 2 light-dependent resistor(LDRs)
- ESP 8266 | I used Adafruit's Feather HUZZAH ESP8266
- [shiftr.io broker](https://www.shiftr.io/)
- p5.js editor

# How it works
The LDRs are placed on top of the Touchbox. In order to start a song, they should be covered by the PwD and the informal carer. When the LDRs are covered, the signals are sent to the p5.js sketch through the broker, shift.io. They are sent via Wi-Fi by the ESP8266 using the MQTT protocol. When the p5.js receives the signals, a song is played.

p5.js code [Can be accessed here](https://editor.p5js.org/simoparaschi/sketches/JRa9bdV6x).

In order to allow loved ones to share music remotely, you can leverage Spotify's API to choose & send a song. The sketch or this interaction [can be accessed here](https://editor.p5js.org/simoparaschi/sketches/rVUKaCxMi).

# Steps
- You can either create your own instance in siftr.io or use ours: **https://connectr.cloud.shiftr.io/**;
- Head to p5.js and [check this sketch](https://editor.p5js.org/simoparaschi/sketches/JRa9bdV6x);
- Connect LDRs to ESP 8266 - there are a few resources out there, [here's one](https://www.instructables.com/NodeMCU-With-LDR/);
- Program your ESP 8266 to send signals to the broker;

If you want to add the second interaction, for loved ones to send songs remotely, then:
- [Check this p5.js sketch](https://editor.p5js.org/simoparaschi/sketches/rVUKaCxMi);
- Note that each time that you send a song, the connectr shiftr.io broker shows this feedback visually;
