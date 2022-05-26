# CSS Transforms, Transitions, and Animations

- [CSS Transforms](https://learn.shayhowe.com/advanced-html-css/css-transforms/)

- [Transitions and Animations](https://learn.shayhowe.com/advanced-html-css/transitions-animations/)

- [8 Simple CSS3 Transitions That Will Wow Your Users](https://www.webdesignerdepot.com/2014/05/8-simple-css3-transitions-that-will-wow-your-users)

## Transforms

- **Transform** property comes in two different settings, two-dimensional and three-dimensional. Each of these come with their own individual properties and values

- **Transform Syntax** - including the transform property followed by the value. The value specifies the transform type followed by a specific amount inside parentheses

- **2D Transforms** - work on the x and y axes, known as horizontal and vertical axes
  - **Rotate** - provides the ability to rotate an element from 0 to 360 degrees. Positive values will rotate an element clockwise, and negative values will rotate the element counterclockwise
  - **Scale** - hange the appeared size of an element, any value between .99 and .01 makes an element appear smaller while any value greater than or equal to 1.01 makes an element appear larger
  - **Translate** - pushing and pulling an element in different directions without interrupting the normal flow of the document
  - **Skew** - distort elements on the horizontal axis, vertical axis, or both
  - **Combine Transforms** - list the transform values within the transform property one after the other without the use of commas

- **Transform Origin** - the default transform origin is the dead center of an element, to change this default origin position the transform-origin property may be used

- The **perspective** for each element can be thought of as a vanishing point, similar to that which can be seen in three-dimensional drawings

- **3D Transforms** - work on both the x and y axes, as well as the z axis. Helps define not only the length and width of an element, but also the depth. Use three new transform values, rotateX, rotateY, and rotateZ
  - **rotateX** value allows you to rotate an element around the x axis, as if it were being bent in half horizontally
  - **rotateY** value allows you to rotate an element around the Y axis, as if it were being bent in half vertically
  - **rotateZ** value allows an element to be rotated around the z axis

- **3D Scale** - elements may be scaled on the z axis

- **3D Translate** - translateZ, negative values will push an element further away on the z axis, resulting in a smaller element and positive values will pull an element closer on the z axis, resulting in a larger element

- **Shorthand** three-dimensional transforms, properties include rotate3d, scale3d, transition3d, and matrix3d

- To allow **nested elements** to transform in their own three-dimensional plane use the transform-style property with the preserve-3d value

- Set the **backface-visibility** property to hidden, and you will hide the element whenever it is facing away from the screen

## Transitions

- for a **transition** to take place, an element must have a change in state, and different styles must be identified for each state, use the :hover, :focus, :active, and :target pseudo-classes

- four **transition related properties** in total, including transition-property, transition-duration, transition-timing-function, and transition-delay

- **transition-property** property determines exactly what properties will be altered in conjunction with the other transitional properties

- **transition-duration** - The duration in which a transition takes place, the value of this property can be set using general timing values, including seconds (s) and milliseconds (ms)

- **transition-timing-function** - set the speed in which a transition will move, keyword values include linear, ease-in, ease-out, and ease-in-out.

- **transition-delay** - determines how long a transition should be stalled before executing

- **Shorthand** - Using the transition value alone, you can set every transition value in the order of transition-property, transition-duration, transition-timing-function, and lastly transition-delay

## Animations

- **Animations keyframes** - To set multiple points at which an element should undergo a transition, use the @keyframes rule

- The different keyframe breakpoints are set using percentages, starting at 0% and working to 100% with an intermediate breakpoint at 50%

- **Animation Name** - animation-name property is used with the animation name, identified from the @keyframes rule, as the property value, The animation-name declaration is applied to the element in which the animation is to be applied to

- declare an **animation-duration** property and value so that the browser knows how long an animation should take to complete, timing function and delay can be declared using the animation-timing-function and animation-delay properties

- **Iteration** - have an animation repeat itself numerous times the animation-iteration-count property, either an integer or the infinite keyword for the value

- declare the **direction** an animation completes using the **animation-direction** property with values including normal, reverse, alternate, and alternate-reverse

- **animation-play-state** property allows an animation to be played or paused using the running and paused keyword values

- **animation-fill-mode** property identifies how an element should be styled either before, after, or before and after an animation is run. Use values none, forwards, backwards, and both

- **Shorthand** - The order of values should be animation-name, animation-duration, animation-timing-function, animation-delay, animation-iteration-count, animation-direction, animation-fill-mode, and lastly animation-play-state

## Example Transitions

- Fade in:

        .fade
        {
            opacity:0.5;
        }
        .fade:hover
        {
            opacity:1;
        }

- Change color:

        .color:hover
        {
            background:#53a7ea;
        }

- Grow & Shrink:

        .grow:hover
        {
            -webkit-transform: scale(1.3);
            -ms-transform: scale(1.3);
            transform: scale(1.3);
        }

        .shrink:hover
        {
            -webkit-transform: scale(0.8);
            -ms-transform: scale(0.8);
            transform: scale(0.8);
        }

- Rotate Elements:

        .rotate:hover
        {
            -webkit-transform: rotateZ(-30deg);
            -ms-transform: rotateZ(-30deg);
            transform: rotateZ(-30deg);
        }

- Square to Circle:

        .circle:hover
        {
            border-radius:50%;
        }

- 3D Shadow:

        .threed:hover
        {
            box-shadow:
                1px 1px #53a7ea,
                2px 2px #53a7ea,
                3px 3px #53a7ea;
            -webkit-transform: translateX(-3px);
        transform: translateX(-3px);
        }

- Swing:

        .swing:hover
        {
            -webkit-animation: swing 1s ease;
            animation: swing 1s ease;
            -webkit-animation-iteration-count: 1;
           animation-iteration-count: 1;
        }

- Inset Border:

        .border:hover
        {
            box-shadow: inset 0 0 0 25px #53a7ea;
        }

[Return home](https://khofstetter94.github.io/reading-notes/)
