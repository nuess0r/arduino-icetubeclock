Arduino based Ice Tube Clock
============================

Use the Arduino IDE to write programs for your Ice Tube Clock from Adafruit. https://www.adafruit.com/product/194

The idea was to rewrite the Ice Tube Clock firmware and add some features but I stopped somewhere on the way.

So the only thing in this repository is the custom board definition needed for the Arduino IDE to know the Ice Tube Clock.

Thanks to this tutorial creating such a definition was relatively fast: https://www.instructables.com/id/Arduino-IDE-Creating-Custom-Boards/

Next:
- Install board in your Arduino IDE (see below)
- Solder a 6-pin ISP connector to your Ice Tube Clock
- Connect an AVR ISP programmer or use another Arduino for ISP.

Arduino IDE Setup
-----------------
This instructions are based on the how-to from Todd Treece
https://learn.adafruit.com/add-boards-arduino-v164/installing-boards

The first thing you will need to do is to download the latest release of the Arduino IDE. You will need to be using version 1.8 or higher for this guide

After you have downloaded and installed the latest version of Arduino IDE, you will need to start the IDE and navigate to the Preferences menu. You can access it from the File menu in Windows or Linux, or the Arduino menu on OS X.

Copy and paste the link below into the Additional Boards Manager URLs option in the Arduino IDE preferences.

`https://github.com/nuess0r/arduino-icetubeclock/blob/master/arduino-custom-board/package_icetubeclock_index.json?raw=true`

If you have multiple boards you want to support, say ESP8266 and Adafruit, have both URLs in the text box separated by a comma (,)

Once done click OK to save the new preference settings.


Installing Boards
-----------------

Now that you have added the appropriate URLs to the Arduino IDE preferences, you can open the Boards Manager by navigating to the Tools->Board menu.

Once the Board Manager opens, click on the category drop down menu on the top left hand side of the window and select Contributed. You will then be able to select and install the boards supplied by the URLs added to the prefrences.

Next, quit and reopen the Arduino IDE to ensure that all of the boards are properly installed. You should now be able to select and upload to the new boards listed in the Tools->Board menu.
