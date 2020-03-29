
# Table of Contents

1.  [Movements](#org4f03f58)
    1.  [Arrow keys](#org5cf93f5)
    2.  [Evil moves](#org379e2f0)
2.  [Objects](#orga190c39)
3.  [Formatting commands](#orgd3bc5c5)
4.  [Deletion](#org5dcd6c9)
    1.  [Single caracter](#org891451c)
    2.  [Single word](#orgb264134)
    3.  [Single line](#orga9f3346)
5.  [Paste](#org1925e1d)
6.  [Replace](#org2604dd8)
    1.  [Character](#org231a8aa)
    2.  [Word](#org3410d3a)
    3.  [Replace mode](#orgc78998f)
7.  [Undos / Redos](#org2c36e85)
8.  [Moving](#org131f390)
    1.  [At bottom of buffer](#orgd4e9b01)
    2.  [At beginning of buffer](#org4f998dd)
    3.  [At specific line](#org63ff4de)
9.  [Inserting text](#orgf3c230d)
    1.  [Characters](#orge8882a7)
    2.  [Lines](#org5a19b8b)
    3.  [Append at line](#org022218a)
10. [Searching / Replacing](#org7bdada8)
    1.  [Searching in text](#org26af00f)
    2.  [Replacing](#org4658801)
    3.  [Matching parenthesis](#orgb6519c9)
11. [Saving / Inserting files](#org047f6f8)
    1.  [Current file](#orge4d2ab6)
    2.  [Current buffer to specific file](#org380acc0)
    3.  [Specific lines in buffer](#orgbbaf826)
    4.  [Inserting file in current position](#org908f267)
12. [Exiting](#org7b6d264)
    1.  [Saving changes](#org2d6e812)
    2.  [Without saving](#org7edca87)



<a id="org4f03f58"></a>

# Movements


<a id="org5cf93f5"></a>

## Arrow keys

You can use the arrow keys in Evil mode, it's not the best way but it works :
<kbd> <left> </kbd>   <kbd> <down> </kbd>   <kbd> <up> </kbd>   <kbd> <right> </kbd> 


<a id="org379e2f0"></a>

## Evil moves

Spacemacs using Evil helps you improve fast movements with these keys :

<kbd> h </kbd>   <kbd> j </kbd>   <kbd> k </kbd>   <kbd> l </kbd> 


<a id="orga190c39"></a>

# Objects

Refer a word using <kbd> w </kbd>

Refer a line using <kbd> $ </kbd>


<a id="orgd3bc5c5"></a>

# Formatting commands

Use a command on multiple objects in one row using : [number] [command] [object] OR [command] [number] [object]
Example : <kbd> 5 d w </kbd> deletes five words from cursor


<a id="org5dcd6c9"></a>

# Deletion


<a id="org891451c"></a>

## Single caracter

<kbd> x </kbd> 


<a id="orgb264134"></a>

## Single word

<kbd> d w </kbd>


<a id="orga9f3346"></a>

## Single line

<kbd> d $ </kbd>
<kbd> d d </kbd>


<a id="org1925e1d"></a>

# Paste

<kbd> p </kbd> puts the deleted/copied/cut text after the cursor


<a id="org2604dd8"></a>

# Replace


<a id="org231a8aa"></a>

## Character

<kbd> r </kbd> replaces the character under the cursor


<a id="org3410d3a"></a>

## Word

<kbd> c </kbd> replaces the word from the cursor 


<a id="orgc78998f"></a>

## Replace mode

<kbd> R </kbd> to enter replace mode until <kbd> <escape> </kbd> is pressed


<a id="org2c36e85"></a>

# Undos / Redos

Spacemacs remembers your actions to go back in time or move forward again. 
<kbd> u </kbd> to undo last action (keep pressed for multiple)
<kbd> C-r </kbd> to redo last action (keep pressed for multiple) 


<a id="org131f390"></a>

# Moving


<a id="orgd4e9b01"></a>

## At bottom of buffer

<kbd> G </kbd>


<a id="org4f998dd"></a>

## At beginning of buffer

<kbd> g g </kbd>  


<a id="org63ff4de"></a>

## At specific line

<kbd> : </kbd>[number] moves you to line [number]


<a id="orgf3c230d"></a>

# Inserting text


<a id="orge8882a7"></a>

## Characters

<kbd> i </kbd> will open edit mode to insert a character before current cursor

<kbd> a </kbd> will open edit mode to insert a character after current cursor


<a id="org5a19b8b"></a>

## Lines

<kbd> o </kbd> will open edit mode to insert a new line after current cursor

<kbd> O </kbd> will open edit mode to insert a new line before current cursor


<a id="org022218a"></a>

## Append at line

<kbd> A </kbd> to append text to the end of the line 


<a id="org7bdada8"></a>

# Searching / Replacing


<a id="org26af00f"></a>

## Searching in text

<kbd> / </kbd> followed by a phrase searches FORWARD in text 

<kbd> ? </kbd> followed by a phrase searches BACKWARD in text 


<a id="org4658801"></a>

## Replacing

<kbd> : s / OLD / NEW </kbd>

<kbd> : s / OLD / NEW / g </kbd>

<kbd> : # , # s / OLD / NEW </kbd>

<kbd> : % s / OLD / NEW / g </kbd>

<kbd> : % s / OLD / NEW / g c </kbd>


<a id="orgb6519c9"></a>

## Matching parenthesis

Typing <kbd> % </kbd>  while the cursor is on a  (,),[,],{, or }  locates its
matching pair.


<a id="org047f6f8"></a>

# Saving / Inserting files


<a id="orge4d2ab6"></a>

## Current file

<kbd> : w </kbd> to save current buffer to file


<a id="org380acc0"></a>

## Current buffer to specific file

<kbd> : w FILENAME </kbd> to save current buffer to specific FILENAME


<a id="orgbbaf826"></a>

## Specific lines in buffer

<kbd> : # , # FILENAME </kbd> to save the lines # through # to specific FILENAME


<a id="org908f267"></a>

## Inserting file in current position

<kbd> : r FILENAME </kbd> retrieves file FILENAME and inserts it into buffer at current position


<a id="org7b6d264"></a>

# Exiting


<a id="org2d6e812"></a>

## Saving changes

<kbd> : q a ! </kbd>


<a id="org7edca87"></a>

## Without saving

<kbd> : w q a </kbd>

