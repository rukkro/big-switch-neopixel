# big-switch-neopixel

Follow the guide [here](https://www.reddit.com/r/MechanicalKeyboards/comments/7oiv5o/guide_how_to_make_a_big_switch_lamp/) to make a lamp and usable keyboard button with NovelKey's Big Switch.

#### Possible differences between the tutorial:
Update the code to match your setup as necessary.

  1. Different pins than used in the diagram.
  Edit these to match your pins:
  
    
    #define LED_PIN 5
    #define BUTTON_PIN 2
    
  2. Used Arduino IDE instead of AVRDUDESS with my code.
  3. Used 16 LED NeoPixel ring and a 5V Pro Micro.

### Setup in Arduino IDE
  1. Install the ProMicro addon to the Arduino IDE, as explained [here](https://learn.sparkfun.com/tutorials/pro-micro--fio-v3-hookup-guide#installing-windows). Ensure you select the correct Pro Micro board (3.3V vs 5V) in Arduino's menus!
  2. Install the NeoPixel libraries, as explained [here](https://learn.adafruit.com/adafruit-neopixel-uberguide/arduino-library-installation).
  3. Open my code into the IDE and try to upload to the Pro Micro. Resetting the board might be necessary.
  
### What does it do?
  1. Normal press to trigger Windows/super key. The button should lightup briefly when pressed.
  2. Long press to put it in LED mode. This will turn the LEDs on and leave them on. As you hold the button down, it will fade between different colors until you let go. Normal press the button to turn off the light.
  
