Hey guys, whazzup? Remy here with ya codes!

Azathoth is our tentative name for the editor app for the RWAC project, and this is the first proper "functioning" update. This will be much further fleshed out,
I promise! I'm just a slow worker...

Currently, you can get an idea of what we intend to have as commands in the file named funcTable, viewable in Excel (but you will have to manually resize the 
column widths, they auto-shrink when the file is closed due to the format). You can also try making some isometric art, with the command "newPoint", used like 
this (you will have to press Enter twice to execute the command, currently trying to find a workaround): newPoint A 0 0 0

This will make a point at the spacial coordinates [1,1,1], but it will be rendered at [0,0], because of the isometric nature of the display system. Don't worry, 
it's supposed to have a lot ofempty space between it and the edges, for now coordinates are 1:1 with the screen's resolution (even it doesn't take up the whole screen 
outside of presentation mode). Currently it will be a 10x10 pixel square, and the color is randomized. If you can, Click on it! And it will say its name. Just in case 
you don't remember the name of the red one, or the electric green one, or the faded black denim one, or... you get the picture.

Next up is Lines and faces, followed by the full Shape class, so we can export to .obj or .amf filetypes. that way Slic3r will be able to convert those into G-Codes!
Yep, we are going to be adding Slic3r integration. 

But doesn't Slic3r have its own editor? yes it does. which brings me to what will make ours different: curve compatibility. Currently, Slic3r cannot handle 
"curved triangles" in the object files. That sounds like a challenge to me! Making the cartesian plane respect smooth surfaces that are curved and non-linear? 
Ok, you're on! Years of Minecraft, and if it's taught me anything, it is that any curve can be simulated by a grid representation that is fine enough. We aren't 
dealing with strict blocks, just non-"curved" surfaces. Is there such a thing without sanding down the object in question? Just having something close enough will suffice.

One last thing, Azathoth is not finalized, so it's still a project file and not a standalone app. DOWNLOAD THIS ENTIRE REPOSITORY, then open the appropriate GP Blocks 
Editor executeable, it should be GP-(operating system here). Then, open it with the built-in file browser, and run Azathoth.gpp. If you need to refresh the project, for 
example to reset it, click Go at the upper right corner of the screen.

And don't forget, we are using FCambus's Spleen for a font choice. We wanted something that looked ironically hackery and cheesey. If you have Linux already, you
probably already have it installed, otherwise follow the directions in that repo to get the low-rez monospace font of the future from the 90's!
