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

