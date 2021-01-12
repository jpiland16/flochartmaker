# flochartmaker
HTML5 rapid flowchart development tool

## Contents

 - [Purpose](#purpose)
 - [How to use](#how-to-use)
 - [Technical notes](#technical-notes)
 - [What you can expect](#what-you-can-expect-from-this-tool)

## Purpose
The motivation behind this tool was the lack of sufficient options for creating flowcharts quickly and easily. Hopefully, the simple keyboard shortcuts used by this program will make flowchart creation a much less arduous task.

## How to use

 - When the page is opened, the starting node is selected. You can begin typing the title of the first node.
 - To create a new node, press an arrow key while holding the CTRL key. The text in the new node will be automatically selected.
 - The CTRL key can also be used for moving from node to node. Moving from one node to an existing node will not create a new connection, even if the two nodes were previously unconnected.
 - To delete a node, press CTRL-Z. Currently, only nodes that are at the ends of a chain can be deleted. The starting node cannot be deleted.
 - To create an additional input to a node, press an arrow key while holding the CTRL and ALT keys. If there is not another node in that direction, then the action would be as if the ALT key was not pressed.
 - To change the shape of a node, press the TAB key while that node is selected. There are currently 5 shapes: rectangle, ellipse, parallelogram, diamond, and "connector." 
 - The connector node cannot display text (although it will save text you previously entered) and can only be used to illustrate connections between other nodes.
 - To change the fill color of a node, use the backtick (\`) key which is located in the top-left corner of the keyboard. Connector nodes do not display a fill color.
 - To add or remove the arrow pointing from one node __to__ the current node, press the SHIFT and TAB keys simultaneously while that node is selected. Currently, removal arrows created by the CTRL-ALT-ARROW method is not supported - the entire connection must be removed.
 
 ## Technical notes
  - The current implementation uses a __single-inheritance__ system to connect nodes. Multiple inputs to a node are allowed through the creation of invisible `pseudoNodes` which cannot be selected. This may be changed in the future to allow for easier removal of multiple inputs.

## What you can expect from this tool

### This tool will:
 - Allow you to use keyboard shortcuts to quickly create flowcharts
 - Make flowchart creation more fun (hopefully!)

### This tool will not:
 - Ask for a name and password
 - Ask you to pay for something
 - Allow you to "click and drag" to move shapes
 - Have confusing menu items
 - Have options to change fonts and colors (feel free to inspect element or download and change CSS!)
 - Be easily used on a mobile device without a physical keyboard
 - Save your flowcharts (it will warn you if you are about to close the tab)
 - Convert your flowcharts to an image (in the future, this might be an option. For now, screenshots are a great option!)