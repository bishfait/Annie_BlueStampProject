# Smart Mirror
Replace this text with a brief description (2-3 sentences) of your project. This description should draw the reader in and make them interested in what you've built. You can include what the biggest challenges, takeaways, and triumphs from completing the project were. As you complete your portfolio, remember your audience is less familiar than you are with all that your project entails!

| **Engineer** | **School** | **Area of Interest** | **Grade** |
|:--:|:--:|:--:|:--:|
| Annie W | Foothill High School | Electrical Engineering | Incoming Senior

**Replace the BlueStamp logo below with an image of yourself and your completed project. Follow the guide [here](https://tomcam.github.io/least-github-pages/adding-images-github-pages-site.html) if you need help.**

![Headstone Image](logo.svg)
  
# Final Milestone
For your final milestone, explain the outcome of your project. Key details to include are:
- What you've accomplished since your previous milestone
- What your biggest challenges and triumphs were at BSE
- A summary of key topics you learned about
- What you hope to learn in the future after everything you've learned at BSE

**Don't forget to replace the text below with the embedding for your milestone video. Go to Youtube, click Share -> Embed, and copy and paste the code to replace what's below.**

<iframe width="560" height="315" src="https://www.youtube.com/embed/F7M7imOVGug" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" allowfullscreen></iframe>

# First Milestone: Intensive Project-- Smart Mirror

The smart mirror utilizes a monitor to display extra details behind a semi-transparent mirror. These details can be a variety of widgets, ranging from displaying the time, the weather, or upcoming events. In essence, the program I used, MagicMirror2, displays a website. By modifying the code behind what this website displays by utilizing Javascript and CSS, the interface of the mirror can be personalized. For the assembly of the mirror, plywood is needed to hold up the monitor in place. Extra decoration of the mirror includes LED strips that will border the mirror.

### Components
- Transparent Mirror
      - The mirror must be transparent for it to display the monitor. Since we are able to see through the mirror and see ourselves in the mirror, we can see what is displayed on the monitor and ourselves. 
- #### Monitor
- Displays the MagicMirror widgets behind the mirror.
- #### Raspberry Pi 400 with MagicMirror2 installed
- The Raspberry Pi 400 is basically a Raspberry Pi 4 inside a keyboard. It powers the monitor and the modules of the MagicMirror are edited on the Raspberry Pi. The MagicMirror2 program is primarily coded by Javascript and CSS. CSS "decorates" the appearance of the modules: setting up icons, the structure of widgets, the font, and so on.
      - Javascript codes for what is displayed and what extra information is needed for the MagicMirror to work. For example, for calendar module, Javascript gets the information necessary from the .ical calendar file provided. Variables set up a maximum of what is displayed or what icon configued by CSS is used.
- #### LED Strips
- Primarily for decoration. I want a rectangle-shaped strip of LEDs that wrap around the monitor, adjacent to the frame of the mirror. It is plugged into a power strip to be powered. The LEDs comes in one long strand, so the strip will need to be cut into four parts to wrap around the monitor.
- #### Monitor Wall Mount, Plywood, Nylon webbing
- Components that will be necessary for the assembly and mounting of the mirror. It would look messy if wires or parts that make the mirror work stuck out in view, so the Nylon webbing will keep different components together behind the mirror, stuck to the back with grommets and screws. The plywood is painted black and is used to keep the monitor in place behind the mirror. In addition, the plywood fills up any negative space that the monitor cannot fill, thus making the space behind the mirror all black for it to work. The MagicMirror background is black as well, thus giving a solid color behind the transparent mirror.
- #### Ultrasonic Sensor(HC-SR04)
- The Ultrasonic Sensor will track nearby movement, thus turning the mirror on when movement is detected near the mirror. Distance from the sensor is calculated by the interaction of the transmitter and receiver. The transmitter emits a chirp that is at a high pitch than the human ear can hear, and it measures the time this sound is bounced off an obstacle. We can code if the time tracked between the obstacle and the sensor in which the time is less than a certain value, the mirror will turn on. This certain value will be calibrated to the time it tracks when someone is standing in front of the mirror.

## Progress
As of now, I have accomplished setting up the Raspberry Pi and the monitor that will display all the widgets on the screen and the mirror. I tweaked existing widgets like the clock and weather to display the right time and place, giving the correct information for different variables in the code to display the right information. I added and synced up my calendars to display my upcoming events, including holidays, and my friends’ birthdays. In addition, I found other people’s code on adding different modules. I added a widget that would sync up to my Google Tasks and update every ten seconds, thus displaying my list of things I need to do. I went into the code itself to modify the mirror to my own liking. This included changing the font, changing the spacing between each item in a list, and changing and adding icons in the CSS files.

## Challenges
It was somewhat difficult since the program used different coding languages than I used. Javascript and CSS was completely new to me. However, learning new coding languages isn’t very hard as different coding languages have similarities. Reading someone else’s code that is in a language that you don’t recognize was intimidating at first, especially that the MagicMirror program is compiled of many, many folders and files in order for it to work, each filled with code necessary for its operation. Through some trial and error, I was able to personalize the set up of the MagicMirror to my own preference.

## Next Steps
The next thing to do is to assemble the mirror and add the LED strips behind the mirror. This requires the use of drilling tools and a router to put the plywood in place and sticking the LED strips in place. For the LED strips, I need to cut and solder the LED strips into desired length for it to be shaped like a rectangle, bordering the monitor.

<!-- ADD THIS LATER: An extra modification to add would be an ultrasonic sensor to detect movement near the monitor. This would detect movement close to the mirror, turning it on. By then, the Smart Mirror would be complete. Any final adjustments to the interface of the mirror would be the last thing to do.-->

<iframe width="560" height="315" src="https://www.youtube.com/embed/TV7BxGYUKKc" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" allowfullscreen></iframe>

# Starter Project: RGB LED Practice Kit
The RGB LED Practice Kit is mostly for practice with soldering. By incorporating three sliding potentiometers to control each value of the RGB LED(red, green, and blue), the switches can control the color and intensity of the LED with remarkable precision.

The three sliding potentiometers would change the resistance in the circuit, thus changing how potent each value emits. In addition, controlling the resistance would also control the brightness of the LED; a higher resistance would result in a dimmer light and vice versa.

The challenging aspect of this project was wiring the LED. In an LED, there is a longer pin that shows which way is the right way to wire it. The RGB LED has four pins, and one long pin. The board did show where the long pin had to go, so this issue was quickly resolved.

<iframe width="560" height="315" src="https://www.youtube.com/embed/UVZ3a5gztnE" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" allowfullscreen></iframe>

# Schematics 
Here's where you'll put images of your schematics. [Tinkercad](https://www.tinkercad.com/blog/official-guide-to-tinkercad-circuits) and [Fritzing](https://fritzing.org/learning/) are both great resoruces to create professional schematic diagrams, though BSE recommends Tinkercad becuase it can be done easily and for free in the browser. 

# Code
Here's where you'll put your code. The syntax below places it into a block of code. Follow the guide [here]([url](https://www.markdownguide.org/extended-syntax/)) to learn how to customize it to your project needs. 

```c++
void setup() {
  // put your setup code here, to run once:
  Serial.begin(9600);
  Serial.println("Hello World!");
}

void loop() {
  // put your main code here, to run repeatedly:

}
```

# Bill of Materials
Here's where you'll list the parts in your project. To add more rows, just copy and paste the example rows below.
Don't forget to place the link of where to buy each component inside the quotation marks in the corresponding row after href =. Follow the guide [here]([url](https://www.markdownguide.org/extended-syntax/)) to learn how to customize this to your project needs. 

| **Part** | **Note** | **Price** | **Link** |
|:--:|:--:|:--:|:--:|
| DIY Soldering RGB Practice Kit | The Starter Project. Practice for soldering | $7.99 | <a href="https://www.amazon.com/Soldering-Practice-Learning-Electronics-Training/dp/B0BKM3D927"> Link </a> |
|:--:|:--:|:--:|:--:|
| Raspberry Pi 400 | Powers the Smart Mirror. | $70.00 | <a href="https://www.digikey.com/en/products/detail/raspberry-pi/SC0373/13282408"> Link </a> |
|:--:|:--:|:--:|:--:|
| Item Name | What the item is used for | $Price | <a href="https://www.amazon.com/Arduino-A000066-ARDUINO-UNO-R3/dp/B008GRTSV6/"> Link </a> |
|:--:|:--:|:--:|:--:|

# Other Resources/Examples
One of the best parts about Github is that you can view how other people set up their own work. Here are some past BSE portfolios that are awesome examples. You can view how they set up their portfolio, and you can view their index.md files to understand how they implemented different portfolio components.
- [Example 1](https://trashytuber.github.io/YimingJiaBlueStamp/)
- [Example 2](https://sviatil0.github.io/Sviatoslav_BSE/)
- [Example 3](https://arneshkumar.github.io/arneshbluestamp/)

To watch the BSE tutorial on how to create a portfolio, click here.
