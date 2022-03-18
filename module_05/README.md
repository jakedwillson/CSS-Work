# Web Design Rules and Framework

## Resources

- [Google Fonts Website](https://fonts.google.com/)
- [Type-Scale.com](https://type-scale.com/)

## Important CSS Properties for Text

1. font-size
1. line-height
1. letter-spacing

## Website Personalities

### Serious/Elegant

- For luxury and elegance, based on thin serif typefaces, golden or pastel colors, and big high-quality images

### Minimalist/Simple

- Focuses on the essential text content, using small or medium-sized sans-serif black text, lines, and few images and icons

### Plain/Neutral

- Design that gets out of the way by using neutral and small typefaces, and a very structured layout. Common in big corporations

### Bold/Confident

- Makes an impact, by featuring big and bold typography, paired with confident use of big and bright colored blocks

### Calm/Peaceful

- For products and services that care, transmitted by calming pastel colors, soft serif headings, and matching images/illustrations

### Startup/Upbeat

- Widely used in startups, featuring medium-sized sans-serif typefaces, light-grey text and backgrounds, and rounded elements

### Playful/Fun

- Colorful and round designs, fueled by creative elements like hand-drawn icons or illustrations, animations and fun language

## Typography

### Definition

- Typography is the art and technique of arranging type to make written language legible, readable and appealing when displayed

## Serif/Sans-Serif

### Serif

- Has decorative lines on letters
- Creates a traditional look/feel
- Conveys trustworthiness
- Good for long text

### Sans-Serif

- Does not have decorative lines
- Modern look and feel
- Clean and simple
- Easier to choose for beginner designer

## Rules on Typefaces

1. Only use good and popular typefaces and play it safe
1. It is okay to use one typeface per page. If you want more, limit to 2 total
1. Choose the right typeface according to your website personality
1. When choosing font-sizes, limit choices. Use a "type scale" tool or other pre-defined range
1. Use a font size between 16px and 32 px for "normal" text
1. For long text (like a blog post), try a size of 20px or even bigger
1. For headlines, you can go really big (50px+) and bold (600+), depending on personality
1. For any text, don't use a font weight under 400 (regular)
1. Use less than 75 characters per line
1. For normal-sized text, use a line height between 1.5 and 2. For big text, go below 1.5 (the smaller/longer the text, the larger the line height needs to be). Example: 1.2 on headline, 1.31 for description below it, 1.52 for body section
1. Decrease letter spacing in headlines, if it looks unnatural (this will come from experience). Example: -3.5 letter spacing.
1. Experiment with all caps for short titles. Make them small and bold and increase letter-spacing.
1. Usually, don't justify text.
1. Do not center long text blocks; centering small blocks is fine though.

### Good/Popular Sans-Serif Typefaces

1. Inter
1. Open Sans
1. Roboto
1. Montserrat
1. Work Sans
1. Lato

### Good/Popular Serif Typefaces

1. Merriweather
1. Aleo
1. Playfair Display
1. Cormorant
1. Cardo
1. Lora

## Choose the Right Color

1. Make the main color match your website's personality: colors convey meaning!
1. Use a good color tone! Don't choose a random tone or CSS named colors.
1. Use your main color to draw attention to the most important elements on the page.
1. Use colors to add interesting accents or make entire components or sections stand out.
1. You can try to use your color strategically in images and illustrations.
1. On dark colored backgrounds, try to use a tint of the background (lighter version) for text.
1. `Text should usually not be completely black`. Lighten it up if it looks heavy and uninviting.
1. Don't make text too light! Use a tool to check contrast between text and background colors. Tools like coolors will give you a `contrast ratio` which needs to be at least 4.5:1 for normal text and 3:1 for large text (18px+)

### Specific Colors

1. Red draws a lot of attention, and symbolizes power, passion and excitement
1. Orange is less aggressive, and conveys happiness, cheerfulness and creativity
1. Yellow means joy, brightness and intelligence
1. Green represents harmony, nature, growth and health
1. `Blue` is associated with peace, trustworthiness and professionalism (most common)
1. Purple conveys wealth, wisdom and magic
1. Pink represents romance, care and affection
1. Brown represents nature, durability and comfort
1. Black symbolizes power, elegance and minimalism, but also grief and sorrow

### Color Tone

#### Generating Colors

1. [Open Color](https://yeun.github.io/open-color/)
1. [Flat UI Colors 2](https://flatuicolors.com/)
1. [tailwindcss](https://tailwindcss.com/)

#### Generating Accent Colors

1. [palleton](https://www.palleton.com/)
1. [coolors](https://coolors.co/)

#### Generating Tints and Shades

1. [Tint & Shade Generator](https://maketintsandshades.com/)

### Establish a Color System

1. You need at least two types of colors in your color palette: a main color and a grey color (the grey color does not necessarily need to be a "true grey", it can be a very dark version of another color, like blue)
1. With more experience, you can add more colors: accent colors (use a tool). There should be a relationship between the main and accent color, which is why you should use a tool
1. For diversity, create lighter and darker "versions" - tints (lighter) and shades (darker)

## Images

### Use Good Images

1. Different types of images: product photos, storytelling photos, illustrations, patterns.
1. Use images to support your website's message and story. Only use relevant ones!
1. Prefer original images. If not possible, use original-looking stock images (not generic ones!)
1. Try to show real people to trigger users' emotions
1. If necessary, crop images to fit your message

### Resources for Authentic Images

1. [Unsplash](https://unsplash.com/)
1. [Pexels](https://www.pexels.com/)
1. [DrawKit](https://drawkit.com/)
1. [unDraw](https://undraw.co/)
1. [Squoosh](https://squoosh.app/) allows you to reduce the file size of an image.

### Handling Text on Images

1. Method 1: Darken or brighten the image (completely or partially, using a gradient)
1. Method 2: Position text into neutral image area
1. Method 3: Put text in a box

### Some Technical Details

1. To account for high-res screens, make image dimensions 2x as big as their displayed size (if original is 600 x 600, displayed is 300 x 300)
1. Compress images for a lower file size and better performance
1. When using multiple images side-by-side, make sure that they have the exact same dimensions

## Icons

### Rules

1. Use a good icon pack, there are tons of free and paid icon packs.
1. Use only one icon pack. Don't mix icons from different icon packs.
1. Use SVG icons or icon fonts (since you can scale indefinitely). Don't use bitmap image formats (.jpg and .png)!
1. Adjust to website personality! Roundness, weight and filled/outlined depend on typography.
1. Use icons to provide visual assistance to text.
1. Use icons for product feature blocks.
1. Use icons associated with actions, and label them (unless no space or icon is 100% clear)
1. Use icons as bullet points.
1. To keep icons neutral, use same color as text. To draw more attention, use different color.
1. Don't confuse your users: icons need to make sense and fit the text or action!
1. Don't make icons larger than what they were designed for. If needed, enclose them in a shape.

### Some Icon Packs

1. [Phosphor Icons](https://phosphoricons.com/)
1. [Ionicons](https://ionic.io/ionicons)
1. [ICONS8](https://icons8.com/)
1. [heroicons](https://heroicons.com/)

### Important CSS Properties

1. stroke
1. width
1. height
1. margin-bottom

## Shadows

### General Concepts

1. Originally, it was Skeuomorphic design (glassy/real-world ocean for example), but then it transitioned into flat design (minimal)
1. After an era of 100% flat design, we are now back to using shadows in UI design (flat design 2.0 - still minimal, but brings back shadows and depth for better usability)
1. Shadow creates depth (3D): the more shadow, the further away from the interface the element is

### Use Shadows Well

1. You don't have to use shadows! Only use them if it makes sense for the website personality (less shadow = serious/elegant; more shadow = playful/fun)
1. Use shadows in small doses: don't add shadows to every element!
1. Go light on shadows, don't make them too dark

### Use Shadows In the Right Situation

1. Use small shadows for smaller elements that should stand out (to draw attention)
1. Use medium-sized shadows for larger areas that should stand out a bit more
1. Use large shadows for elements that should really `float above` the interface (e.g., navigations and pop-up windows)
1. Experiment with changing shadows on mouse interaction (click and hover). Medium-sized shadow "pulls" button closer to the user; smaller shadow "pushes" button back into the interface.
1. Bonus: experiment with glows (colored shadows)

### Important CSS Properties for Shadows

1. `box-shadow (horizontal offset) (vertical offset) (blur) (scale) (color)`, example: `box-shadow: 20px 20px 20px 10px #000`

## Border Radius

### Use Border Radius Well

1. Use border-radius to increase the playfulness and fun of the design, to make it less serious
1. Typefaces have a certain roundness: make sure that border-radius matches that roundness
1. Use border-radius on buttons, images, around icons, standout sections and other elements

### Notes

1. You can make an element round by giving it a border-radius of 50%
