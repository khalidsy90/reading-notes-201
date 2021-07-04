# Images HTML

You can insert any image in your web page by using <img> tag. Following is the simple syntax to use this tag.

```<img src = "Image URL" ... attributes-list/>```
The ```<img>``` tag is an empty tag, which means that, it can contain only list of attributes and it has no closing tag .

### Set Image Border

By default, image will have a border around it, you can specify border thickness in terms of pixels using border attribute. A thickness of 0 means, no border around the picture.

```html
<!DOCTYPE html>
<html>

   <head>
      <title>Set Image Border</title>
   </head>
 
   <body>
      <p>Setting image Border</p>
      <img src = "/html/images/test.png" alt = "Test Image" border = "3"/>
   </body>
 
</html>
```

### Set Image Alignment

By default, image will align at the left side of the page, but you can use align attribute to set it in the center or right.

```html
<!DOCTYPE html>
<html>

   <head>
      <title>Set Image Alignment</title>
   </head>
 
   <body>
      <p>Setting image Alignment</p>
      <img src = "/html/images/test.png" alt = "Test Image" border = "3" align = "right"/>
   </body>
 
</html>
```

### centering IMAGES

To center an image, set left and right margin to auto and make it into a block element:

```css
.center {
  display: block;
  margin-left: auto;
  margin-right: auto;
  width: 50%;
}
```

### Background Image on a HTML element

To add a background image on an HTML element, use the HTML style attribute and the CSS background-image property:

```css
body {
  background-image: url('img_girl.jpg');
}
```

### Background Repeat

the image will repeat itself, horizontally and vertically, until it reaches the end of the element.

To avoid the background image from repeating itself, set the background-repeat property to no-repeat.

```css
body {
  background-image: url('example_img_girl.jpg');
  background-repeat: no-repeat;
}
```

### Background Cover

If you want the background image to cover the entire element, you can set the background-size property to cover.

Also, to make sure the entire element is always covered, set the background-attachment property to fixed:

This way, the background image will cover the entire element, with no stretching (the image will keep its original proportions):

```css
body {
  background-image: url('img_girl.jpg');
  background-repeat: no-repeat;
  background-attachment: fixed;
  background-size: cover;
}
```

### background position

The background-position property in CSS allows you to move a background image (or gradient) around within its container

```css
html {
  background-position: 100px 5px; 
}
```

### CSS background - Shorthand property

To shorten the code, it is also possible to specify all the background properties in one single property. This is called a shorthand property.

```css
body {
  background: #ffffff url("img_tree.png") no-repeat right top;
}
```

### CSS Linear Gradients

To create a linear gradient you must define at least two color stops. Color stops are the colors you want to render smooth transitions among. You can also set a starting point and a direction (or an angle) along with the gradient effect.

```css
background-image: linear-gradient(direction, color-stop1, color-stop2, ...);
```

### HTML figcaption tag

The ```<figcaption>``` element is used to provide a caption to an image.

It is an optional tag and can appear before or after the content within the ```<figure>``` tag.

Only one ```<figcaption>``` element can be nested within a ```<figure```> tag although the ```<figure```> element itself may contain multiple other elements like ```<img>``` or ```<code>```.

The ```<figcaption>``` element is used with ```<figure>``` element and it can be placed as the first or last child of the ```<figure>``` element.

```html
<figure>  
  <img src="https://static.javatpoint.com/htmlpages/images/tajmahal.jpg" alt="Taj Mahal"/>  
<figcaption>Fig.1.1 - A front view of the great Taj Mahal in Agra.</figcaption>  
</figure>  
```

---------------------

# 9 Places to Insert Keywords on Your Website

