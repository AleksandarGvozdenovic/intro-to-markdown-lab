# The Anatomy of a CSS Selector

CSS selectors are patterns used to target HTML elements so you can style them. Understanding selectors is essential for effective CSS design.

## 1. Basic syntax

A CSS rule-set looks like this:


selector {
  property: value;
}
Selector: Specifies which HTML element(s) the rule applies to.

Property: The style attribute you want to change.

Value: The style you want to apply.

Example:

p {
  color: blue;
}
This will make all <p> elements have blue text.

2. Types of selectors
Element selector
Targets HTML elements by their tag name.

h1 {
  font-size: 2em;
}
Class selector
Targets elements with a specific class attribute. Prefix with a dot (.).

.button {
  background-color: green;
}
ID selector
Targets an element with a specific ID attribute. Prefix with a hash (#).

#header {
  padding: 20px;
}
Universal selector
Targets all elements on the page.

* {
  margin: 0;
  padding: 0;
}
Group selector
Targets multiple selectors at once.

h1, h2, h3 {
  font-family: Arial, sans-serif;
}
3. Combining selectors
You can combine selectors to target more specific elements.

Example:

div.content p {
  line-height: 1.5;
}
This targets all <p> elements inside a <div> with class "content".

4. Pseudo-classes and pseudo-elements
Pseudo-classes allow styling elements in a specific state.

a:hover {
  color: red;
}
Pseudo-elements target part of an element.

p::first-line {
  font-weight: bold;
}
5. Example
nav ul li a.active {
  text-decoration: underline;
}
This will underline active navigation links inside list items.

Tip: Organize your selectors logically, and keep them as specific as necessary to avoid unnecessary overrides.

For more CSS selector examples, check out the MDN CSS Selectors documentation.


---
