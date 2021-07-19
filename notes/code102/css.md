# CSS Styling

**CSS** stands for Cascading Style Sheets. It's gives one the ability to visually transform your html into stunning website. It also has a pretty simple syntax.

### Syntax

CSS is a rule-based language — you define rules specifying groups of styles that should be applied to particular elements or groups of elements on your web page. For example "I want the main heading on my page to be shown as large blue text."

The following code shows a very simple CSS rule that would achieve the styling described above:

```
h1 {
  color: blue;
  font-size: 3rem;
}
```
The rule starts with a *selector*. This selects the HTML element that we are going to style. In this instance we are styling level one headings.

Then there's a set of curly braces `{ }`. Inside of those will be one or more declarations, which take the form of property and value pairs. Each pair specifies a property of the element(s) we are selecting, then a value that we'd like to give the property.

The property is before the colon; the value is after the colon. CSS properties have different allowable values.
A CSS stylesheet will typically contain many such rules, written one after the other.


```
h1 {
  color: red;
  font-size: 3rem;
}

p {
  color: #474747;
}
```

### Adding CSS to Your Webpapge

The three ways of inserting a style sheet are:

- External CSS
- Internal CSS
- Inline CSS

#### External CSS

External CSS is what you'll most commonly see on the web.

External styles are defined within the `<link>` element, inside the `<head>` section of an HTML page:
```
<html>
  <head>
    <link rel="stylesheet" href="mystyle.css">
  </head>
  <body>
    <h2>This is a heading</h2>
    <p>This is a paragraph</p>
  </body>
</html>
```
External style sheets must be saved with a .css extenstion & should not contain any HTML tags.

#### Internal CSS

Internal CSS is defined inside the `<style>` element, inside the `<head>` section of an HTML page:
```
<html>
  <head>
    <style>
      body {
        background-color: #a78f5e;
      }

      h2 {
        color: #BCBCBC;
        margin-left: 20px;
      }
    </style>
  </head>
  <body>
    <h2>This is a heading</h2>
    <p>This is a paragraph</p>
  </body>
</html>
```

#### Inline CSS

Inline CSS may be used to apply a unique style for a single element.

To use inline styles, add the style attribute to the relevant element. The style attribute can contain any CSS property.

```
<html>
<body>

<h2 style="color:purple;text-align:right;">This is a heading</h1>
<p style="color:grey;">This is a paragraph.</p>

</body>
</html>
```

#### The Cascade

The cascading part of CSS is that all the styles in a page will "cascade" into a new "virtual" style sheet by the following rules, where number one has the highest priority:

1. Inline CSS
2. External & Internal CSS
3. Browser Defaults