### 1. In your header

      1. Title tags
      Title tags are the first places that the search engines will scan, and they are what appear as the actual link on the search engine results page. This is one of the most important places to emphasize your keywords, so make sure that the title tag on each page uses your most important keywords.

      2. META description tag
      Within your header, there are a number of hidden META tags that only the search engines will see, and the META description tag is one of these hidden tags. On the search engine results page, you can generally see the META description tag by looking at the chunk of text underneath the link.

      3. META keywords tag
      It’s still being debated how much weight the search engines give to the META keywords tag. In the early days of search, websites used to cram this tag full of any and all keywords or keyword combinations, in the hopes that the search engines would grasp onto something.

### In your content

4. Headers and Sub-headers
One of my 10 tips for improving your titles and sub-headers is to put any keywords you’re using in them up front. Doing so not only emphasizes what comes in the content below, but is useful for people scanning through your website quickly. Just try to keep it clear, concise, and relevant when doing so.

5. Page content
Your page content is reason your website’s exists in the first place, and it’s the backbone of everything else on your website. It’s also what people link to (and links are another contributing factor to SEO) and what will draw people to your website in the first place.

One big consideration when writing your content is keyword density. While your best bet is to incorporate your targeted keyword phrase into your content as often as possible, you want to be careful not to overdo it. You’re not trying to sell your product to search engines; you’re trying to sell it to people, and if your content reads horribly, it can make a bad impression and most likely decrease the chance of making a conversion.

We’ve all seen websites where the keyword density is so high that the content reads horribly. As long as you’re simply aware of the phrase you’re targeting when you’re writing the content, you should end up with an adequate keyword density, probably within the 3-5% range. It’s alright if the targeted keywords stand out when you read through your content; after all, that’s what the person was searching for, and seeing it emphasized will reinforce that they have the information they need to make their decision.

Also remember the 1-to-1 rule: 1 page of content should be optimized for 1 keyword.

6. Link text
One of my reasons for avoiding using “click here” in link text is that it’s not SEO-friendly. Search engines use the strength of your links in their algorithm, and one of the things that determines link strength is whether the link text using specific keywords in it.

Use specific keywords in your link text helps them estimate how relevant that link is. It also helps build the relevancy of a particular page to a particular keyword phrase.

With all of the places on your website where links are, this doesn’t apply solely to links within your page content. It applies to your main navigation links, to your breadcrumbs (as I mentioned already), to your footer links, etc. It’s all about association, and you want the search engines to associate certain keywords with your website in general and with specific pages on your website in particular.

Bonus places
7. Breadcrumbs
Another common navigation tool on websites, breadcrumbs can help people pinpoint where they are on your website, as well as how to get back to where they were previously. As with any place you have words on your website, your breadcrumbs are another opportunity for you to incorporate your keywords. Just make sure that the breadcrumb links provide enough detail about what the pages are, without being overly length – 1 to 3 words at most.

8. ALT and TITLE attributes
While these attributes were created for usability purposes, they don’t have to be used solely in those ways. They can also be used for SEO purposes in the sense that they’re another opportunity for you to incorporate additional text onto your page – text that contain the keywords you’re optimizing for.

I’ve written previously about using the ALT and TITLE attributes properly, but the important point is that you shouldn’t write them with only the search engines in mind.

Keep them relevant to the element in question, and don’t use them to either duplicate content elsewhere on the page or to stuff them full of keywords to the point that they become completely unhelpful. Above all when it comes to them, think usability first, SEO second.

9. Embedded file names
What I’m referring to as embedded file names are things like web pages, images, etc. These aren’t necessarily things that people will see within your actual content – they’re just ways that you can get more keywords onto your page.

How you write file names should be a no-brainer, but it’s important that you not give them a generic or vague label. People will see the file name of a web page when they hover over a link, so using a file name that contains the keywords that the page is about is useful from usability purposes. (This is one of the main reasons why you should enable your permalinks in WordPress; with HTML websites, you have an easier time controlling the file names.

When it comes to images, why name your image files something vague such as “image01.jpg” when you can name it something that includes a keyword instead? It’s not something that someone will see or that will really make a difference, but it’s just another spot where you can get the keyword onto the page for the search engines to see it.
