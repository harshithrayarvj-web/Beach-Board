# Beach-Board 
***Journals are separate files in the repo!***

*They contain most of the extra details*

A very dynamic and adaptable keyboard meant to pack as many punches as it can within it's relatively small form factor. Contains a raspberry pi pico, 68 hot-swapable switches, en ec11 rotary encoder, an sd card socket, and a TFT LCD, while being meant to operate on QMK.
<img width="1416" height="656" alt="Screenshot 2026-08-10 220419" src="https://github.com/user-attachments/assets/1cf71260-2d0f-4423-8690-0595cbca54da" />

# The idea behind it
As much as modern keyboards have numerous shortcuts and even gestures for other inputs, I felt that a centralized unit that could do almost all of those things, and more, could be very useful to quickly do things in a straight forward way, similar to a streamdeck. I plan on leveraging the keyboard layout to make it more moldable and flexible for complex tasks, even if they have many smaller details. Along with this I wanted to expand on how screens could be used on keyboards, instead of basic simple screens that show just one type of data, such as WPM, without much flavor, I wanted to have a screen that could potentially both add to the aesthetics of the keyboard, and provide a functional use depending on the task at hand. The theme of a beach themed "surf board" was because of my first long term profile picture that I drew, it helped me create an identity online, so I wanted to hint at that with my first proper project being a keyboard.

# Characteristics of keyboard
- 68 switches (epomaker creamy jade)
- TFT LCD - animations and information
- 16mb USB C Pi Pico
- Hotswap sockets
- Ortholinear
- Microsd card socket - expanding storage
- ec11 Rotary Encoder
- QMK (keyboard intended to be easily customizable and versatile)

# Schematic
<img width="1136" height="788" alt="Screenshot 2026-08-07 152231" src="https://github.com/user-attachments/assets/e974c058-d6ab-43f0-8031-a578f59e1b14" />

# PCB (silkscreen)
<img width="1526" height="425" alt="Screenshot 2026-08-04 191510" src="https://github.com/user-attachments/assets/ca65f309-c6ec-4189-b90a-41b1e7d3ced4" />
<img width="1663" height="493" alt="Screenshot 2026-08-04 191330" src="https://github.com/user-attachments/assets/b0e7ea01-7cd7-45d1-bece-d5a9dd211789" />

# Firmware (MAINLY WIP)
<img width="888" height="301" alt="Screenshot 2026-08-09 140202" src="https://github.com/user-attachments/assets/d3684a31-a165-43bb-853a-3fd23907d670" />
Need to remake the layout due to losing the tab and being unable to use the other file, or I need to test it on the website again.
Keyboard layout needed to make Firmware development easier with the QMK configurator.

# Notes
The keyboard's case was designed with a good amount of clearance to make up for any tolerance issues, but that might lead to fitment issues, so try to use glue or filler items to help the keyboard come together cleaner. Although the large parts are made with clearance in mind, smaller parts like the screen support might have tight clearances, so don't be afraid to sand it down or cut off some extra bits of plastic if they don't fit.
Pay attention to how and where the small components solder to (resistors, capacitors, or the mcp), and make sure the solder doesn't short.
Try to keep an eye on how high the pico sits on the board to not make it hit the case or put too much stress on the pins if the pins are slightly off from spec, pushing them down too far might put stress on the attachment points for the pins on the pico.

# Reflection
Although the project is overall much simpler than what I aim to do for the future, it definitely helped me kick start PCB designing and showed me how to make a finished product (for the most part). It isn't perfect, and I knew that, especially since how rigid hardware can be could affect it's versatility and how future proof it is, meanwhile software can be improved constantly, and that's why I aimed for a mostly software centric keyboard, and looking back I think my fears are pretty exaggerated and unfounded in some areas, but my general prediction was true, and my lack of skill with designing parts for the case, mounting holes, or clearances showed a lot, however it is something I wish to improve on for future projects, and my keyboard showed me some issues I can look at for now. 

I think the main difficulty with the project that's worse than designing the hardware was rather finding the parts that were cheap but reliable to get, as some parts seemed cheap but did not have a reliable stock, or had enormous shipping fees (though I did have to compromise on a few things for that due to no other alternatives, and a large portion of cost came from shipping itself unfortunately from things like JLPCB and Aliexpress). This project has showed me where to start now with planning for parts and the overall components I could realistically use, something that's harder to be flexible with than even designing parts for a project, like designing the case around a certain screw/hot insert dimension.

There were also easy things that I really enjoyed to do, like placing down the footprints for the pcb, routing, adding silkscreen art, and designing some simple sections of the hardware (especially decoration, like the waves on the screen case), they were mostly enjoyable outside of trying to find settings or tools for a specific action, but I learned to use onshape and kicad decently now. 

Overall, this project really helped me jump into designing something functional and useful, letting me learn to use software like onshape and kicad, and create a BOM and work out issues with how realistic it would be, the experience is really valuable for future projects I plan on doing. The risks I took for this project like using a TFT LCD and a Microsd socket were confusing and scary due to the probability of missing something essential or something that would protect them, but the risk seems worth it as now I know about pull up resistors, decoupling capacitors, ground pour, and how to better go about routing and placing components to make them as clean as possible (but I won't lie, I like how my PCB looks rendered in white with the routes from the MCP, minus the large amount of small route sections visible, but I'm sure cleaner routing is better looking). Using my experience so far, I wish to make more projects and have them come into the real world, hopefully pushing them to be more and more reliable, efficient, and compact.
