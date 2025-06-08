# Cascading Style Sheets

The styling system that makes your HTML look good instead of like a 2009 webpage.

## Cascading 

**User Agent Stylesheets**  
Contain browser defaults for styles. Lowest precedence - basically your base stats.

**User Stylesheets**  
Contain user preferences saved in the browser, which override user agent stylesheets.

**Author Stylesheets**  
Contain the CSS code we write. Highest level of precedence - your fed carry calling the shots.

## Declaration
**property: value;**  
The basic syntax for styling something.

## Declaration Block
```css
{
    color: blue;
    margin: 10px;
}
```
Group of declarations wrapped in curly braces. Your ability combo.

## Ruleset
```css
selector {
    property: value;
    property: value;
}
```
Complete CSS rule with selector and declaration block.

## Link Tag
**`<link>`**  
Self-closing tag for linking external stuff. Mostly used for CSS files. Goes in the `<head>` section.