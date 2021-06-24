# Image in HTML

You can insert any image in your web page by using ```<img>``` tag. Following is the simple syntax to use this tag.

```<img src = "Image URL" ... attributes-list/>```
* The required alt attribute provides an alternate text for an image, if the user for some reason cannot view it (because of slow connection, an error in the src attribute, or if the user uses a screen reader).
* You can use the style attribute to specify the width and height of an image.
* You can use the style attribute to specify the width and height of an image.

--------------------
# color
We've already seen some properties in CSS that take color values
```css
p {
  color: red;
}
```
**There are several different ways to specify colors in CSS.**

1. Color Keywords
The first and easiest way to specify a color is using one of the 140 predefined color keywords specified in CSS.

The original 17 are listed below. An unsightly bunch...
```css
|Color|	Keyword	Hex Value |
|------|-------------------|
 black |	#000000
 gray	| #808080
 silver |	#c0c0c0
 white |	#ffffff
 maroon |	#800000
 red	| #ff0000
 purple	| #800080
 fuchsia	| #ff00ff
 green	| #008000
 ```


2. RGB
Most of you have probably heard about CMYK values for print design. RGB, which stands for red, green, and blue is the color model that monitors use. Since in web design we're primarily concerned with what web pages look like on screens, RGB is the color model we use.

3. RGBA
RGBA is all the rage.

    Seriously though, it's just like RGB, except with the addition of a fourth value: the alpha channel.

    The alpha value represents the level of transparency that the rgb color should have. It can be a value from 0 to 1 or a percentage from 0 to 100%. Note that you must specify RGBA instead of RGB.

4. HSL

    The HSL color model is one of the least used, but gaining traction because can be more intuitive to use when working with shades and color adjustments.

    HSL stands for: hue, saturation, and lightness

5. HSLA

    HSLA is simply the HSL color model with the addition of an alpha channel. This works exactly the same way as the alpha channel in RGBA.
```css
h1 {
   background-color: hsla(240, 25%, 50%, .5);
}
```

6. Hexadecimal

Probably the most common (yet least intuitive) way to specify colors in CSS is to use their hexadecimal (or hex) values. Hex values are actually just a different way to represent RGB values. Instead of using three numbers between 0 and 255, you use six hexadecimal numbers. Hex numbers can be 0-9 and A-F. Hex values are always prefixed with a # symbol.

Demonstrated here are some basic CSS rules rules using hex values.
```css
p { color: #000000; }     /* black */
h1 { color: #ffffff; }    /* white */
h1 { color: #aaaaaa; }    /* medium gray */
ul { color: #8050c8; }    /* purple */
```
------------------
# Contrast using CSS

The syntax for contrast is filter: contrast(value); Contrast takes percentage values between 0% to over 100%. A value of 100% results in no change to the image. Values less than 100% reduce the contrast of the image, whereas values greater than 100% increase the contrast of the image. Decimal values are also acceptable as input values. Below are a few examples of applying various contrasts to the image. As you can see at 70% the image is dimmer than the original image. As the contrast is increased the shadows get darker while the highlight tones of the image get brighter.

contrast(70%)                                        contrast(120%)

contrast(150% )                                       contrast(250%)

Brightness
The syntax for adjusting brightness is filter: brightness(value); Brightness like contrast takes percentage values ranging from 0% to above 100%. A value of 100% keeps the original image. Any value less than 100% dims the image, with a value of 0% resulting in a completely black image. Values over 100% increases the brightness of the image. Below is the image at four different brightness levels.

brightness(80%)                                       brightness(130%)

brightness(180%)                                   brightness(250%)

Conclusion
Images are a great way to enhance webpage content and communicate more effectively with users.  The CSS filter property can be used to create bright high contrasted images or dim low contrasted images quickly and easily.

## CSS Opacity / Transparency


The opacity property can take a value from 0.0 - 1.0. The lower value, the more transparent:

## CSS font Property
|Property/Value|Description|
|--------------|-----------|
|font-style |	Specifies the font style. Default value is "normal"|
|font-variant |	Specifies the font variant. Default value is "normal"|
|font-weight |	Specifies the font weight. Default value is "normal"|
|font-size/line-height	| Specifies the font size and the line-height. Default value is "normal"|
|font-family |	Specifies the font family. Default value depends on the browser|
|caption |	Uses the font that are used by captioned controls (like buttons, drop-downs, etc.)|
|icon |	Uses the font that are used by icon labels|
|menu |	Uses the fonts that are used by dropdown menus|
|message-box |	Uses the fonts that are used by dialog boxes|
|small-caption |	A smaller version of the caption font|
|status-bar |	Uses the fonts that are used by the status bar|
|initial |	Sets this property to its default value. Read about initial|
|inherit |	Inherits this property from its parent element. Read about inherit"|

```css
<p style="font:caption">The browser font used in captioned controls.</p>
<p style="font:icon">The browser font used in icon labels.</p>
<p style="font:menu">The browser font used in dropdown menus.</p>
<p style="font:message-box">The browser font used in dialog boxes.</p>
<p style="font:small-caption">A smaller version of the caption font.</p>
<p style="font:status-bar">The browser font used in the status bar.</p>
```

