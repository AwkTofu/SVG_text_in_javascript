# Key things to know.
This uses d3.js library: https://d3js.org/

The SVG Path was created using an mono space font.

## Creating SVG Paths
An easy way is to use Adobe Illustrator and type the letter in the font you want. Make sure the letter is center correctly. Then exporting the file as SVG. Lastly, open the file and copy the SVG path and paste it in a list of hash of all possible letters and characters on the keyboard.

## Functions Parameters and Return
append_text(g, text, id, x, y, fill_color, scale, horizontal_letter_spacing = 6, stroke_width = 2)
 - g: is the group or the element of the html you are appending the SVG text path to. It should be selected using d3 select.
 - text: the string of text that you want to show
 - id: setting the id of all the path elements in html, so you can find it easiler.
 - x: X location of where the first letter will appear
 - y: Y Location of where the first letter will appear
 - fill_color: color of the text
 - scale: size of the letter/characters
 - horizontal_letter_spacing: the width of each character, used to determine next X location where the next letter will appear. Default is 6.
 - stroke_width: the number that tells how wide the line is in units, default is 2.
 - RETURN TYPE: null

 function append_text_w_wrap(g, text, id, x1, x2, y, fill_color, scale, horizontal_spacing = 6, vertical_spacing = 12, stroke_width = 2)
  - g: is the group or the element of the html you are appending the SVG text path to. It should be selected using d3 select.
 - text: the string of text that you want to show
 - id: setting the id of all the path elements in html, so you can find it easiler.
 - x1: X location of where the first letter will appear
 - x2: X location of where the letters should stop, and start appearing in the next line.
 - y: Y Location of where the first letter will appear
 - fill_color: color of the text
 - scale: size of the letter/characters
 - horizontal_spacing: the width of each character, used to determine next X location where the next letter will appear. Default is 6.
 - vertical_spacing: the height of each character, used to determine next Y location where the next letter will appear. Default is 12.
 - stroke_width: the number that tells how wide the line is in units, default is 2.
 - RETURN TYPE: next Y location of where you are allowed to put more strings.