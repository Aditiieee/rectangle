# rectangle
position: absolute;:

This positions the element in relation to its closest positioned ancestor (excluding the static positioned elements). If no positioned ancestors are present, it will position relative to the initial containing block (usually the viewport).
top: 50%; and left: 50%;:

These set the top-left corner of the element to be positioned at 50% of the height and 50% of the width of its closest positioned ancestor, respectively. Now, this alone will not center the element. Instead, its top-left corner will be at the center point of its parent, which means the element will be down and to the right of where we want it to be.
transform: translate(-50%, -50%);:

This is where the magic happens. The translate function of the transform property is used to move the element left/up by 50% of its own width/height.
-50% for the X-axis (translateX) shifts the element left by half of its width.
-50% for the Y-axis (translateY) shifts the element up by half of its height.
When combined with the top and left values, this ensures that the element is perfectly centered, no matter its size.


Relative Position: Setting the top, right, bottom, and left properties of an element with position: relative; property will cause it to adjust from its normal position. The other objects or elements will not fill the gap.
Absolute Position: An element with position: absolute; will cause it to adjust its position with respect to its parent. If no parent is present, then it uses the document body as parent.
Fixed Position: Position: fixed; property applied to an element will cause it to always stay in the same place even if the page is scrolled. To position the element we use top, right, bottom, left properties.


CSS transitions provide a way to control animation speed when changing CSS properties. Instead of having property changes take effect immediately, you can cause the changes in a property to take place over a period of time. For example, if you change the color of an element from white to black, usually the change is instantaneous. With CSS transitions enabled, changes occur at time intervals that follow an acceleration curve, all of which can be customized.
transition-property
Specifies the name or names of the CSS properties to which transitions should be applied. Only properties listed here are animated during transitions; changes to all other properties occur instantaneously as usual.

transition-duration
Specifies the duration over which transitions should occur. You can specify a single duration that applies to all properties during the transition, or multiple values to allow each property to transition over a different period of time.

transition-timing-function
Specifies a function to define how intermediate values for properties are computed. Easing functions determine how intermediate values of the transition are calculated. Most easing functions can be specified by providing the graph of the corresponding function, as defined by four points defining a cubic bezier. You can also choose easing from Easing functions cheat sheet.

transition-delay
Defines how long to wait between the time a property is changed and the transition actually begins.
