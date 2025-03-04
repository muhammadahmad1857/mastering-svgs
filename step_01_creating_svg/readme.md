# SVG Detailed Attribute Explanation

**Navigation:**  
- [Introduction](#introduction)  
- [Circle Attributes](#circle-attributes)  
- [Rectangle Attributes](#rectangle-attributes)  
- [Line Attributes](#line-attributes)  
- [Polygon Attributes](#polygon-attributes)  
- [Text Attributes](#text-attributes)  
- [Conclusion](#conclusion)

---

## Introduction

This document explains, in clear detail, the various SVG attributes used in our SVG Editor. It is designed for beginners, ensuring that every property—such as coordinate settings, size definitions, and styling options—is explained thoroughly. Whether you are learning about circles, rectangles, lines, or polygons, this guide will help you understand how each attribute contributes to the final rendered graphic.

---

## Circle Attributes

- **cx & cy**  
  - **What They Do:**  
    - `cx` specifies the x-coordinate (horizontal position) of the circle's center.
    - `cy` specifies the y-coordinate (vertical position) of the circle's center.
  - **Example:**  
    - With `cx="125"` and `cy="125"`, the center of the circle is positioned at 125 pixels from the left and 125 pixels from the top of the SVG canvas.

- **r (Radius)**  
  - **What It Does:**  
    - Defines the distance from the center of the circle to its edge.
  - **Example:**  
    - `r="100"` means the circle extends 100 pixels outward from its center.

- **stroke & stroke-width**  
  - **stroke:**  
    - Sets the color of the circle's outline (border).
  - **stroke-width:**  
    - Specifies the thickness of that outline.
  - **Example:**  
    - `stroke="black"` with `stroke-width="3"` produces a black border that is 3 pixels thick.

- **fill**  
  - **What It Does:**  
    - Determines the color used to fill the interior of the circle.
  - **Example:**  
    - `fill="yellow"` fills the circle with a yellow color.

---

## Rectangle Attributes

- **x & y**  
  - **What They Do:**  
    - `x` determines the horizontal position of the rectangle's upper-left corner.
    - `y` determines the vertical position of the rectangle's upper-left corner.
  - **Example:**  
    - `x="50"` and `y="50"` places the rectangle starting at 50 pixels from the left and 50 pixels from the top.

- **width & height**  
  - **What They Do:**  
    - `width` specifies how wide the rectangle is.
    - `height` specifies how tall the rectangle is.
  - **Example:**  
    - `width="100"` and `height="60"` creates a rectangle 100 pixels wide and 60 pixels high.

- **rx & ry (Rounded Corners)**  
  - **What They Do:**  
    - `rx` sets the horizontal radius for rounding the corners.
    - `ry` sets the vertical radius for rounding the corners.
  - **How They Work:**  
    - These attributes soften the edges of the rectangle by rounding the corners.
    - If both `rx` and `ry` are set (for example, to `10`), each corner becomes a quarter of an ellipse with a horizontal radius of 10 and a vertical radius of 10.
  - **Example:**  
    - `rx="10"` and `ry="10"` gives the rectangle smooth, rounded corners.

- **stroke, stroke-width & fill**  
  - **stroke:**  
    - Defines the color of the rectangle's border.
  - **stroke-width:**  
    - Determines the thickness of the border.
  - **fill:**  
    - Specifies the color that fills the rectangle.
  - **Example:**  
    - `stroke="black"`, `stroke-width="3"`, and `fill="lightblue"` create a light blue rectangle with a black border 3 pixels thick.

---

## Line Attributes

- **x1, y1, x2 & y2**  
  - **What They Do:**  
    - `x1` and `y1` mark the starting point of the line.
    - `x2` and `y2` mark the ending point of the line.
  - **Example:**  
    - `x1="30"`, `y1="30"` and `x2="200"`, `y2="100"` draw a line starting at coordinate (30, 30) and ending at coordinate (200, 100).

- **stroke & stroke-width**  
  - **stroke:**  
    - Sets the color of the line.
  - **stroke-width:**  
    - Specifies the thickness of the line.
  - **Example:**  
    - `stroke="red"` with `stroke-width="2"` results in a red line that is 2 pixels thick.

---

## Polygon Attributes

- **points**  
  - **What It Does:**  
    - Defines the vertices (corners) of the polygon.
  - **Format:**  
    - A series of coordinate pairs formatted as `x,y`, with each pair separated by a space.
  - **Understanding the Format:**  
    - For example, `points="80,50 230,50 230,200 155,125 80,200"` defines five vertices:
      - **80,50:** First vertex
      - **230,50:** Second vertex
      - **230,200:** Third vertex
      - **155,125:** Fourth vertex
      - **80,200:** Fifth vertex
  - **How It Works:**  
    - The browser connects the vertices in the order they are listed, and automatically connects the last vertex back to the first to close the shape.
  - **Why It Matters:**  
    - Adjusting these numbers changes the shape of the polygon. Each coordinate pair determines where a corner will be placed on the SVG canvas.

- **fill**  
  - **What It Does:**  
    - Sets the interior color of the polygon.
  - **Example:**  
    - `fill="pink"` fills the polygon with a pink color.

- **Interactivity:**  
  - In the SVG Editor, you can add or remove vertices dynamically. This interactivity lets you see firsthand how modifying the `points` attribute alters the shape.

---

## Text Attributes

- **x & y**  
  - **What They Do:**  
    - Define the starting point where the text is rendered within the SVG canvas.
  - **Example:**  
    - `x="0"` and `y="250"` position the text at the left edge and 250 pixels from the top.

- **font-family & font-size**  
  - **font-family:**  
    - Determines the style of the font (e.g., Verdana, Arial).
  - **font-size:**  
    - Specifies the size of the text.
  - **Example:**  
    - `font-family="Verdana"` and `font-size="20"` render the text in a clear, legible manner.

- **fill**  
  - **What It Does:**  
    - Sets the color of the text.
  - **Example:**  
    - `fill="black"` displays the text in black.

---

## Conclusion

- **Understanding Coordinates:**  
  - Attributes such as `cx`, `cy`, `x`, `y`, and the coordinate pairs in `points` place each element accurately on the canvas.
  
- **Dimensions and Sizing:**  
  - Properties like `r`, `width`, and `height` define the size of shapes.
  
- **Styling and Appearance:**  
  - Attributes such as `fill`, `stroke`, and `stroke-width` consistently control the colors and borders of SVG elements.
  
- **Specialized Attributes:**  
  - `rx` and `ry` for rectangles offer rounded corners.
  - The `points` attribute for polygons is a flexible way to define complex shapes by listing vertex coordinates.

This guide is intended to help beginners understand the role of each attribute in creating and modifying SVG graphics. For further reading on SVG fundamentals, please visit [What Are SVGs](#) for an introduction.
