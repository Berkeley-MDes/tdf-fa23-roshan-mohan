
I needed a lightweight laptop stand that I could easily carry in my backpack. Considering acrylic's flexible properties, I noticed a lack of projects that utilized this aspect of plastic linear deformation in acrylic.

So, I thought, why not create a laptop stand that flexes to the desired form and then unflexes to a flat shape? An added benefit would be the minimal use of materials.

I quickly sketched the idea. If successful, I believed it could be a great first contribution to shapediver.com, allowing users to customize the design based on their laptop dimensions, required height, and angle.

To achieve this, I needed to model it in its bent form and then unroll it. I sought help from TJ to understand how to unroll the model, and during our interaction, I gained valuable insights into the Grasshopper workflow.

I still had doubts about the curve an acrylic sheet would form when bent. Would it be an arc, an ellipse, a parabola, or something not conic? To gain some insight, I conducted a basic simulation in Fusion. It turns out that thinner acrylic sheets tend to form an arc, while thicker sheets of the same dimensions tend toward an ellipse.

I replicated the arc pattern in Grasshopper, trimmed the surface at my desired angle for the laptop base, and then used the unroll function to create a laser-cuttable template.

After generating the DXF file, I attempted to cut it on a 1.5mm scrap acrylic sheet at a 1:2 scale. It worked well, flexing without breaking and providing repeatable results!

I also wanted to try the living hinge pattern on wood. I found suitable scrap wood and created the cut pattern after importing the DXF into Illustrator.

The cutting process went smoothly, and the flexure pattern worked, although the plywood wasn't ideal due to its weak grain structure at random locations. I had to reinforce my part with masking tape.

I documented this journey in this 2-minute video: https://youtu.be/yoj3MpN0xTw

My next steps include honing my Grasshopper skills and making the model available on shapediver.com for customization by others.
