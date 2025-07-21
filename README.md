1.CSS/HTML ANIMATION
So,when using @keyframes we target the transition called before, these transitions contains transforms which are animation different styles.

animation> name	Name of @keyframes
animation> duration	How long the animation lasts
animation> delay	Time before the animation starts
animation> iteration-count	How many times to repeat
animation> direction	Normal, reverse, alternate
animation> fill-mode	Keeps end state (forwards)
animation> timing-function	Easing like ease-in-out

Basically Animation element work hand in hand with the key frame element which targets the transforms in the animation

MAIN FLEX PROPERTIES

1. display: flex;

Activates flex on the parent element.


---

2. flex-direction

Controls the direction of the items.

Value	Description

row	Horizontal (default)
row-reverse	Right to left
column	Vertical top to bottom
column-reverse	Bottom to top


.container {
  display: flex;
  flex-direction: column;
}

3. justify-content

Aligns items horizontally (main axis).

Value	Description

flex-start	Align to left/start
flex-end	Align to right/end
center	Center horizontally
space-between	Space between items
space-around	Space around items
space-evenly	Equal space around all items


.container {
  display: flex;
  justify-content: space-between;
}
4. align-items

Aligns items vertically (cross axis).

Value	Description

stretch	Default, fills height
flex-start	Top
flex-end	Bottom
center	Center vertically
baseline	Align text baselines


.container {
  display: flex;
  align-items: center;
}
5. flex-wrap

Controls if items wrap to the next line.

Value	Description

nowrap	Default, one line
wrap	Wrap to new lines if needed
wrap-reverse	Wrap in reverse direction


.container {
  display: flex;
  flex-wrap: wrap;
}
6. align-content

Aligns multiple lines (if flex-wrap: wrap).

Value	Description

stretch	Default
flex-start	Top
flex-end	Bottom
center	Center
space-between	Equal vertical space
space-around	Space around lines


🔗 FLEX ITEM PROPERTIES (children)

7. flex-grow

Item grows to fill space. Default is 0.

.box {
  flex-grow: 1; /* Each grows equally */
}

8. flex-shrink

Item shrinks if needed. Default is 1.

.box {
  flex-shrink: 1;
}
9. flex-basis

Initial size before growing/shrinking.

.box {
  flex-basis: 150px;
}
10. flex

A shorthand for:
flex: [flex-grow] [flex-shrink] [flex-basis];

.box {
  flex: 1 0 150px;
}
11. align-self

Override alignment for individual item.

.box:nth-child(2) {
  align-self: flex-end;
}



ROLLLING EYES EXPLANATIONS (JAVASCRIPT)
graphical eye tracker using HTML/CSS/JAVASCRIPT
getBoundingClientRect()\tab -Gets the eye's position and size\par
centerX, centerY\tab -Center of the eye\par
e.clientX, e.clientY\tab\tab -Position of the mouse\par
atan2(dy, dx)\tab\tab -Returns the angle from center to mouse\par
cos(angle), sin(angle)\tab\tab -Gets X and Y movement using trigonometry\par
style.left/top\tab    \tab -Moves the pupil visually inside the eye\par
trackEye() function for both eyes: for any action change\par
combine both the eyes and the pupils\par
trackEye(pupil1, eye1);\par
trackEye(pupil2, eye2);\par

Here is the Syntax for @keyframes:
keyframes animationName {
  0%   { /* styles at start */ }
  50%  { /* styles midway */ }
  100% { /* styles at end */ }
}

You can use:

UNDER percentages: 0%, 50%, 100%---- CAN BE SUBSTITUTED WITH KEYWORDS LIKE FROM OR TO.

2. ANIMATION TIMING
linear	Same speed throughout out the entire animation
Ease	Starts slow, speeds up, ends slow
Ease-in	Starts slow, then speeds up
Ease-out	Starts fast, then slows down
Ease-in-out	Slow-fast-slow
cubic-bezier()	Custom easing (advanced) this works like fade in and out.

