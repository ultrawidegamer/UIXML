<div align="center">
  <img src="https://github.com/ultrawidegamer/UIXML/blob/main/logo.png" alt="logo" width="400" height="400">
  <br><br>
  <div>Develop UIX panels in Resonite using XML</div>
</div>

<br>

# How to Use 

1. Spawn UIXML Parser in Resonite from my public folder (Items/UIXML) <br>
resrec:///U-ultrawidegamer/R-b6fe258a-ca9f-4822-83b8-f7e6dba2c89b

2. Start typing UIXML into the parser item or provide it with a URL to your hosted UIXML code

3. Click generate to see your generated UIX panel

<br>

# Elements

## Canvas
A wrapper for all UI elements, which allows rendering. The default content layout is horizontal.

| **Attribute**   | **Type**   | **Description** |
|-----------------|------------|-----------------|
| height         | Float      | Specifies the height of the canvas. |
| width          | Float      | Specifies the width of the canvas. |
| background     | ColorX     | Sets the color of the back and border of the canvas. |
| border         | Float      | Specifies the size of the canvas border. |
| font           | Uri        | Defines the font used in the canvas. |
| logo           | Uri        | Sets the logo displayed on the canvas. |
| color          | ColorX     | Sets the color of the panel content. |
| spacing        | Float      | Defines the spacing between child elements. |
| padding        | Float      | Sets the padding for all sides of the canvas. |
| padtop         | Float      | Sets the top padding for the canvas. |
| padright       | Float      | Sets the right padding for the canvas. |
| padbottom      | Float      | Sets the bottom padding for the canvas. |
| padleft        | Float      | Sets the left padding for the canvas. |

```xml
<canvas>
  UIXML elements go in here
</canvas>
```

## Text
Plain text to display static information.

| **Attribute**   | **Type**   | **Description** |
|-----------------|------------|-----------------|
| color          | ColorX     | Sets the text color. |
| fontsize       | Float      | Specifies the font size for the text. |
| minheight      | Float      | Minimum height of the text element. |
| minwidth       | Float      | Minimum width of the text element. |
| halign         | TextHorizontalAlignment | Horizontal alignment of the text. |
| valign         | TextVerticalAlignment   | Vertical alignment of the text. |

### Relevant Types:
- **TextHorizontalAlignment**: left, center, right, justify
- **TextVerticalAlignment**: top, middle, bottom

```xml
<canvas>
  <text>Hello world</text>
</canvas>
```

## Button
A simple clickable button for user interaction.

| **Attribute**   | **Type**   | **Description** |
|-----------------|------------|-----------------|
| color          | ColorX     | Sets the color of the button. |
| fontsize       | Float      | Specifies the font size of the button text. |
| minheight      | Float      | Minimum height of the button. |
| minwidth       | Float      | Minimum width of the button. |
| halign         | TextHorizontalAlignment | Horizontal alignment of the button. |
| valign         | TextVerticalAlignment   | Vertical alignment of the button. |

### Relevant Types:
- **TextHorizontalAlignment**: left, center, right, justify
- **TextVerticalAlignment**: top, middle, bottom

```xml
<canvas>
  <button>Hello world</button>
</canvas>
```

## Input
A basic input field for string data input.

| **Attribute**   | **Type**   | **Description** |
|-----------------|------------|-----------------|
| color          | ColorX     | Sets the input text color. |
| fontsize       | Float      | Specifies the font size for input text. |
| placeholder    | String     | Placeholder text when input is empty. |
| minheight      | Float      | Minimum height of the input field. |
| minwidth       | Float      | Minimum width of the input field. |
| halign         | TextHorizontalAlignment | Horizontal alignment of the input field. |
| valign         | TextVerticalAlignment   | Vertical alignment of the input field. |
| padding        | Float      | Padding inside the input field. |
| padtop         | Float      | Top padding inside the input field. |
| padright       | Float      | Right padding inside the input field. |
| padbottom      | Float      | Bottom padding inside the input field. |
| padleft        | Float      | Left padding inside the input field. |

