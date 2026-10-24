# patch-notes_indie-gaming-publication
Patch Notes: Indie Gaming Publication


Documentation:
-My intention for this project was to create a site for news on independent gaming and trading card games (TCG), with my audience being those that partake in online/console gaming, as well as collecting and playing various TCGs. 
-The reset strategy with at least two important decisions is found on the actual specimen page.
-My major token groups include raw color, semantic color, type, type scaling, spacing and component radius. I attempted to keep the naming of tokens as clear as possible, starting each section with it's overarching purpose (like color) and then went more narrow (like page-bg or text). 
-I didn't use any third-party fonts and instead went with what should already be web-safe. I made sure that for each of my three font categories (display, body and sub) that they all had fallback fonts, including the most web-safe declarations such as 'sans-serif' or 'monospace'.
-The alternate theme was created without any duplicating component rules by adding a second class to the alt-themed card, then styling based on the alt theme using that second class. 
-For accessibility, each link can be accessed by pressing tab and each image has alt text, although they are all just placeholders at the moment. For contrast, I used a dark background with brighter accents of red, yellow and purple. I am also aware that most people that are online often and are interested in this sort of material tend to use dark mode, so I made a darker background my default.
-One change I made due to testing was one that was sort of new to me. This is a small thing, but I wanted my footer to not only always be under the main material, but to be glued to the bottom of the page without using absolute positions. What I settled on was make the body flex and making the flex direction as a column. I made the body min-height 100% of the viewport height and then set main's flex as 1. This ensured that the footer was always at the bottom of the screen regardless of viewport size, as I used percentages rather than absolute values. 
-I used ChatGPT to assist in cleaning up my token names and verifying that my button code was correct. For my token names, it suggested that I add a a prefix to each that describes the overarching purpose, i.e. color. For my button code suggested that I add 'cursor: pointer' to give a visual cue that the mouse is over the button. I verified the relevant claims using MDN and tested that the cursor did change when over the button. I retained both suggestions because the tokens became easier to use with this naming convention and the cursor is a proper way to add accessibility for keyboard and mouse users. I can explain the final implementation.


Required Tests:
-I tested the viewport at 320, 768 and 1280 px and as expected, they all responded appropriately. The content wrapped and took up the proper amount of space on the screen.
-I tested the zoom at 200% and as expected, it responded appropriately. The content wrapped and took up the proper amount of space on the screen.
-For keyboard control, the expected result was that by using tab only, all links and buttons on the page would be accessible. The actual result proved that to be the case.
-For my font fallback, there were minor changes, primarily a small reduction in size, when the fallback font was used. The site still remained responsive and maintained the overall preferred look.
-The HTML has been verified using Nu HTML Checker. The CSS has been verified using The W3C CSS Validation Service.

Publication Links:
Repository Link - 
Published Specimen Link - 