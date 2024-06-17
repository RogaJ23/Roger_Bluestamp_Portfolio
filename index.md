# Bluestamp WALLE robot
A simple emotional robot that can interact with the user.  With 2 8x8 LED eyes and servo-controlled eyebrows, this robot is great at conveying emotions and makes for an interesting project.  Some challenges, takeaways, and triumphs are...

<!---
You should comment out all portions of your portfolio that you have not completed yet, as well as any instructions:
-->
| **Engineer** | **School** | **Area of Interest** | **Grade** |
|:--:|:--:|:--:|:--:|
| Roger J | Valley Christian | Electrical Engineering | Incoming Junior
<!---
**Replace the BlueStamp logo below with an image of yourself and your completed project. Follow the guide [here](https://tomcam.github.io/least-github-pages/adding-images-github-pages-site.html) if you need help.**
![Headstone Image](logo.svg)
-->
<!---
# Final Milestone

**Don't forget to replace the text below with the embedding for your milestone video. Go to Youtube, click Share -> Embed, and copy and paste the code to replace what's below.**

<iframe width="560" height="315" src="https://www.youtube.com/embed/F7M7imOVGug" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" allowfullscreen></iframe>

For your final milestone, explain the outcome of your project. Key details to include are:
- What you've accomplished since your previous milestone
- What your biggest challenges and triumphs were at BSE
- A summary of key topics you learned about
- What you hope to learn in the future after everything you've learned at BSE



# Second Milestone

**Don't forget to replace the text below with the embedding for your milestone video. Go to Youtube, click Share -> Embed, and copy and paste the code to replace what's below.**

<iframe width="560" height="315" src="https://www.youtube.com/embed/y3VAmNlER5Y" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" allowfullscreen></iframe>

Since my first milestone, I've worked on mostly the code for my WALLE robot.  I made the ultrasonic sensor work and linked it to the other parts of my project.  Now based on the distance from the ultrasonic sensor, the LED will display different emotions, the servos will turn accordingly, and the LCD also displays text accordingly.  One challenge that I faced was that when I first coded the project, the LED would flash repeatedly and be very inconsistent.  I fixed this problem by adding a delay for all the functions called so the ultrasonic sensors wouldn't go crazy.  My final step until finishing the project is just to get the 3D models and put the whole thing together.

For your second milestone, explain what you've worked on since your previous milestone. You can highlight:
- Technical details of what you've accomplished and how they contribute to the final goal
- What has been surprising about the project so far
- Previous challenges you faced that you overcame
- What needs to be completed before your final milestone 
-->
# First Milestone

<iframe width="853" height="480" src="https://www.youtube.com/embed/qGtCxEa6qno" title="Roger J.  First Milestone" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>


For my first milestone, I wired all the parts to the breadboard and the Arduino Uno.  I connected the Servos, the LCD, the 8 by 8 LEDs via soldering, and connected the battery to the breadboard to power the servos, as the Arduino doesn't provide enough power to power all the servos.  I also wrote some rough code to make sure all the parts worked.  I got the servos to turn by connecting them to the battery and the Arduino, the LEDs to light up with patterns(instead of linking both together I just connected both of them separately to the Arduino using the digital pins), and the LCD to display text after importing a few libraries.  One challenge that I faced was that my LEDs did not match the schematic, so I had to research online to find out which pins they went in.  Furthermore, I also had to look at the LedControl libraries and write my own code as my circuit was slightly different from the guide.  Another challenge was that the many wires that I had used made the circuit very messy and very difficult to navigate, however, I solved by using shorter wires whenever possible.  Eventually, the LED should be able to display patterns mimicking eyes, the LCD should be able to display text accordingly, the servos should allow the robot to turn its head, and finally, an ultrasonic sensor will be installed so the robot can gauge how close you are to it.  My next milestone would be to code everything so it can finally become like a robot.

<!---
- An explanation about the different components of your project and how they will all integrate together
- Technical progress you've made so far
- Challenges you're facing and solving in your future milestones
- What your plan is to complete your project
-->
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
| Arduino Uno Micro Controller | What the item is used for | $27.60 | <a href="https://store-usa.arduino.cc/products/arduino-uno-rev3?selectedStore=us"> Link </a> |
| 8x8 LED Matrix | Displays Patterns | $8.39 | <a href="https://www.amazon.com/HiLetgo-MAX7219-Matrix-Display-Control/dp/B07W6KZR5D/ref=sr_1_5?dib=eyJ2IjoiMSJ9.6txDTzXzJwL8zRVV3YtO1yrmajfw_y0CRyigoCFoMIf88gIXeooJOXb8vYGUPIq0ObonuTtZnzUEotuXGhGzon6_EBAz6eLEiSHXrQnBn1bpSF8szejjS2wPzlB_Aroc0BcPT6NmkuJIvRKPQyfU9aBSBU_OkM12iRvIUaR5i2HyxZtCrPSBX1vzREg-EEXIP5nszX4BSmPGHCafCqtopu99CJ6Td4UNGO7lZv-4peXGvjHPyu3Y28APtZjtCZPvynuY8HzGD7u7RWK7hqPFmP-GRyYzSpcaqaHQoV2xDUI.qPsKRkoPQyIxU-Ya7c2xrVnCVEO19NlNWIfv44fwAH4&dib_tag=se&keywords=8x8+LED+Matrix&qid=1718650968&sr=8-5"> Link </a> |
| 16x2 LCD w/ I2C backpack | Display Text | $9.95 | <a href="https://www.adafruit.com/product/292"> Link </a> |
| 2x Standard Sized Hobby Servos | What the item is used for | $27.60 | <a href="https://store-usa.arduino.cc/products/arduino-uno-rev3?selectedStore=us"> Link </a> |
| Arduino Uno Micro Controller | What the item is used for | $27.60 | <a href="https://store-usa.arduino.cc/products/arduino-uno-rev3?selectedStore=us"> Link </a> |
| Arduino Uno Micro Controller | What the item is used for | $27.60 | <a href="https://store-usa.arduino.cc/products/arduino-uno-rev3?selectedStore=us"> Link </a> |

# Other Resources/Examples
One of the best parts about Github is that you can view how other people set up their own work. Here are some past BSE portfolios that are awesome examples. You can view how they set up their portfolio, and you can view their index.md files to understand how they implemented different portfolio components.
- [Example 1](https://trashytuber.github.io/YimingJiaBlueStamp/)
- [Example 2](https://sviatil0.github.io/Sviatoslav_BSE/)
- [Example 3](https://arneshkumar.github.io/arneshbluestamp/)

To watch the BSE tutorial on how to create a portfolio, click here.

# Starter Project

<iframe width="560" height="315" src="https://www.youtube.com/embed/FUIzb9q6gWU" title="Roger J.  Starter Project" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>

The Starter Project that I created was the retro arcade game.  It is composed of a microcontroller, LED dot matrix screens, digital tube, keyboard, buzzer, and power supply circuit.  The process was to solder all of the parts onto the PCB, and then also to connect a battery holder to the PCB for the game to work.  
Process:
1. First solder all the buttons to the PCB(6)
2. Solder the 5 joints of the micro USB
3. Solder the 220uF electrolytic capacitor.(Long pin into +, short pin into -)
4. Solder the self-lock switch
5. Solder the buzzer, 2 dot matrix modules, and digital display tube
6. Test the game kit using the micro USB
7. Install the battery case on the back of the shell
8. Use bolts to stabilize and connect the shells
9. Finally, installed button caps and shell to the PCB, to protect the kit and make it nice to hold

Some difficulties that I encountered were during soldering because the parts were so closely compacted. Using a multimeter, I determined the parts that were wrongly connected and used both a desoldering pump and desoldering wire to remove overlapping metal.  With these changes and also connecting a battery holder to the PCB, I was finally able to make it work and encased it in a protective shell.