### Relevant Types:
- **TextHorizontalAlignment**: left, center, right, justify
- **TextVerticalAlignment**: top, middle, bottom

```xml
<canvas>
  <input>Hello world</input>
</canvas>
```

## Checkbox
A simple clickable box used for boolean data.

| **Attribute**   | **Type**   | **Description** |
|-----------------|------------|-----------------|
| color          | ColorX     | Sets the color of the checkbox. |
| minheight      | Float      | Minimum height of the checkbox. |
| minwidth       | Float      | Minimum width of the checkbox. |

```xml
<canvas>
  <checkbox></checkbox>
<canvas>
```

## Image
Embeds an image into the UI.

| **Attribute**   | **Type**   | **Description** |
|-----------------|------------|-----------------|
| uri            | Uri        | URI of the image to display. |
| minheight      | Float      | Minimum height of the image. |
| minwidth       | Float      | Minimum width of the image. |

```xml
<canvas>
  <image uri="resdb:///c7a9e00aa0455709d29524c627f698e7d26261f3d41ea0cbf50df50a3e28caac.webp"></image>
</canvas>
```

## Slider
A range input that allows selecting a value between zero and one.

| **Attribute**   | **Type**   | **Description** |
|-----------------|------------|-----------------|
| format         | SliderFormat | Specifies the format for the slider values. |
| color          | ColorX     | Sets the color of the slider. |
| minheight      | Float      | Minimum height of the slider. |
| minwidth       | Float      | Minimum width of the slider. |

### Relevant Types:
- **SliderFormat**: vertical, horizontal

```xml
<canvas>
  <slider></slider>
</canvas>
```

## Datetime
Displays a date or time in a specified format.

| **Attribute**   | **Type**   | **Description** |
|-----------------|------------|-----------------|
| format         | DateTimeFormat | Specifies the format of the date/time. |
| user           | DateTimeUser   | User-related attribute to display the date/time. |
| use24hour      | Boolean    | Display time in 24-hour format. |
| color          | ColorX     | Sets the color of the datetime text. |
| fontsize       | Float      | Specifies the font size for the datetime text. |
| minheight      | Float      | Minimum height of the datetime element. |
| minwidth       | Float      | Minimum width of the datetime element. |
| halign         | TextHorizontalAlignment | Horizontal alignment of the datetime. |
| valign         | TextVerticalAlignment   | Vertical alignment of the datetime. |

### Relevant Types:
- **DateTimeFormat**: date, time, datetime, timedate
- **DateTimeUser**: host, local, any user id
- **TextHorizontalAlignment**: left, center, right, justify
- **TextVerticalAlignment**: top, middle, bottom

```xml
<canvas>
  <datetime></datetime>
</canvas>
```

## User Icon
Displays a user's profile picture.

| **Attribute**   | **Type**   | **Description** |
|-----------------|------------|-----------------|
| user           | UserIconUser   | Specifies the user for whose profile picture to display. |
| minheight      | Float      | Minimum height of the user icon. |
| minwidth       | Float      | Minimum width of the user icon. |

### Relevant Types:
- **UserIconUser**: local, host, any user id

```xml
<canvas>
  <usericon></usericon>
</canvas>
```

## Box
A container that holds no content and can be used to organize UI elements.

| **Attribute**   | **Type**   | **Description** |
|-----------------|------------|-----------------|
| minheight      | Float      | Minimum height of the box element. |
| minwidth       | Float      | Minimum width of the box element. |

```xml
<canvas>
  <vertical>
    <box></box>
    <image uri="resdb:///c7a9e00aa0455709d29524c627f698e7d26261f3d41ea0cbf50df50a3e28caac.webp"></image>
    <box></box>
  </vertical>
</canvas>
```

## Textarea
A multi-line input field for longer text.

