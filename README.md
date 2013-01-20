css micro-styles
================

Each CSS Micro Style is invariably a class containing a single rule.  The class name is constructed as a contraction of the CSS rule.

I have often found micro-styles useful while prototyping for their speed and clarity.  For example, you might perhaps be using a baseline of 20px and have a need to test how a Margin Bottom of 20 pixels rule would look:

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

As the prototype transforms into a design I would expect margin, padding, clear and float micro-styles to disappear from the mark-up, their rules finding a home in other classes. However I find grid and font-size microstyles to be of excellent use in finished designs.

Take a look at [Unit](https://github.com/paulhhowells/unit) as an example of a grid system using micro-styles, and [Ink](https://github.com/paulhhowells/unit) as font-size & baseline system of micro-styles.