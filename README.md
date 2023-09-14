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
