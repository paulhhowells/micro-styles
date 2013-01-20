css micro-styles
================

CSS micro-styles is a naming convention. Each micro-style is invariably a class containing a single rule.  The class name is constructed as a contraction of the CSS rule.

## prototyping

I have often found the speed and clarity of micro-styles useful while prototyping.  For example, you might perhaps be using a baseline of 20px and have a need to test how a Margin Bottom of 20 pixels rule would look:

    .mb-20 {margin-bottom: 20px;}

'margin-bottom' becomes 'mb', and '20px' follows the hyphen as '20'

Another example could be that you are wondering if a Padding Left and Right of 10px would complement your grid, so you might create:

    .pl-10 {padding-left: 10px;}
    .pr-10 {padding-right: 10px;}

'padding-left' becomes 'pl'
'padding-right' becomes 'pr'

Other types of micro-styles you might find useful:

    .c-l {clear: left;}
    .c-b {clear: both;}

    .f-l {float: left;}
    .f-r {float: right;}

    .mr-16 {margin-right: 16px;}
    .pt-0 {padding-top: 0;}
    .w-50pc {width: 50%;}

As the prototype transforms into a design I would suggest that margin, padding, clear and float micro-styles should disappear from the mark-up, their rules finding a home in other classes.

## systems

Used as a naming convention within a framework or system, micro-styles may function excellently within finished designs as well as prototypes.  Again, their key qualities should be brevity (for speed & convenience of writing) and clarity of purpose.

Take a look at [Unit](https://github.com/paulhhowells/unit) as an example of a grid system using micro-styles, and [Ink](https://github.com/paulhhowells/unit) as a font-size & baseline system of micro-styles.  In these examples .u-8 creates a column 8 units wide, and .f-14 sets the font-size to an ems value equivalent to 14px.

## a few final words

CSS micro-styles are intended as a precision tool for a small domain of tasks. It is not a convention I would encourage being applied to the lump of a design’s CSS rules.  (If you’re rethinking how you write CSS take a look at [SMACSS](http://smacss.com/)). Just as in HTML and Javascript, legibility is invaluable!  Applied carefully (and with judicious use of comments) micro-styles can be of as much utility to the other folk who will read and work on the CSS you create as to yourself.