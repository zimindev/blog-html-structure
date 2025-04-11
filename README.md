Here's a comprehensive guide to HTML document structure:

### **Basic HTML Document Structure**
```html
<!DOCTYPE html>
<html lang="en">
<head>
    <!-- Meta information and links -->
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Document Title</title>
    <link rel="stylesheet" href="styles.css">
</head>
<body>
    <!-- Visible content -->
    <header>
        <h1>Main Heading</h1>
        <nav>
            <ul>
                <li><a href="#home">Home</a></li>
                <li><a href="#about">About</a></li>
            </ul>
        </nav>
    </header>
    
    <main>
        <section>
            <h2>Content Section</h2>
            <article>
                <h3>Article Title</h3>
                <p>Article content...</p>
            </article>
        </section>
        
        <aside>
            <h3>Related Info</h3>
            <p>Additional content...</p>
        </aside>
    </main>
    
    <footer>
        <p>Copyright &copy; <span id="year"></span></p>
    </footer>

    <script src="script.js"></script>
</body>
</html>
```

### **Key Structural Elements**

1. **Document Declaration**
   ```html
   <!DOCTYPE html>
   ```
   - Must be first line
   - Declares HTML5 document type

2. **Root Element**
   ```html
   <html lang="en">
   ```
   - Wraps all content
   - `lang` attribute specifies language

3. **Head Section**
   ```html
   <head>
       <meta charset="UTF-8"> <!-- Character encoding -->
       <meta name="viewport" content="width=device-width, initial-scale=1.0">
       <title>Page Title</title>
       <link rel="stylesheet" href="styles.css">
   </head>
   ```
   - Contains metadata, title, and links
   - Not visible to users

4. **Body Section**
   ```html
   <body>
       <!-- All visible content -->
   </body>
   ```
   - Contains all displayable content

### **Semantic HTML5 Elements**

| Element      | Purpose |
|-------------|---------|
| `<header>`  | Introductory content |
| `<nav>`     | Navigation links |
| `<main>`    | Primary content (unique per page) |
| `<section>` | Thematic grouping |
| `<article>` | Self-contained composition |
| `<aside>`   | Tangentially related content |
| `<footer>`  | Footer content |

### **Important Notes**

1. **Nesting Rules**:
   - Block elements can contain other block/inline elements
   - Inline elements shouldn't contain block elements
   - Lists (`<ul>`, `<ol>`) must only contain `<li>` elements

2. **Accessibility**:
   ```html
   <img src="image.jpg" alt="Description">
   <button aria-label="Close">X</button>
   ```
   - Always include `alt` text for images
   - Use ARIA attributes when needed

3. **Modern Practices**:
   - Use semantic elements over generic `<div>` when possible
   - Keep nesting reasonable (3-4 levels max)
   - Validate your HTML using [W3C Validator](https://validator.w3.org/)

This structure provides a solid foundation for any HTML document while ensuring accessibility, SEO-friendliness, and maintainability.
