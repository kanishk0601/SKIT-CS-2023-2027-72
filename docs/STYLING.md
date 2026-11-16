
# Frontend Styling Documentation

## 1. Overview

The project uses CSS to style its web interface and provide a consistent visual appearance across the home page, image upload page, and real-time detection page.

The main stylesheet is:

`static/styles.css`

The stylesheet contains general styling, button effects, upload form styling, error messages, navigation links, video feed styling, and animations.

## 2. General Styling

The global body styling includes:

- Font family: Arial, sans-serif
- Background color: #f4f4f4
- Text color: #333
- Margin: 0
- Padding: 0

Headings (`h1`) use:
- Green color (#4CAF50)
- Center alignment
- Top margin of 20px

Links use green text (#4CAF50), bold font weight, and no underline. On hover, the link color changes to #388E3C.

## 3. Layout and Containers

### Container

The `.container` class provides the main page layout.

- Width: 80%
- Horizontal margins: auto
- Overflow: hidden

### Content Box

The `.box` class provides a white content area.

- White background
- Padding: 20px
- Border radius: 8px
- Subtle box shadow
- Vertical margin: 20px 0

## 4. Button Styling

The `.button-container` class uses Flexbox to arrange buttons horizontally.

- Display: flex
- Justified content: center
- Gap: 20px

The `.button` class defines the appearance of navigation buttons.

- Green background (#4CAF50)
- White text
- Font size: 16px
- Bold text
- Padding: 15px 30px
- Border radius: 8px
- Smooth background-color and transform transitions

### Button Interaction

| State | Styling |
|---|---|
| Normal | Green background |
| Hover | #45a049 and scale(1.05) |
| Active | #388e3c and scale(0.95) |

## 5. Image Upload Form Styling

The upload form uses Flexbox with a vertical layout.

- Display: flex
- Flex direction: column
- Alignment: center

The file input has a bottom margin of 10px.

The submit button includes:
- Green background (#4CAF50)
- White text
- Padding: 10px 20px
- Border radius: 5px
- Pointer cursor
- Font size: 16px

On hover, its background changes to #45a049.

## 6. Error and Navigation Styling

### Error Message

The `.error` class displays error messages using:

- Red color (#ff0000)
- Bold font weight

### Back Link

The `.back-link` class provides a navigation link with:

- Block display
- Center alignment
- Top margin: 20px

## 7. Real-Time Camera Feed Styling

The `.video-container` class centers the video feed using Flexbox.

- Width: 80%
- Horizontal margins: auto
- Display: flex
- Justified content: center

The image element uses:

- Green border (2px solid #4CAF50)
- Border radius: 8px
- Width: 100%
- Maximum width: 800px
- Automatic height

## 8. Animation

The stylesheet defines a `fadeIn` animation using CSS keyframes.

- Starting opacity: 0
- Ending opacity: 1

The animation is applied to `h1` and `.box` elements.

Animation duration: 1 second.

Animation timing function: ease-out.

## 9. Styling Structure

```text
static/
├── .gitkeep
└── styles.css
```

The stylesheet is linked from the HTML templates using Flask's static file URL mechanism.

## 10. Summary

The CSS stylesheet provides a simple and consistent interface for the face shape detection application.

It improves the presentation of navigation buttons, upload forms, error messages, content containers, and the real-time video feed through colors, spacing, borders, transitions, and animations.
