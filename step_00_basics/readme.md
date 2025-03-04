# SVG Basics README

**Navigation:**  
- [What Are SVGs](#what-are-svgs)  
- [Why Use SVGs](#why-use-svgs)  
- [Difference Between Raster Images and SVGs](#difference-between-raster-images-and-svgs)  
- [Basics of SVGs](#basics-of-svgs)  
- [Code Explanation](#code-explanation)  

---

## What Are SVGs?

- **Scalable Vector Graphics (SVG):**
  - XML-based markup language for describing 2D vector graphics.
  - Uses shapes such as lines, curves, circles, and polygons.
  - Resolution-independent, making them perfect for scalable and high-quality graphics.

---

## Why Use SVGs?

- **Scalability:**  
  - Can be resized to any dimensions without losing quality.
- **Small File Sizes:**  
  - Typically more efficient for icons and simple illustrations compared to raster images.
- **Interactivity & Animation:**  
  - Easily styled with CSS and manipulated with JavaScript.
- **Accessibility:**  
  - Text remains selectable and searchable.
- **Editability:**  
  - As an XML format, it is straightforward to edit and optimize.

---

## Difference Between Raster Images and SVGs

- **Raster Images:**
  - Composed of individual pixels.
  - Common formats include JPEG, PNG, and GIF.
  - Quality degrades (pixelation) when scaled beyond its original dimensions.
  - Best for detailed photographs and complex imagery.
  
- **SVGs:**
  - Composed of vectors defined by mathematical formulas.
  - Infinitely scalable without quality loss.
  - Ideal for icons, logos, and simple illustrations.
  - Can be dynamically styled and animated.

---

## Basics of SVGs

- **Inline SVG:**
  - Embedding SVG code directly into your HTML file.
  - **Examples Include:**
    - **Circle:** `<circle cx="100" cy="100" r="50" fill="blue" />`
    - **Rectangle:** `<rect width="100" height="50" fill="green" />`
    - **Polygon:** `<polygon points="100,0 200,0 200,100 100,100" fill="red" />`
    - **Line:** `<line x1="0" y1="0" x2="200" y2="200" stroke="black" stroke-width="3" />`
    - **Other Shapes:** Ellipse, Polyline, Path, and Text.
  
- **SVG Using `<symbol>` and `<use>`:**
  - Define reusable graphic elements using `<symbol>`.
  - Render the symbol with `<use>` to avoid repeating the same code.
  
- **SVG Via `<img>` Tag:**
  - Embed an external SVG file.
  - Keeps the SVG code separate from your HTML, which aids in organization and caching.
  - **Example:** `<img src="external.svg" alt="External SVG Example" width="200" height="200" />`

---

## Code Explanation

- **Inline SVG Examples:**
  - **Circle:**  
    - Creates a blue circle with center coordinates `(100, 100)` and a radius of `50`.
  - **Rectangle:**  
    - Renders a green rectangle with a width of `100` and a height of `50`.
  - **Polygon:**  
    - Draws a red quadrilateral by connecting specified points.
  - **Line:**  
    - Draws a black diagonal line from the top-left to the bottom-right.
  - **Additional Elements:**  
    - **Ellipse:** Creates an oval shape.
    - **Polyline:** Connects multiple points with straight lines.
    - **Path:** Uses commands (like quadratic Bézier curves) for complex curves.
    - **Text:** Displays text within the SVG.

- **SVG Using `<symbol>` and `<use>`:**
  - **Symbol Definition:**  
    - The `<symbol>` element defines a star shape (or any graphic) which is hidden (`style="display: none;"`) from direct display.
  - **Symbol Usage:**  
    - The `<use>` element references this symbol with `href="#starSymbol"` to display it.

- **SVG Via `<img>` Tag:**
  - **Embedding External SVG:**  
    - Uses an `<img>` tag to load the external file `external.svg`.
    - Ensures that the external file is in your project directory.

- **External SVG File (`external.svg`):**
  - **XML Declaration:**  
    - Specifies XML version and encoding.
  - **SVG Container:**  
    - Sets the width, height, and SVG namespace.
  - **Graphic Elements in External SVG:**  
    - **Background Rectangle:** Provides a light grey background.
    - **Circle:** Draws a sky blue circle.
    - **Triangle (Polygon):** Creates a lime green triangle.
    - **Diagonal Line:** Draws a black diagonal line.
    - **Text:** Displays a label at the bottom indicating "External SVG".

---

## Conclusion

- **Understanding SVGs:**  
  - Learn what SVGs are and their key benefits.
- **Raster vs. Vector:**  
  - Recognize the differences and decide which image type suits your project.
- **SVG Implementation Basics:**  
  - Understand how to use inline SVGs, reusable symbols, and external SVG files.
- **Code Walkthrough:**  
  - Gain insights into how each SVG element works through detailed examples.

By mastering these fundamentals, you can effectively utilize SVGs to create scalable, interactive, and visually appealing graphics for your web applications.
