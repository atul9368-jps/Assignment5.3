1. The HTML File (index.html)
HTML
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Typography Showcase Page</title>

    <!-- Step 1: Import 2 complementary fonts from Google Fonts (Montserrat & Merriweather) -->
    <link rel="preconnect" href="https://fonts.googleapis.com">
    <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
    <link href="https://fonts.googleapis.com/css2?family=Merriweather:ital,wght@0,300;0,400;0,700;1,400&family=Montserrat:wght@400;600;800&display=swap" rel="stylesheet">

    <!-- External Stylesheet -->
    <link rel="stylesheet" href="style.css">
</head>
<body>

    <header class="showcase-header">
        <h1>Typography Showcase</h1>
        <p class="subtitle">Exploring Font Pairings, Alignment, Spacing, and Styles</p>
    </header>

    <main class="container">
        
        <!-- Section 1: Heading Styles -->
        <section class="showcase-section">
            <h2>1. Heading Styles</h2>
            <div class="card">
                <h1 class="heading-large">Main Heading (Montserrat Bold 800)</h1>
                <h2 class="heading-medium">Subheading Level 2 (Montserrat SemiBold 600)</h2>
                <h3 class="heading-small">Subheading Level 3 (Montserrat Regular 400)</h3>
            </div>
        </section>

        <!-- Section 2: Paragraph Styles -->
        <section class="showcase-section">
            <h2>2. Paragraph Styles</h2>
            <div class="card">
                <p class="paragraph-default">
                    <strong>Default Paragraph:</strong> Typography is the art and technique of arranging type to make written language legible, readable, and appealing when displayed. Good typography improves readability and user experience.
                </p>
                <p class="paragraph-lead">
                    <strong>Lead Paragraph (Expanded Spacing):</strong> This paragraph uses a larger font size, increased line-height, and generous letter-spacing to create a clean, elegant introductory style.
                </p>
                <p class="paragraph-compact">
                    <strong>Compact Paragraph:</strong> This paragraph demonstrates tighter line-height and letter-spacing, often used for captions or dense blocks of supplementary information.
                </p>
            </div>
        </section>

        <!-- Section 3: Text Emphasis -->
        <section class="showcase-section">
            <h2>3. Text Emphasis & Decorations</h2>
            <div class="card">
                <p class="text-italic">This text demonstrates an italicized font style for subtle emphasis.</p>
                <p class="text-underlined">This text uses an underline text decoration to highlight key concepts.</p>
                <p class="text-uppercase">This text is converted to uppercase with expanded letter-spacing.</p>
                <p class="text-center-aligned">This paragraph is center-aligned to draw visual focus.</p>
                <p class="text-right-aligned">This paragraph is aligned to the right side of the container.</p>
            </div>
        </section>

    </main>

</body>
</html>
2. The CSS File (style.css)
CSS
/* Universal Box Sizing */
* {
    box-sizing: border-box;
    margin: 0;
    padding: 0;
}

/* Step 2: Global Page Styling & Body Font Selection (Merriweather) */
body {
    background-color: #f8f9fa;
    color: #2b2d42;
    font-family: 'Merriweather', Georgia, serif; /* Body Font */
    line-height: 1.7; /* Step 5: Base line-height */
    padding-bottom: 40px;
}

.container {
    max-width: 900px;
    margin: 0 auto;
    padding: 0 20px;
}

/* Header Styling */
.showcase-header {
    background-color: #1d3557;
    color: #ffffff;
    text-align: center; /* Step 4: text-align */
    padding: 50px 20px;
    margin-bottom: 40px;
}

.showcase-header h1 {
    font-family: 'Montserrat', sans-serif; /* Step 2: Heading Font */
    font-size: 3rem; /* Step 3: font-size */
    font-weight: 800; /* Step 3: font-weight */
    letter-spacing: 2px; /* Step 5: letter-spacing */
    margin-bottom: 10px;
}

.subtitle {
    font-style: italic; /* Step 4: font-style */
    font-size: 1.1rem;
    color: #a8dadc;
}

/* Section & Card Layout */
.showcase-section {
    margin-bottom: 40px;
}

/* Step 2: Heading Font Family Applied Globally to h2 */
h2 {
    font-family: 'Montserrat', sans-serif;
    color: #1d3557;
    font-size: 1.8rem;
    margin-bottom: 15px;
    border-bottom: 2px solid #457b9d;
    padding-bottom: 8px;
}

.card {
    background-color: #ffffff;
    padding: 25px;
    border-radius: 8px;
    box-shadow: 0 4px 10px rgba(0, 0, 0, 0.05);
}

/* SECTION 1: HEADING STYLES */
.heading-large {
    font-family: 'Montserrat', sans-serif;
    font-size: 2.2rem; /* Step 3 */
    font-weight: 800;  /* Step 3 */
    color: #e63946;
    margin-bottom: 15px;
}

.heading-medium {
    font-family: 'Montserrat', sans-serif;
    font-size: 1.6rem; /* Step 3 */
    font-weight: 600;  /* Step 3 */
    color: #457b9d;
    margin-bottom: 15px;
}

.heading-small {
    font-family: 'Montserrat', sans-serif;
    font-size: 1.2rem; /* Step 3 */
    font-weight: 400;  /* Step 3 */
    color: #1d3557;
    margin-bottom: 10px;
}

/* SECTION 2: PARAGRAPH STYLES */
.paragraph-default {
    font-size: 1rem;
    line-height: 1.6; /* Step 5 */
    margin-bottom: 20px;
}

.paragraph-lead {
    font-size: 1.25rem; /* Step 3 */
    line-height: 2.0;   /* Step 5 */
    letter-spacing: 0.5px; /* Step 5 */
    color: #1d3557;
    margin-bottom: 20px;
}

.paragraph-compact {
    font-size: 0.9rem; /* Step 3 */
    line-height: 1.3;  /* Step 5 */
    letter-spacing: -0.2px; /* Step 5 */
    color: #6c757d;
}

/* SECTION 3: TEXT EMPHASIS */
.text-italic {
    font-style: italic; /* Step 4 */
    margin-bottom: 15px;
}

.text-underlined {
    text-decoration: underline; /* Step 4 */
    text-decoration-color: #e63946;
    margin-bottom: 15px;
}

.text-uppercase {
    text-transform: uppercase;
    letter-spacing: 3px; /* Step 5 */
    font-weight: 600;
    font-size: 0.95rem;
    color: #457b9d;
    margin-bottom: 15px;
}

.text-center-aligned {
    text-align: center; /* Step 4 */
    margin-bottom: 15px;
}

.text-right-aligned {
    text-align: right; /* Step 4 */
}