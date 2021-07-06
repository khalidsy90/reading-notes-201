# Transform

```css
transform: scaleY(0.4);
```

Defines how the element is transformed.

Removes any transformation.

```css
transform: none;
```

--------------------

Move the element on the horizontal axis.

```css
transform: translateX(40px);
```

-----------------------

Move the element on the vertical axis.

```css
transform: translateY(20px);
```

------------------

You can use percentage values: the percentage is relative to the element itself, and not the parent.

```css
transform: translateY(100%);
```

------------------

You can use translate() with two values:

the first value is for the horizontal axis
the second value is for the vertical axis

```css
transform: translate(20px, -10%);
```

----------------------

Scale the element on the horizontal axis.

```css
transform: scaleX(1.5);
```

------------------

Scale the element on the vertical axis.

```css
transform: scaleY(0.4);
```

---------------

You can use negative values: it will invert the element.

```css
transform: scaleY(-2);
```

------------

You can use ```scale()``` with two values:

the first value is for the horizontal axis
the second value is for the vertical axis
By using the same value for both, you can scale proportionally.

```css
transform: scale(0.8, 0.8);
```

-----------

Rotate the element.

You can use:

degrees from 0 to 360deg
gradians from 0 to 400grad
radians from 0 to 2πrad
turns from 0 to 1turn

```css
transform: rotate(45deg);
```

----------------

Skew the element on the horizontal axis.

```css
transform: skewX(15deg);
```

-------------------

Skew the element on the vertical axis.

```css
transform: skewY(45deg);
```

------------------

You can use skew() with two values:

the first value is for the horizontal axis
the second value is for the vertical axis

```css
transform: skew(10deg, -20deg);
```

-------------------

You can combine multiple transformations by separating them with a space

```css
transform: rotate(5deg) scale(1.1, 1.1) translate(-20%, 30px);
```

-------------
------------

# Transition

**CSS transitions allows you to change property values smoothly, over a given duration.**

Transition properties:

1. transition
2. transition-delay

--------

The transition will wait 1 seconds, and thus start right away.

```css
transition-delay: 1s /1000ms ;
```

we cane use ```s``` or ```ms``` to set the time

3. transition-duration

Defines how long the transition lasts.

The transition will last 1 seconds, and is thus instant.

```css
transition-duration: 0s/1000ms;
```

we cane use ```s``` or ```ms``` to set the time

---------

4. transition-property

Defines which properties will transition.

The element will transition all properties:

background
color
transform

```css
transition-property: all;
```

or we can select any proprty from pervious one

5. transition-timing-function

Defines how the values between the start and the end of the transition are calculated.

The transition starts slowly, accelerates in the middle, and slows down at the end.

```css
transition-timing-function: ease;
```

**ease-in** : The transition starts slowly, and accelerates gradually until the end.
**ease-out** :The transition starts quickly, and decelerates gradually until the end.
**ease-in-out** :Like ease, but more pronounced.
The transition starts quickly, and decelerates gradually until the end.
**step-start** :The transition jumps instantly to the final state.
**step-end** : The transition stays at the initial state until the end, when it instantly jumps to the final state.
**```step(Integer,end)```** : By using ```steps()``` with an integer, you can define a specific number of steps before reaching the end. The state of the element will not vary gradually, but rather jump from state to state in separate instants.

----------------------------

# Animation

The animation property in CSS can be used to animate many other CSS properties such as color, background-color, height, or width. Each animation needs to be defined with the ```@keyframes``` at-rule which is then called with the animation property

### Sub-properties
* animation-name: declares the name of the @keyframes at-rule to manipulate.

* **animation-duration**: the length of time it takes for an animation to complete one cycle.

* **animation-timing**-function: establishes preset acceleration curves such as ease or linear.

* **animation-delay**: the time between the element being loaded and the start of the animation sequence (cool examples).

* **animation-direction**: sets the direction of the animation after the cycle. Its default resets on each cycle.

* **animation-iteration-count**: the number of times the animation should be performed.

* **animation-fill-mode**: sets which values are applied before/after the animation.

* _For example_, you can set the last state of the animation to remain on screen, or you can set it to switch back to before when the animation began.

* **animation-play-state**: pause/play the animation.