| **Attribute**   | **Type**   | **Description** |
|-----------------|------------|-----------------|
| color          | ColorX     | Sets the color of the text in the textarea. |
| fontsize       | Float      | Specifies the font size for the text in the textarea. |
| placeholder    | String     | Placeholder text for the textarea. |
| minheight      | Float      | Minimum height of the textarea. |
| minwidth       | Float      | Minimum width of the textarea. |
| halign         | TextHorizontalAlignment | Horizontal alignment of the textarea. |
| valign         | TextVerticalAlignment   | Vertical alignment of the textarea. |
| padding        | Float      | Padding inside the textarea. |
| padtop         | Float      | Top padding inside the textarea. |
| padright       | Float      | Right padding inside the textarea. |
| padbottom      | Float      | Bottom padding inside the textarea. |
| padleft        | Float      | Left padding inside the textarea. |

### Relevant Types:
- **TextHorizontalAlignment**: left, center, right, justify
- **TextVerticalAlignment**: top, middle, bottom

```xml
<canvas>
  <textarea fontsize="30">
    Hello, this is a piece of text that I will continue writing until the end of time. Yep, it's never going to end. I really hope you enjoy reading, because this is going to be a long one and I mean really long longer than anything you've probably ever read in your life. Longer than your brain could even hold in seventy lifetimes, even. Not that I’m calling you stupid or anything! Sorry, that came out wrong. What I mean to say is that this message is just very long, and I’m sure your brain is perfectly evolved enough to hold at least 7% of what this message might contain. You know, I’m actually getting kind of tired, so just kidding! The text won’t go on forever, and you won’t have to worry about needing to develop your brain any more than it already is. :)
  </textarea>
</canvas>
```

## Scroll
A scrollable container that holds multiple UI elements and allows for scrolling.

| **Attribute**   | **Type**   | **Description** |
|-----------------|------------|-----------------|
| minheight      | Float      | Minimum height of the scroll container. |
| minwidth       | Float      | Minimum width of the scroll container. |
| halign         | LayoutHorizontalAlignment | Horizontal alignment of the scroll container. |
| valign         | LayoutVerticalAlignment   | Vertical alignment of the scroll container. |
| spacing        | Float      | Spacing between elements inside the scroll container. |
| padding        | Float      | Padding inside the scroll container. |
| padtop         | Float      | Top padding inside the scroll container. |
| padright       | Float      | Right padding inside the scroll container. |
| padbottom      | Float      | Bottom padding inside the scroll container. |
| padleft        | Float      | Left padding inside the scroll container. |

### Relevant Types:
- **LayoutHorizontalAlignment**: left, center, right, justify
- **LayoutVerticalAlignment**: top, middle, bottom, justify

```xml
<canvas>
  <scroll>
    <text fontsize="30">Hello, this is a piece of text 1</text>
    <text fontsize="30">Hello, this is a piece of text 2</text>
    <text fontsize="30">Hello, this is a piece of text 3</text>
    <text fontsize="30">Hello, this is a piece of text 4</text>
    <text fontsize="30">Hello, this is a piece of text 5</text>
    <text fontsize="30">Hello, this is a piece of text 6</text>
    <text fontsize="30">Hello, this is a piece of text 7</text>
    <text fontsize="30">Hello, this is a piece of text 8</text>
    <text fontsize="30">Hello, this is a piece of text 9</text>
    <text fontsize="30">Hello, this is a piece of text 10</text>
    <text fontsize="30">Hello, this is a piece of text 11</text>
    <text fontsize="30">Hello, this is a piece of text 12</text>
  </scroll>
</canvas>
```

## Dialog
An overlay element that shows a popup confirmation box.

| **Attribute**   | **Type**   | **Description** |
|-----------------|------------|-----------------|
| format         | DialogFormat | Specifies the format of the dialog content. |
| color          | ColorX     | Sets the color of the dialog elements. |
| fontsize       | Float      | Specifies the font size of the dialog text. |
| title          | String     | Title text for the dialog box. |
| positive       | String     | Text for the positive action button in the dialog. |
| negative       | String     | Text for the negative action button in the dialog. |
| minheight      | Float      | Minimum height of the dialog box. |
| minwidth       | Float      | Minimum width of the dialog box. |

### Relevant Types:
- **DialogFormat**: confirm, alert

```xml
<canvas>
  <dialog>text to show in dialog</dialog>
</canvas>
```

## Horizontal Layout
A layout that organizes UI elements horizontally from left to right.

