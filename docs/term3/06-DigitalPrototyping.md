---
hide:
    - toc
---

# Digital Prototyping
<div style="height:2px; background-color: #E17858; margin-top: 40px; margin-bottom: -20px;"></div>


## CNC Furniture
> Modular Shelf. 

> Núria Valsells, Oliver Lloyd and Carmen Robres

### References
![](../images\term3\Prototyping\RefesM3.jpg) 


### Process
At first, we had to make several changes to the product design. Initially, we attempted to create a modular and large shelving unit. However, we soon realized that we didn't have enough wood to construct a shelving unit made up of four blocks. Therefore, we opted to create an L-shaped structure to reduce the amount of wood needed. 

This design better suited our requirements and the available materials. However, when we presented this design for cutting, we were informed that it lacked balance due to excess material on the sides, and it didn't guarantee stability. Consequently, we redesigned the structure to consist of cubes, small squares that could be added both vertically and horizontally. 

This time, we focused on just two blocks instead of three and incorporated further structural changes to ensure balance. We transitioned from using pressure-based joints to employing a T-joint system, which required screws and washers to secure the pieces together. Additionally, to insert the shelves into the cubes, we utilized a typical Ikea-style system where holes were drilled, and small wooden pegs to support the shelves. 

However, we encountered two structural issues: the initial design was intended for a CNC M4 machine, which was broken, necessitating a design change, and the male-female joint configuration was modified to ensure structural integrity by making each piece have both male and female sides for better grip and stability. These adjustments were made, and we were finally able to print and cut using the CNC machine.

![](../images\term3\Prototyping\PROCESS.jpg)

Finally, we proceeded to cut with the CNC. We encountered only one error, which occurred when programming the CNC: we positioned the material incorrectly. As a result, during the transition from engraving to cutting, the CNC slightly went over the material. Essentially, it cut the wood when it shouldn't have while moving. To rectify this, we stopped the machine and corrected the error so that when it returned to zero, it moved upward this time.

Additionally, we had a minor oversight: the wooden pieces needed to be positioned perfectly. When inserting the screws, we should have drilled slightly smaller holes to ensure better fixation. Nonetheless, the final product turned out perfectly. My reflection would be to explore ways to connect the two modules, perhaps using 3D printed pieces or similar solutions.

![](../images\term3\Prototyping\PROCESS2.jpg)

![](../images\term3\Prototyping\CNCFINAL.jpg)



### Reflection: The four F’s of active reviewing
*Facts:* 

- We had to redesign the product three times to improve its stability.

- There was a minor error in the CNC, but it was corrected.

- The most complex part was the design and the tolerance to consider, taking into account the tools that had to be used and the CNC itself.

 *Feelings:* 

- Initially, I thought the CNC would be intimidating, but after redesigning the product 3 times, I gained confidence knowing it would cut well.

-  This process helped me understand better how it works and gave me much more assurance, not only in the design process, which is also complex due to speed and tolerance issues, but also because it's a large machine that commands respect.

- Despite encountering errors, we were finally able to create a correct and functional structure.


 *Findings:* 

- I learned various methods of joining, which I believe will be valuable in the future.

- The experience also taught me to derive confidence from it and explore different ways to create stable products.

 *Future:* 
 
- I aim to utilize the CNC more in the future.

- Additionally, I envision using 3D printing to create parts that can join the sides of the structure, ensuring better quality and stability.
 
