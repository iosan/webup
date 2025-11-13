# Theme Variations

With CSS variables, you can easily create different color themes by overriding the variables in the `:root` selector.

## Current Theme: Industrial Dark Sepia
The default theme uses dark sepia (#3d2f21) for a professional industrial look.

## Alternative Themes

### Theme 1: Blue Industrial
```css
:root {
    --color-primary: #1a3a52;           /* Dark blue */
    --color-primary-light: #85b3d1;     /* Light blue */
    --color-background: #f0f4f8;        /* Light blue-gray */
}
```

### Theme 2: Modern Gray
```css
:root {
    --color-primary: #2c3e50;           /* Dark gray-blue */
    --color-primary-light: #bdc3c7;     /* Light gray */
    --color-background: #ecf0f1;        /* Very light gray */
}
```

### Theme 3: Deep Green
```css
:root {
    --color-primary: #1e3a1a;           /* Forest green */
    --color-primary-light: #a8d5ba;     /* Mint green */
    --color-background: #f1f8f4;        /* Very light green */
}
```

### Theme 4: Warm Orange
```css
:root {
    --color-primary: #d35400;           /* Dark orange */
    --color-primary-light: #f39c12;     /* Light orange */
    --color-background: #fef5e7;        /* Cream */
}
```

### Theme 5: Professional Navy
```css
:root {
    --color-primary: #001f3f;           /* Navy blue */
    --color-primary-light: #7fdbff;     /* Sky blue */
    --color-background: #f4f7f9;        /* Light blue-white */
}
```

## How to Apply a Theme

1. **Option 1: Replace in style.css**
   - Open `css/style.css`
   - Find the `:root` section at the top
   - Replace the color variables with your chosen theme

2. **Option 2: Create a separate theme file**
   - Create a new file like `css/theme-blue.css`
   - Add only the variable overrides
   - Link it after style.css in your HTML:
   ```html
   <link rel="stylesheet" href="css/style.css">
   <link rel="stylesheet" href="css/theme-blue.css">
   ```

3. **Option 3: Use media queries for dark mode**
   ```css
   @media (prefers-color-scheme: dark) {
       :root {
           --color-primary: #000000;
           --color-background: #1a1a1a;
           --color-text-dark: #ffffff;
           --color-text-medium: #cccccc;
       }
   }
   ```

## Customizing Other Aspects

### Spacing
Change spacing variables to adjust the overall layout:
```css
:root {
    --spacing-sm: 16px;      /* Smaller padding */
    --spacing-md: 32px;      /* Tighter spacing */
    --spacing-lg: 80px;      /* Less left margin */
}
```

### Logo Size
```css
:root {
    --logo-size: 100px;      /* Larger logo */
}
```

### Image Gallery
```css
:root {
    --gallery-gap: 60px;           /* More space between images */
    --image-size: 300px;           /* Larger images */
    --image-rotation-large: 8deg;  /* More dramatic rotation */
}
```

### Typography
```css
:root {
    --font-family: 'Helvetica Neue', Helvetica, Arial, sans-serif;
    --line-height-text: 1.8;       /* More spacious text */
}
```

## Tips

- **Test your theme** in multiple browsers
- **Maintain contrast ratios** for accessibility (WCAG AA minimum 4.5:1)
- **Use hex or rgba** for colors that support transparency
- **Group related variables** for easier management
- **Document custom themes** for future reference