| **Attribute**   | **Type**   | **Description** |
|-----------------|------------|-----------------|
| minheight      | Float      | Minimum height of the layout. |
| minwidth       | Float      | Minimum width of the layout. |
| halign         | LayoutHorizontalAlignment | Horizontal alignment of the layout. |
| valign         | LayoutVerticalAlignment   | Vertical alignment of the layout. |
| spacing        | Float      | Spacing between elements in the layout. |
| padding        | Float      | Padding for the layout. |
| padtop         | Float      | Top padding for the layout. |
| padright       | Float      | Right padding for the layout. |
| padbottom      | Float      | Bottom padding for the layout. |
| padleft        | Float      | Left padding for the layout. |

### Relevant Types:
- **LayoutHorizontalAlignment**: left, center, right, justify
- **LayoutVerticalAlignment**: top, middle, bottom, justify

```xml
<canvas>
  <horizontal>
    <text>one</text>
    <text>two</text>
    <text>three</text>
  </horizontal>
</canvas>
```

## Vertical Layout
A layout that organizes UI elements vertically from top to bottom.

| **Attribute**   | **Type**   | **Description** |
|-----------------|------------|-----------------|
| minheight      | Float      | Minimum height of the layout. |
| minwidth       | Float      | Minimum width of the layout. |
| halign         | LayoutHorizontalAlignment | Horizontal alignment of the layout. |
| valign         | LayoutVerticalAlignment   | Vertical alignment of the layout. |
| spacing        | Float      | Spacing between elements in the layout. |
| padding        | Float      | Padding for the layout. |
| padtop         | Float      | Top padding for the layout. |
| padright       | Float      | Right padding for the layout. |
| padbottom      | Float      | Bottom padding for the layout. |
| padleft        | Float      | Left padding for the layout. |

### Relevant Types:
- **LayoutHorizontalAlignment**: left, center, right, justify
- **LayoutVerticalAlignment**: top, middle, bottom, justify

```xml
<canvas>
  <vertical>
    <text>one</text>
    <text>two</text>
    <text>three</text>
  </vertical>
</canvas>
```

## Overlapping Layout
A layout where UI elements are layered on top of each other.

| **Attribute**   | **Type**   | **Description** |
|-----------------|------------|-----------------|
| minheight      | Float      | Minimum height of the layout. |
| minwidth       | Float      | Minimum width of the layout. |
| halign         | LayoutHorizontalAlignment | Horizontal alignment of the layout. |
| valign         | LayoutVerticalAlignment   | Vertical alignment of the layout. |
| padding        | Float      | Padding for the layout. |
| padtop         | Float      | Top padding for the layout. |
| padright       | Float      | Right padding for the layout. |
| padbottom      | Float      | Bottom padding for the layout. |
| padleft        | Float      | Left padding for the layout. |

### Relevant Types:
- **LayoutHorizontalAlignment**: left, center, right, justify
- **LayoutVerticalAlignment**: top, middle, bottom, justify

```xml
<canvas>
  <overlapping>
    <text>one</text>
    <text>two</text>
    <text>three</text>
  </overlapping>
</canvas>
```

## Loading
An element that, when enabled, disables all UI elements inside and shows a loading spinner.

| **Attribute**   | **Type**   | **Description** |
|-----------------|------------|-----------------|
| minheight      | Float      | Minimum height of the layout. |
| minwidth       | Float      | Minimum width of the layout. |
| color          | ColorX     | Color of the loading spinner. |

```xml
<canvas>
  <loading>
    <text>one</text>
    <text>two</text>
    <text>three</text>
  </loading>
</canvas>
```

<br><br>

# Project Name
UIXML is a term that refers to both the process of generating a user interface from XML and the use of UIXML as a UIX language within a markdown format.

<br>

# **WARNING:**

- **Canvas** is the required root UIXML element.
- All of the elements will have their attributes passed in as the string equivalent of their type.
- All element tags and attributes must be lowercase.
- Double quotes are a requirement when specifying attribute data.
- Special characters like `=" # \ <>` need to be escaped with a backslash (`\`).