<span style="background-color: #FFFCFA; padding: 10px; border: 1px solid #699ADA;"> [Fabrication files](https://drive.google.com/drive/folders/1NmSh28hcguX5nGBE1HpGVCuo5WYQRLI6?usp=drive_link).</span>

## Sensing & Wearables

> Anna Fedele and Carmen Robres

### References
For this project, our goal was to experiment with different input methods, whether through textiles, the phone, or the camera. This prepared us for MDFest, which is essentially our project theme: playing with sensors and exploring how we can detect the body in various ways. Our reference was to create a sort of online call where, based on the detected emotions and movement, the camera feed would change color and sound according to how the person on the other end interacted with you.
The inputs are supposed to be: Soft sensor, phone and face.

![](../images\term3\Prototyping\RefesM4.jpg) 

### Soft Sensor
We also created two types of textile sensors. One had a mesh design, allowing us to detect various pressure points across the fabric. The other, simpler one, colored red, detected pressure or its absence using an Arduino. Essentially, we developed these textiles in class and then programmed Arduino and Processing to receive and display the data accordingly.

![](../images\term3\Prototyping\SOFTM4.jpg) 

### Process
Next, we took the three inputs and trained the Wekinator so that, in the following module, we could simply play with inputs 0, 1, or 2. Essentially, we aimed to train a model to detect when someone is angry, indicated by aggressive movements, when someone is happy, indicated by fluid movements, and when someone is confused, indicated by minimal movement. The third input is the soft sensor, which essentially allowed us to halt all subsequent inputs. In other words, face and phone tracking are of the same type, recognizing feelings and emotions, while the last one is simply a button we'll use to alter the inputs and outputs of Wekinator and Max8 in a different way.

![](../images\term3\Prototyping\FABRICATIONM4.jpg) 

**Video of the training**
<iframe width="560" height="315" src="https://www.youtube.com/embed/D30XIrBqzps?si=DH1QLfwCDWyFmj_2" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>


**Final Product**
<iframe width="560" height="315" src="https://www.youtube.com/embed/KlrL4ZGIO6s?si=FO0AeRaU3HYV8eYU" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>



### Reflection: The four F’s of active reviewing

*Facts:* 

- Programming emotions was more complex than the soft sensor.
- Determining what constituted an angry movement compared to a happy one took more time, as the phone only captures X, Y, and Z inputs and does not define movement over time; it only defines positions.
- Wekinator is relatively simple to program, but the challenge lies in understanding which input to use and how to program it.

 *Feelings:* 

- It was quite interesting, especially since this is the topic of my thesis. I enjoyed exploring different ways to train and detect body movements and send messages through various devices without the need for MQTT.

 *Findings:* 

- I discovered how to create a soft sensor, which was something new to me.
- Detecting emotions over time is challenging because it involves analyzing frames and movements. 
- Training a model on movement is complex since it detects an input per every frame. The position of a hand can be considered happy or angry because the overall detection is the movement not the frame.
- Creating a database is complex, especially for subjective aspects like emotions. 

 *Future:* 

- Improving the dataset. The model would need thorough training with different people, lighting conditions, camera orientations, and distances to ensure accuracy.
- Delving into more articles about different physical characteristics of emotions would be beneficial for accurate detection.

 
<span style="background-color: #FFFCFA; padding: 10px; border: 1px solid #699ADA;"> [Wekinator and Arduino files](https://drive.google.com/drive/folders/1MikflwB34YotAWqRJw89eskvKkQK2kZk?usp=sharing).</span>



## Output Visuals

> Anna Fedele and Carmen Robres

### References

The main objective is to alter the inputs through sound and video, attempting to manipulate the visuals to touch upon various aspects of the video recieved.

![](../images\term3\Prototyping\RefesM5.jpg) 


### Process

![](../images\term3\Prototyping\FABRICATIONM5.jpg) 

For this project, our task was to use the inputs we had programmed through Wekinator and produce the output. Since we aimed to alter the concept of a video call, we generated an audio message like, "Hello, hello, can you hear me?" and also the camera feed. Then, based on the movements and emotions we conveyed to our computer, the output of both the camera feed and audio would change. Ultimately, the soft sensor was used more to create a negative or pause effect on the camera feed. In other words, while emotions detected triggered changes in the image, the soft sensor served as a way to pause, switch, and create a negative of the camera feed.


<iframe width="560" height="315" src="https://www.youtube.com/embed/Aez96EIRoJ4?si=kktfisGckZhYRVLo" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>

**Final Product**

<iframe width="560" height="315" src="https://www.youtube.com/embed/C4JTLCt9FJ0?si=rMS3MqCw8D9c8jZ5" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>


### Reflection: The four F’s of active reviewing

*Facts:* 

- Editing in Max was quite complex because, fundamentally, editing sound and image may seem easy, but you need to understand the factors interacting with both to know what to adjust.
- Receiving all these messages via OSC was relatively easy since there were only three outputs listened to from the same port.

 *Feelings:* 

- Experimenting with Max 8 was quite enjoyable, but it's indeed challenging to understand how the program works because we're unsure of its capabilities. 
- Lacking musical knowledge makes it difficult to grasp audio editing and mixing concepts.


 *Findings:* 

- From now on, I'll be able to use Max to create better outputs, as my thesis revolves around presenting different aspects artistically. 
- Max seems very suitable for creating artistic representations that are sensory, sound-based, or visual, allowing people to understand concepts like aggression and emotions through the program.

 *Future:* 

 - I would also like to complete the cycle by not only receiving inputs and generating generic outputs but also sending messages from Max to other devices for a more personalized understanding of the programming.

 
<span style="background-color: #FFFCFA; padding: 10px; border: 1px solid #699ADA;"> [Max8 files](https://drive.google.com/drive/folders/1tu5ag2uHh_FHIjiZ3CIBKoR3howRwg7L?usp=sharing).</span>
