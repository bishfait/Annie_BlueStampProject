# Smart Mirror
Replace this text with a brief description (2-3 sentences) of your project. This description should draw the reader in and make them interested in what you've built. You can include what the biggest challenges, takeaways, and triumphs from completing the project were. As you complete your portfolio, remember your audience is less familiar than you are with all that your project entails!

| **Engineer** | **School** | **Area of Interest** | **Grade** |
|:--:|:--:|:--:|:--:|
| Annie W | Foothill High School | Electrical Engineering | Incoming Senior

<!--**Replace the BlueStamp logo below with an image of yourself and your completed project. Follow the guide [here](https://tomcam.github.io/least-github-pages/adding-images-github-pages-site.html) if you need help.**-->

<h1 align="center"><img src="annieHeadshot.png" width="400"/></h1>
  
# Final Milestone
For your final milestone, explain the outcome of your project. Key details to include are:
- What you've accomplished since your previous milestone
- What your biggest challenges and triumphs were at BSE
- A summary of key topics you learned about
- What you hope to learn in the future after everything you've learned at BSE

**Don't forget to replace the text below with the embedding for your milestone video. Go to Youtube, click Share -> Embed, and copy and paste the code to replace what's below.**

<iframe width="560" height="315" src="https://www.youtube.com/embed/F7M7imOVGug" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" allowfullscreen></iframe>

# Second Milestone

<<**video**>>

## Progress
Focusing on the modifications of the MagicMirror, I set up and programmed the ultrasonic sensor to turn on or off the mirror's monitor whether an obstacle is in distance or not. This is to mimic someone standing in front of a mirror, and that certain distance is the distance from the mirror to the person. Basically, if an object is in a certain distance in front of the sensor, the MagicMirror will turn on and stay on as long as the object is within the vicinity. When the sensor cannot detect any obstacles in front of it, it will wait fifteen seconds before turning the mirror off. After the mirror is off, any detected obstacles can turn on the mirror again. In essence, the mirror can be turned on and off multiple times and continuously detect for obstacles to turn on or off the mirror. In addition, I coded the sensor to wait five minutes before terminating the code, so it will stop running after a period of inactivity.

## Challenges
### Wiring the Ultrasonic Sensor
Figuring out how to wire the Raspberry Pi to the ultrasonic sensor was a difficulty that I encountered. The Raspberry Pi 400, similar to a Raspberry Pi 4, has many pins(40  pins) and figuring out which pins that the ultrasonic sensor had to be plugged into was difficult. An ultrasonic sensor has four pins: VCC, GND, Trig, and Echo. VCC and GND are the power supply pins. The trig pin sends an ultrasonic wave, which can hit an obstacle and gets reflected back. The reflected wave is received by the receiver of the sensor and goes from the initial state of HIGH to LOW when the wave is received. In addition, the ultrasonic sensor operates on 5V, but sending a 5V output signal from the echo pin to the GPIO(General Purpose Input/Output of Rpi would damage the pin since it is rated at 3.3V. Thus, a voltage divider circuit is necessary to turn 5V into 3.3V by using two series resistors.

Plugging in the power supply pins into the correct pins of the Raspberry Pi was the simple part; figuring out the correct set up for the echo and trig pins were the challenging part. The echo pin required the voltage divider pin. With a lot of research, on the Raspberry Pi 400 the trig pin goes into GPIO 11(pin 23) and the echo pin goes into GPIO 12(pin 32). 
<h1 align="center"><img src="circuitDiagram.jpg" width="500"/></h1>
<h5 align="center">Circuit of the ultrasonic sensor</h5>
<h1 align="center"><img src="Image 6-21-23 at 10.06 AM.jpg" width="200"/></h1>
<h5 align="center">Raspberry Pi 400 GPIO Pinout Diagram</h5>

### Coding the Sensor with Python

## Next Steps
# First Milestone: Intensive Project-- Smart Mirror

<iframe width="560" height="315" src="https://www.youtube.com/embed/TV7BxGYUKKc" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" allowfullscreen></iframe>

The smart mirror utilizes a monitor to display extra details behind a semi-transparent mirror. These details can be a variety of widgets, ranging from displaying the time, the weather, or upcoming events. In essence, the program I used, MagicMirror2, displays a website. By modifying the code behind what this website displays by utilizing Javascript and CSS, the interface of the mirror can be personalized. For the assembly of the mirror, plywood is needed to hold up the monitor in place. Extra decoration of the mirror includes LED strips that will border the mirror.

### Components

#### Transparent Mirror
The mirror must be transparent for it to display the monitor. Since we are able to see through the mirror and see ourselves in the mirror, we can see what is displayed on the monitor and ourselves. 

#### Monitor
Displays the MagicMirror widgets behind the mirror.

#### Raspberry Pi 400 with MagicMirror2 installed
The Raspberry Pi 400 is basically a Raspberry Pi 4 inside a keyboard. It powers the monitor and the modules of the MagicMirror are edited on the Raspberry Pi. The MagicMirror2 program is primarily coded by Javascript and CSS. CSS "decorates" the appearance of the modules: setting up icons, the structure of widgets, the font, and so on.

Javascript codes for what is displayed and what extra information is needed for the MagicMirror to work. For example, for calendar module, Javascript gets the information necessary from the .ical calendar file provided. Variables set up a maximum of what is displayed or what icon configued by CSS is used.

#### LED Strips
Primarily for decoration. I want a rectangle-shaped strip of LEDs that wrap around the monitor, adjacent to the frame of the mirror. It is plugged into a power strip to be powered. The LEDs comes in one long strand, so the strip will need to be cut into four parts to wrap around the monitor.

#### Monitor Wall Mount, Plywood, Nylon webbing
Components that will be necessary for the assembly and mounting of the mirror. It would look messy if wires or parts that make the mirror work stuck out in view, so the Nylon webbing will keep different components together behind the mirror, stuck to the back with grommets and screws. The plywood is painted black and is used to keep the monitor in place behind the mirror. In addition, the plywood fills up any negative space that the monitor cannot fill, thus making the space behind the mirror all black for it to work. The MagicMirror background is black as well, thus giving a solid color behind the transparent mirror.

#### Ultrasonic Sensor(HC-SR04)
The Ultrasonic Sensor will track nearby movement, thus turning the mirror on when movement is detected near the mirror. Distance from the sensor is calculated by the interaction of the transmitter and receiver. The transmitter emits a chirp that is at a high pitch than the human ear can hear, and it measures the time this sound is bounced off an obstacle. We can code if the time tracked between the obstacle and the sensor in which the time is less than a certain value, the mirror will turn on. This certain value will be calibrated to the time it tracks when someone is standing in front of the mirror.

<h1 align="center"><img src="ultrasonicSensorDiagram" width="500"/></h1>

## Progress
As of now, I have accomplished setting up the Raspberry Pi and the monitor that will display all the widgets on the screen and the mirror. I tweaked existing widgets like the clock and weather to display the right time and place, giving the correct information for different variables in the code to display the right information. I added and synced up my calendars to display my upcoming events, including holidays, and my friends’ birthdays. In addition, I found other people’s code on adding different modules. I added a widget that would sync up to my Google Tasks and update every ten seconds, thus displaying my list of things I need to do. I went into the code itself to modify the mirror to my own liking. This included changing the font, changing the spacing between each item in a list, and changing and adding icons in the CSS files.

## Challenges
It was somewhat difficult since the program used different coding languages than I used. Javascript and CSS was completely new to me. However, learning new coding languages isn’t very hard as different coding languages have similarities. Reading someone else’s code that is in a language that you don’t recognize was intimidating at first, especially that the MagicMirror program is compiled of many, many folders and files in order for it to work, each filled with code necessary for its operation. Through some trial and error, I was able to personalize the set up of the MagicMirror to my own preference.

## Next Steps
The next thing to do is to assemble the mirror and add the LED strips behind the mirror. This requires the use of drilling tools and a router to put the plywood in place and sticking the LED strips in place. For the LED strips, I need to cut and solder the LED strips into desired length for it to be shaped like a rectangle, bordering the monitor.

<!-- ADD THIS LATER: An extra modification to add would be an ultrasonic sensor to detect movement near the monitor. This would detect movement close to the mirror, turning it on. By then, the Smart Mirror would be complete. Any final adjustments to the interface of the mirror would be the last thing to do.-->

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
| Wireless Mouse | Configures Raspberry Pi for the mirror display. Will be taken out later. | $7.79 | <a href="https://www.amazon.com/Wireless-TECKNET-Receiver-Portable-Adjustable/dp/B095HBY3RF?th=1"> Link </a> |
|:--:|:--:|:--:|:--:|
| Ultrasonic Distance Sensor | Tracks and calculates a person's distance from a mirror to turn on or off the mirror. | $4.50 | <a href="https://www.sparkfun.com/products/15569"> Link </a> |
|:--:|:--:|:--:|:--:|
| Power Strip | Powers Smart Mirror components. | $16.99 | <a href="https://www.amazon.com/gp/product/B092J8LPWR?ie=UTF8&psc=1&linkCode=sl1&tag=qtkwa-20&linkId=2711afc9129fc98b2bd0b14730062c9a&language=en_US&ref_=as_li_ss_tl"> Link </a> |
|:--:|:--:|:--:|:--:|

# Other Resources/Examples
One of the best parts about Github is that you can view how other people set up their own work. Here are some past BSE portfolios that are awesome examples. You can view how they set up their portfolio, and you can view their index.md files to understand how they implemented different portfolio components.
- [Example 1](https://trashytuber.github.io/YimingJiaBlueStamp/)
- [Example 2](https://sviatil0.github.io/Sviatoslav_BSE/)
- [Example 3](https://arneshkumar.github.io/arneshbluestamp/)

To watch the BSE tutorial on how to create a portfolio, click here.
