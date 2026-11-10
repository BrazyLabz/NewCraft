BOOKS (v0.92)
=============
Every .json file in this folder is one book you can find in a bookcase and read in the game.
A bookcase has 2 shelves of 8 books (16 spaces) and shows the books that are in it, each in its own colour.
Bookcases you find in the world have 1 or 2 books left in them. Right-click a bookcase to take them
(or put books back), then hold a book and right-click to read it.

To make a new book: copy example_book.json, rename it (my_book.json), and change what's inside.
The file name is the book's id — keep it lowercase with no spaces.

  "title"   the name on the cover (shows in your hand instead of the tip)
  "author"  shows under the title ("by Daniel Reyes")
  "year"    optional, shows on the title page
  "color"   "random" (any of the cover colours) or a colour like "#7c2d12"
  "weight"  how often it turns up: 1 = normal, 2 = twice as often, 0 = never in bookcases
  "pages"   a list of pages: ["page one", "page two", ...]   \n = a new line
  "text"    OR one long piece of writing: the game cuts it into pages for you (use \n\n between paragraphs)

Check your file is valid JSON (every "quote" closed, commas between things, no comma after the last one).
A broken file is skipped and the game tells you which one in the browser console (F12).

After adding books:
  - dev.html (Play NovaCraftZ.bat) picks them up straight away (reload the page).
  - Run "Rebuild index.bat" so index.html (GitHub) and the Windows game get them too.
