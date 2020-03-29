- [Movements](#sec-1)
  - [Arrow keys](#sec-1-1)
  - [Evil moves](#sec-1-2)
- [Objects](#sec-2)
- [Formatting commands](#sec-3)
- [Deletion](#sec-4)
  - [Single caracter](#sec-4-1)
  - [Single word](#sec-4-2)
  - [Single line](#sec-4-3)
- [Paste](#sec-5)
- [Replace](#sec-6)
  - [Character](#sec-6-1)
  - [Word](#sec-6-2)
  - [Replace mode](#sec-6-3)
- [Undos / Redos](#sec-7)
- [Moving](#sec-8)
  - [At bottom of buffer](#sec-8-1)
  - [At beginning of buffer](#sec-8-2)
  - [At specific line](#sec-8-3)
- [Inserting text](#sec-9)
  - [Characters](#sec-9-1)
  - [Lines](#sec-9-2)
  - [Append at line](#sec-9-3)
- [Searching / Replacing](#sec-10)
  - [Searching in text](#sec-10-1)
  - [Replacing](#sec-10-2)
  - [Matching parenthesis](#sec-10-3)
- [Saving / Inserting files](#sec-11)
  - [Current file](#sec-11-1)
  - [Current buffer to specific file](#sec-11-2)
  - [Specific lines in buffer](#sec-11-3)
  - [Inserting file in current position](#sec-11-4)
- [Exiting](#sec-12)
  - [Saving changes](#sec-12-1)
  - [Without saving](#sec-12-2)


# Movements<a id="sec-1"></a>

## Arrow keys<a id="sec-1-1"></a>

You can use the arrow keys in Evil mode, it's not the best way but it works :

<kbd> <left> </kbd> <kbd> <down> </kbd> <kbd> <up> </kbd> <kbd> <right> </kbd>

## Evil moves<a id="sec-1-2"></a>

Spacemacs using Evil helps you improve fast movements with these keys :

<kbd> h </kbd> <kbd> j </kbd> <kbd> k </kbd> <kbd> l </kbd>

# Objects<a id="sec-2"></a>

Refer a word using <kbd> w </kbd>

Refer a line using <kbd> $ </kbd>

# Formatting commands<a id="sec-3"></a>

Use a command on multiple objects in one row using : [number] [command] [object] OR [command] [number] [object]

Example : <kbd> 5 d w </kbd> deletes five words from cursor

# Deletion<a id="sec-4"></a>

## Single caracter<a id="sec-4-1"></a>

<kbd> x </kbd>

## Single word<a id="sec-4-2"></a>

<kbd> d w </kbd>

## Single line<a id="sec-4-3"></a>

<kbd> d $ </kbd> <kbd> d d </kbd>

# Paste<a id="sec-5"></a>

<kbd> p </kbd> puts the deleted/copied/cut text after the cursor

# Replace<a id="sec-6"></a>

## Character<a id="sec-6-1"></a>

<kbd> r </kbd> replaces the character under the cursor

## Word<a id="sec-6-2"></a>

<kbd> c </kbd> replaces the word from the cursor

## Replace mode<a id="sec-6-3"></a>

<kbd> R </kbd> to enter replace mode until <kbd> <escape> </kbd> is pressed

# Undos / Redos<a id="sec-7"></a>

Spacemacs remembers your actions to go back in time or move forward again.

<kbd> u </kbd> to undo last action (keep pressed for multiple) <kbd> C-r </kbd> to redo last action (keep pressed for multiple)

# Moving<a id="sec-8"></a>

## At bottom of buffer<a id="sec-8-1"></a>

<kbd> G </kbd>

## At beginning of buffer<a id="sec-8-2"></a>

<kbd> g g </kbd>

## At specific line<a id="sec-8-3"></a>

<kbd> : </kbd>[number] moves you to line [number]

# Inserting text<a id="sec-9"></a>

## Characters<a id="sec-9-1"></a>

<kbd> i </kbd> will open edit mode to insert a character before current cursor

<kbd> a </kbd> will open edit mode to insert a character after current cursor

## Lines<a id="sec-9-2"></a>

<kbd> o </kbd> will open edit mode to insert a new line after current cursor

<kbd> O </kbd> will open edit mode to insert a new line before current cursor

## Append at line<a id="sec-9-3"></a>

<kbd> A </kbd> to append text to the end of the line

# Searching / Replacing<a id="sec-10"></a>

## Searching in text<a id="sec-10-1"></a>

<kbd> / </kbd> followed by a phrase searches FORWARD in text

<kbd> ? </kbd> followed by a phrase searches BACKWARD in text

## Replacing<a id="sec-10-2"></a>

<kbd> : s / OLD / NEW </kbd>

<kbd> : s / OLD / NEW / g </kbd>

<kbd> : # , # s / OLD / NEW </kbd>

<kbd> : % s / OLD / NEW / g </kbd>

<kbd> : % s / OLD / NEW / g c </kbd>

## Matching parenthesis<a id="sec-10-3"></a>

Typing <kbd> % </kbd> while the cursor is on a (,),[,],{, or } locates its matching pair.

# Saving / Inserting files<a id="sec-11"></a>

## Current file<a id="sec-11-1"></a>

<kbd> : w </kbd> to save current buffer to file

## Current buffer to specific file<a id="sec-11-2"></a>

<kbd> : w FILENAME </kbd> to save current buffer to specific FILENAME

## Specific lines in buffer<a id="sec-11-3"></a>

<kbd> : # , # FILENAME </kbd> to save the lines # through # to specific FILENAME

## Inserting file in current position<a id="sec-11-4"></a>

<kbd> : r FILENAME </kbd> retrieves file FILENAME and inserts it into buffer at current position

# Exiting<a id="sec-12"></a>

## Saving changes<a id="sec-12-1"></a>

<kbd> : q a ! </kbd>

## Without saving<a id="sec-12-2"></a>

<kbd> : w q a </kbd>
