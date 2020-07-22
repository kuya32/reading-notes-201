# Read: 14a - CSS Transforms, Transitions, and Animations

## Article on CSS Transforms

- Elements may be distorted, or transformed, on both a two-dimensional plane or a three-dimensional plane.
- The transform property accepts a handful of different values
  - transform: rotate(xdeg);
  - transform: scale(x); or scaleX(x); or scaleY(x); or scale(x, y);
  - transform: translateX(x); or translateY(x);
    - Change the position of an element on the horizontal or vertical axis
  - transform: skewX, skewY, skew(x, y);
    - Used to distort elements on the horizontal, vertical or both axis
  - You can do combinations of different transform properties
- transform-origin
  - Changes the default origin position which is defaulted at dead center
- Perspective (vanishing point)
  - Use the perspective value within the transform property on individual elements
  - The lower the value the closer the perspective appears, thus creating a high intensity perspective and a large three-dimensional change.
- perspective-origin 
  - Changes the default origin position which is defaulted at dead center
- Three-dimensional transforms
  - Same as 2D but adds the z-axis
- Transform-style
  - The **transform-style** property needs to be placed on the parent element, above any nested transforms. The **preserve-3d** value allows the transformed children elements to ***appear*** in their own three-dimensional plane while the flat value forces the transformed children elements to lie flat on the two-dimensional plane

## Article on CSS Transitions & Animations

- We can create transitions and animations in CSS with some properties. The first is transition which have four:
  - Transition-property
    - Determines exactly what properties will be altered in conjunction with the other transitional properties
    - Not all properties may be transitioned, only properties that have an identifiable halfway point
  - Transition-duration
    - Duration in which a transition takes place
    - value of this property can be set using general timing values, including seconds (s) and milliseconds (ms)
  - Transition-timing-function
    - Used to set the speed in which a transition will move. It has four key values. 
    - Linear
      - Identifies a transition moving in a constant speed from one state to another
    - Ease-in
      - Identifies a transition that starts slowly and speeds up throughout the transition
    - Ease-out
      - Identifies a transition that starts quickly and slows down throughout the transition
    - Ease-in-out.
      - Identifies a transition that starts slowly, speeds up in the middle, then slows down again before ending
  - Transition-delay
    - Delay sets a time value, seconds or milliseconds, that determines how long a transition should be stalled before executing
  - Transition Shorthand example
    - ```transition: background .2s linear, border-radius 1s ease-in 1s;```
- When more control is required, transitions need to have multiple states. This is where **animations** come in.
- The easiest way for determining styles for different states is by using the **:hover, :focus, :active, and :target** pseudo-classes
  - @keyframes rule
    - Sets multiple points at which an element should undergo a transition
    - @keyframes rule includes the **animation name, any animation breakpoints, and the properties intended to be animated**
  - Animation name
    - Applied to the element in which the animation is to be applied to
  - Other properties work just like transition but with animation
  - Animation-iteration-count
    - To have an animation repeat itself numerous times
    - The values take integers or infinite 
  - Animation-direction
    - Declare the direction an animation completes.
    - Values include **normal, reverse, alternate, and alternate-reverse**
  - Animation-play-state
    - Allows an animation to be played or paused using the running and paused keyword values respectively
  - Animation-fill-mode
    - Identifies how an element should be styled either before, after, or before and after an animation is run
    - Values accepted are:
      - None
        - Will not apply any styles to an element before or after an animation has been run
      - Forward
        - Will keep the styles declared within the last specified keyframe
      - Backwards
        - Will apply the styles within the first specified keyframe as soon as being identified, before the animation has been run
      - Both
        - Will apply the behaviors from both the forwards and backwards values
  - Shorthand for animation example
    - ```animation: slide 2s ease-in-out .5s infinite alternate;```

[Back to README](README.md)