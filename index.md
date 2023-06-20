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
## Test
The smart mirror utilizes a monitor to display extra details behind a mirror. These details can be a variety of widgets, ranging from displaying the time, the weather, and upcoming events. In essence, the program I used, MagicMirror2, displays a website. By modifying the code behind what this website displays by utilizing Javascript, HTML, and CSS, the interface of the mirror is personalized.

As of now, I have accomplished setting up the Raspberry Pi and the monitor that will display all the widgets on the screen and the mirror. I tweaked existing widgets like the clock and weather to display the right time and place. I added and synced up my calendars to display my upcoming events, including holidays, and my friends’ birthdays. In addition, I found other people’s code on adding different modules. I added a widget that would sync up to my Google Tasks and update every ten seconds, thus displaying my list of things I need to do. I went into the code itself to modify the mirror to my own liking. It was somewhat difficult since the program used different coding languages than I used. Although I was slightly familiar with HTML, Javascript and CSS was completely new to me. However, learning new coding languages isn’t very hard as different coding languages have similarities. Reading someone else’s code that is in a language that you don’t recognize was intimidating at first, but over time I got familiarized with the different codes.

The next thing to do is to assemble the mirror and fix up the LEDs. An extra modification to add would be an ultrasonic sensor to detect movement near the monitor. This would detect movement close to the mirror, turning it on. By then, the Smart Mirror would be complete. Any final adjustments to the interface of the mirror would be the last thing to do.

**Don't forget to replace the text below with the embedding for your milestone video. Go to Youtube, click Share -> Embed, and copy and paste the code to replace what's below.**

<iframe width="560" height="315" src="https://www.youtube.com/embed/y3VAmNlER5Y" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" allowfullscreen></iframe>

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
