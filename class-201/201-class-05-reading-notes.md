# Images, Color, Text

- Duckett, J. (2011). Html &amp; Css. John Wiley &amp; Sons, Inc.

- Nanwani, R. (2016, November 13). JPEG vs PNG vs GIF — which image format to use and when? [web log]. Retrieved May 12, 2022, from <https://blog.imagekit.io/jpeg-vs-png-vs-gif-which-image-format-to-use-and-when-c8913ae3e01d>.

## Images

- Consider buying **stock photos** from companies, watch out for copyrights

- Store all you images in folders and lable them appropriately to help you stay organized

- **Adding images** - Use 'img' element (its and empty element). Add a 'src' to tell the browser where to find the image. Add 'alt' to describe the image for screen readers. Add 'title' for additional info, will appear when image is hovered over. Specify height and width in pixels.

        <img src="URL" alt="This is an image of a house" title="This house stands in a valley in Montana" width="300" height="300" />

- **Where to place image** - Before paragraph, inside the start of a paragraph, in the middle of a paragraph. Think about block elements and inline, if image followed by block the paragraph starts on a new line, inline image element inserts the image in the middle of the words

- **Rules for creating images** - save images in the right format, save images at the right size, use the correct resolution. Consider using Adobe Photoshop to ensure all these attributes are correct

- **Image Dimensions** - save the images with the height and width you'd like them to appear on the page, consider the resolution when enlarging

- **Image resolution** - images for the web should be saved at a resolution of 72ppi (pixels per inch), higher resolution = larger file size. **Vector** images do not lose or gain resolution when enlarged or shrunk

- **Animated GIFs** - shows several images of an image in a sequence to make an animation

- **Transparency** - select 'transparent GIF' or 'PNG' to create a partially transparent image

- **Figure and Figure Caption** - the 'figure' element can house an image and caption together, write the caption with the 'figcaption' element

## Color

- **Foreground color** - specify the color of text with RGB values (ex: rgb(13, 134, 34)), hex codes (ex: #ee3e80), color names (ex: red)

- **Background color** - set the background color of each HTML element 'box' with 'background-color: red;'

- **Contrast** - always consider contrast when picking foreground and background colors to make things legible

- **CSS#: Opacity** - value is a number between 0.0 and 1.0, use 'rgba' (ex: rgba(0,0,,0,0.5))

- **CSS3: HSL & HSLA** - alternative way to specify color. Use 'hsl' followed by 'hue' in a degree between 0-360, 'saturation' as a percentage, and 'lightness' as a percentage from 0%(white) and 100%(black) (ex: hsl(0, 0%, 78%)). Add transparency with 'hsla' and a fourth element 'alpha' as a number between 0 and 1.0

## Text

- **Typeface terminology** - 'serif' fonts add little points on the ends of the letter strokes, 'sans-serif' has straight letter ends, 'monospace' every letter is the same width

- Consider the 'weight' (skinnines to thickness), 'style' (normal, italic, oblique), 'stretch' (squished together, regular, or extended)

- Remember that typefaces are subject to copyright and licenses! ALso the computer needs to have certain typefaces installed to show it! Also remember that PCs render type less smoothly, think about that if designing on a Mac

- **Specifying typefaces** - use 'font-family' to choose the typeface you want to use

- **Size of type** - use 'font-size' to specify size, you can use pixels or percentages. **EMs** are equivalent to the width of the letter 'm'

- **@font-face** - will download the fontface onto a computer that doesnt already have it installed so that it shows up on that screen. You will need the 'font-family' which is the name of the font, the 'src' which is the path to the font, and the 'format' which says the format the font is supplied in

- **Bold** - use 'font-weight' to great bold text, use one of two values - 'normal' for normal weight, and 'bold' for bold

- **Italic** - use 'font-style' and use one of three values, 'normal', 'italic', or 'oblique'

- **Uppercase & lowercase** - use 'text-transform' to change the case of text, use 'uppercase', 'lowercase', or 'capitalize' (for the first letter of each word)

- **Underline & strike** - use 'text-decoration' and the value 'none' (to remove decoration), 'underline', 'overline', 'line-through', 'blink' (makes the text flash on and off)

- **Leading** - use 'line-height' to change the size of the space between text lines

- **letter & word spacing** - use 'letter-spacing' to space out each individual letter, and use 'word-spacing' to change the space between words

- **Alignment** - use 'text-align' and one of the four values, 'left', 'right', 'center', or 'justify' (each line but the last should take up the width of the box)

- **Vertical alignment** - use 'vertical-align' mostly used with inline elements, use values 'baseline', 'sub', 'super', 'top', 'text-top', 'middle', 'bottom', 'text-bottom'

- **Indenting text** - use 'text-indent' to indent the first line of text, can be changed in size with pixels or ems

- **CSS3: Drop shadow** - use 'text-shadow' to make a drop shadow, takes four values - length to the left, distance to top or bottom, amount of blur, color

- **First letter or line** - use ':first-letter' to change how the first letter of a paragraph looks, and ':first-line' for the first sentence. these are pseudo-elements and are stated after the selector

- **Styling links** - use ':link' to change how your links look, pseudo-element and is placed after the selector. ':visited' for links that have been clicked on

- **Responding to users** - ':hover' changes something as the user hovers over it, ':active' changes how something behaves as it is being activated by a user, ':focus' when an element has focus

- **Attribute selectors** - you can make rules for elements that have an attribute with a specific value

## JPEG vs PNG vs GIF

- use JPEG for photos full of colors with smooth intensity like landscapes, use PNG if an image needs transparency or if it contains sharp edges and contrast. Use GIF for animations

- **Compression** - two types - *lossless* means images can be recontructed after compression because no data is lost. *lossy* is irreversible and images cannot be reconstructed after compression. JPEG is a lossy, PNG is lossless, GIF is lossless

- **Transparency** - when something is completely invisible. JPEG images dont support transparency. PNG supports transparency (alpha channels allow partial transparency and you could also declare a single color as transparent), GIF supports transparency (declaring a single color as transparent)

- **Colors** - Number of colors. JPEG can support around 16 million colors. PNG, two modes - PNG8 supports up to 256 colors, and PNG24 up to 16 million. GIF is limited to 256 colors

- **Animation** - change or movement in an image. Only GIF supports animation

[Return home](https://khofstetter94.github.io/reading-notes/)
