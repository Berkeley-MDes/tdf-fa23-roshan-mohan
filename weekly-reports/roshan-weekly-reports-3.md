# Report 3 - Week of 09/11/2023  #


I needed a lightweight laptop stand that I could easily carry in my backpack. Considering acrylic's flexible properties, I noticed a lack of projects that utilized this aspect of plastic linear deformation in acrylic.

So, I thought, why not create a laptop stand that flexes to the desired form and then unflexes to a flat shape? An added benefit would be the minimal use of materials.

I quickly sketched the idea. If successful, I believed it could be a great first contribution to shapediver.com, allowing users to customize the design based on their laptop dimensions, required height, and angle.

To achieve this, I needed to model it in its bent form and then unroll it. I sought help from TJ to understand how to unroll the model, and during our interaction, I gained valuable insights into the Grasshopper workflow.


I still had doubts about the curve an acrylic sheet would form when bent. Would it be an arc, an ellipse, a parabola, or something not conic? To gain some insight, I conducted a basic simulation in Fusion. It turns out that thinner acrylic sheets tend to form an arc, while thicker sheets of the same dimensions tend toward an ellipse.

I replicated the arc pattern in Grasshopper, trimmed the surface at my desired angle for the laptop base, and then used the unroll function to create a laser-cuttable template.

<img width="1500" alt="Screenshot 2023-09-14 at 11 53 29 PM" src="https://github.com/Berkeley-MDes/tdf-fa23-roshan-mohan/assets/142958314/29bd6bad-8af8-4367-9eb6-df1a4446eb82">
<img width="1544" alt="Screenshot 2023-09-14 at 11 53 08 PM" src="https://github.com/Berkeley-MDes/tdf-fa23-roshan-mohan/assets/142958314/f43aa9d9-f044-4971-b521-160b727ee06a">

![Screenshot 2023-09-11 at 11 14 14 PM](https://github.com/Berkeley-MDes/tdf-fa23-roshan-mohan/assets/142958314/cbca993c-dd9d-4163-8999-2f87ed664626)


After generating the DXF file, I attempted to cut it on a 1.5mm scrap acrylic sheet at a 1:2 scale. It worked well, flexing without breaking and providing repeatable results!

I also wanted to try the living hinge pattern on wood. I found suitable scrap wood and created the cut pattern after importing the DXF into Illustrator.

The cutting process went smoothly, and the flexure pattern worked, although the plywood wasn't ideal due to its weak grain structure at random locations. I had to reinforce my part with masking tape.

I documented this journey in this 2-minute youtube video: 

[![The Journey](https://img.youtube.com/vi/yoj3MpN0xTw/0.jpg)](https://www.youtube.com/watch?v=yoj3MpN0xTw)


My next steps include honing my Grasshopper skills and making the model available on shapediver.com for customization by others.
