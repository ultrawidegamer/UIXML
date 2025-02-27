<div align="center">
  <img src="https://github.com/ultrawidegamer/UIXML/blob/main/logo.png" alt="logo" width="400" height="400">
  <br><br>
  <div>Develop UIX panels in Resonite using XML</div>
</div>

<br><br>

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


## Checkbox
A simple clickable box used for boolean data.

| **Attribute**   | **Type**   | **Description** |
|-----------------|------------|-----------------|
| color          | ColorX     | Sets the color of the checkbox. |
| minheight      | Float      | Minimum height of the checkbox. |
| minwidth       | Float      | Minimum width of the checkbox. |


## Image
Embeds an image into the UI.

| **Attribute**   | **Type**   | **Description** |
|-----------------|------------|-----------------|
| uri            | Uri        | URI of the image to display. |
| minheight      | Float      | Minimum height of the image. |
| minwidth       | Float      | Minimum width of the image. |


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
- **DateTimeUser**: host, local, <any user id>
- **TextHorizontalAlignment**: left, center, right, justify
- **TextVerticalAlignment**: top, middle, bottom


## User Icon
Displays a user's profile picture.

| **Attribute**   | **Type**   | **Description** |
|-----------------|------------|-----------------|
| user           | UserIconUser   | Specifies the user for whose profile picture to display. |
| minheight      | Float      | Minimum height of the user icon. |
| minwidth       | Float      | Minimum width of the user icon. |

### Relevant Types:
- **UserIconUser**: local, host, <any user id>


## Box
A container that holds no content and can be used to organize UI elements.

| **Attribute**   | **Type**   | **Description** |
|-----------------|------------|-----------------|
| minheight      | Float      | Minimum height of the box element. |
| minwidth       | Float      | Minimum width of the box element. |

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


## Loading
An element that, when enabled, disables all UI elements inside and shows a loading spinner.

| **Attribute**   | **Type**   | **Description** |
|-----------------|------------|-----------------|
| minheight      | Float      | Minimum height of the layout. |
| minwidth       | Float      | Minimum width of the layout. |
| color          | ColorX     | Color of the loading spinner. |

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
