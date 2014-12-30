Project Description
-------------------

BigfootCSS is a set of helper CSS classes used to aid in the rapid creation of prototype user interfaces. It was built with simplicity and minimum footprint in mind.



**It does three things very well:**

1. Everything is defined as classes. It will not interfere with other styles unless explicitly applied.
2. Classes are single purpose, for example "xl" defines the font size to be Extra Large and nothing else. There are some compound classes, but they are minimum.
3. Does its best to apply regardless of target. When a class is assigned it does its best to ensure it applies whether you assign it to an Input, an Anchor tag, paragraph, or a table cell.

**Here is a partial list of what's included:**

As I said before these classes try to fix the problem of being overridden by element direct styling typical in a, input, td, select, and textarea tags. When you assign one of these classes to any element, it insures that it takes precedence.

*Font Size:*
s = small (13px)
xs = extra small (10px)
xxs = extra extra small (9px)
m = medium (16px)
l = large (19px)
xl =extra large (24px)
xxl = extra extra large (32px)

*Floats:*
To float elements left or right simply apply these classes to the element. Remember to wrap them with a container that has the clearfix class applied as in the example above.
fl = float left
fr = float right

*Widths, Heights, Padding and Margins:*
I know that some of you will balk at the idea of classes with preset sizes, but before you decide to start hurling stones, remember what I said before, every class that is there, is there because I use it often and find it to simplify and speed up my development. Like I’ve said this is a good middle ground before custom css rules for everything, and inline styles (which are evil).

w{number} = Sets the width of the element to the {number} of pixels specified. for example w25, sets the width of the element to 25px.  Numbers from 1-10 are in 1 pixel increments, 10-200 are in 5 pixel increments and 200-600 are in 25 pixel increments and 600-980 are in 10 pixel increments. With the exception of the standard ad sizes as found here
wp{number} = Sets the width of the element in percentages of it’s parent’s size. 1-10 and 95-100 are in 1% increments, the reset are in 5% point increments.
h{number} = Sets the height of the element in pixels. Numbers from 1-31 are in 1 pixel increments, from 30-250 are in 5 pixel increments, 250-600 are in 10 pixel increments
m{number} = Sets the margin for an element to the specified number. Numbers from 1-10 are in 1 pixel increments, 10-50 are in 5 pixel increments.
mt{number} , mr{number}, mb{number}, ml{number} = Sets the margin-[top, right, bottom, left] correspondingly. Numbers from 1-10 are in 1 pixel increments, 10-50 are in 5 pixel increments.
p{number} = Sets the padding for an element to the specified number. Numbers from 1-10 are in 1 pixel increments, 10-50 are in 5 pixel increments.
pt{number} , pr{number}, pb{number}, pl{number} = Sets the padding-[top, right, bottom, left] correspondingly. Numbers from 1-10 are in 1 pixel increments, 10-50 are in 5 pixel increments.


*Colors and Backgrounds:*
These are particularly useful in application development, as you often want to change the color or background to a preset set of colors, but it is not imperative that you be extremely precise with the color as you would with the palette of a hand crafted site. In these cases having some preset colors greatly improves the consistency and speed with which you can achieve element relevance through design in your applications.

bg{color} = stands for background-color and then the color specified. colors included are: white, black, light, dark, hl (which means highlight, sets the background to a light yellow), the colors are as described by their name.
black, white, red, xdard, dark, light, light[1-3], xlight = Sets the color css attribute of elements (including overriding the anchor tag color if applied to an anchor) to the appropriate color.

*Display and Position:*
 
hide = sets the display property of the element to none
block = sets the display property of the element to block
inline = sets the display property of the element to inline
inlineb = sets the display property of the element to inline-block
prel = sets the position to relative
pabs = sets the position to absolute
pfixed = sets the position to fixed
pstatic = sets the position to static

*Text alignment:*
 
tr = text-align: right
tl = text-align: left
tc = text-align: center
tj = text-align: justify
tvt = vertical-align: top
tvc = vertical-align: middle
tvb = vertical-align: bottom

*Miscellaneous Classes:*
 
pointer = sets the cursor to be the pointer when the mouse is over this element
cnomal = sets the mouse cursor to the normal sate
b = set the font-weight to bold
i = sets the contained text to italic
nowrap =adds text-whitespace: nowrap
strike = adds text-decoration: line-through
hlist = makes an unordered list’s <ul> elements display inline and horizotally, useful when creating menu and other horizontal use of <ul>
tablemin = turns a properly formatted table (one that uses the <thead> <th> and <tbody> elements) into a nicely displayed one by adding formatting to it in a very simplistic style
noscroll = sets the overflow to hidden in order to hide the scroll bar.
scroll = sets the showing of scroll bar to auto, (overflow: auto)
hscroll = shows the horizontal scroll bar
vscroll = shows the vertical scroll bar