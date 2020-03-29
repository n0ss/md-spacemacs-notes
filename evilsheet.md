
# Table of Contents

1.  [Movements](#org51b41cb)
    1.  [Arrow keys](#org6f8d9e2)
    2.  [Evil moves](#orgb6c0172)
2.  [Objects](#org11b9e9e)
3.  [Formatting commands](#orgb089ba1)
4.  [Deletion](#org7c313fd)
    1.  [Single caracter](#orgb65f847)
    2.  [Single word](#orgdd90294)
    3.  [Single line](#org4157732)
5.  [Paste](#org36f26ae)
6.  [Replace](#org5a9ea0c)
    1.  [Character](#orgc6794f7)
    2.  [Word](#org543bd8a)
    3.  [Replace mode](#org3a4d7b4)
7.  [Undos / Redos](#org95fc06b)
8.  [Moving](#orge550c68)
    1.  [At bottom of buffer](#org3dbb5b7)
    2.  [At beginning of buffer](#org5d432b2)
    3.  [At specific line](#org839e992)
9.  [Inserting text](#org7872b4a)
    1.  [Characters](#org116ec2e)
    2.  [Lines](#orgc404c3f)
    3.  [Append at line](#org3228631)
10. [Searching / Replacing](#org21d151d)
    1.  [Searching in text](#org996440d)
    2.  [Replacing](#org2ec6453)
    3.  [Matching parenthesis](#org548c389)
11. [Saving / Inserting files](#org19e19d3)
    1.  [Current file](#org80d71e6)
    2.  [Current buffer to specific file](#org05126e4)
    3.  [Specific lines in buffer](#orgca3c2d6)
    4.  [Inserting file in current position](#org07d0670)
12. [Exiting](#org640d531)
    1.  [Saving changes](#orge51feeb)
    2.  [Without saving](#org63439f2)



<a id="org51b41cb"></a>

# Movements


<a id="org6f8d9e2"></a>

## Arrow keys

You can use the arrow keys in Evil mode, it's not the best way but it works :
<kbd> <left> </kbd>   <kbd> <down> </kbd>   <kbd> <up> </kbd>   <kbd> <right> </kbd> 


<a id="orgb6c0172"></a>

## Evil moves

Spacemacs using Evil helps you improve fast movements with these keys :
<kbd> h </kbd>   <kbd> j </kbd>   <kbd> k </kbd>   <kbd> l </kbd> 


<a id="org11b9e9e"></a>

# Objects

Refer a word using <kbd> w </kbd>

Refer a line using <kbd> $ </kbd>


<a id="orgb089ba1"></a>

# Formatting commands

Use a command on multiple objects in one row using : [number] [command] [object] OR [command] [number] [object]
Example : <kbd> 5 d w </kbd> deletes five words from cursor


<a id="org7c313fd"></a>

# Deletion


<a id="orgb65f847"></a>

## Single caracter

<kbd> x </kbd> 


<a id="orgdd90294"></a>

## Single word

<kbd> d w </kbd>


<a id="org4157732"></a>

## Single line

<kbd> d $ </kbd>
<kbd> d d </kbd>


<a id="org36f26ae"></a>

# Paste

<kbd> p </kbd> puts the deleted/copied/cut text after the cursor


<a id="org5a9ea0c"></a>

# Replace


<a id="orgc6794f7"></a>

## Character

<kbd> r </kbd> replaces the character under the cursor


<a id="org543bd8a"></a>

## Word

<kbd> c </kbd> replaces the word from the cursor 


<a id="org3a4d7b4"></a>

## Replace mode

<kbd> R </kbd> to enter replace mode until <kbd> <escape> </kbd> is pressed


<a id="org95fc06b"></a>

# Undos / Redos

Spacemacs remembers your actions to go back in time or move forward again. 
<kbd> u </kbd> to undo last action (keep pressed for multiple)
<kbd> C-r </kbd> to redo last action (keep pressed for multiple) 


<a id="orge550c68"></a>

# Moving


<a id="org3dbb5b7"></a>

## At bottom of buffer

<kbd> G </kbd>


<a id="org5d432b2"></a>

## At beginning of buffer

<kbd> g g </kbd>  


<a id="org839e992"></a>

## At specific line

<kbd> : </kbd>[number] moves you to line [number]


<a id="org7872b4a"></a>

# Inserting text


<a id="org116ec2e"></a>

## Characters

<kbd> i </kbd> will open edit mode to insert a character before current cursor

<kbd> a </kbd> will open edit mode to insert a character after current cursor


<a id="orgc404c3f"></a>

## Lines

<kbd> o </kbd> will open edit mode to insert a new line after current cursor

<kbd> O </kbd> will open edit mode to insert a new line before current cursor


<a id="org3228631"></a>

## Append at line

<kbd> A </kbd> to append text to the end of the line 


<a id="org21d151d"></a>

# Searching / Replacing


<a id="org996440d"></a>

## Searching in text

<kbd> / </kbd> followed by a phrase searches FORWARD in text 

<kbd> ? </kbd> followed by a phrase searches BACKWARD in text 


<a id="org2ec6453"></a>

## Replacing

<kbd> : s / OLD / NEW </kbd>

<kbd> : s / OLD / NEW / g </kbd>

<kbd> : # , # s / OLD / NEW </kbd>

<kbd> : % s / OLD / NEW / g </kbd>

<kbd> : % s / OLD / NEW / g c </kbd>


<a id="org548c389"></a>

## Matching parenthesis

Typing <kbd> % </kbd>  while the cursor is on a  (,),[,],{, or }  locates its
matching pair.


<a id="org19e19d3"></a>

# Saving / Inserting files


<a id="org80d71e6"></a>

## Current file

<kbd> : w </kbd> to save current buffer to file


<a id="org05126e4"></a>

## Current buffer to specific file

<kbd> : w FILENAME </kbd> to save current buffer to specific FILENAME


<a id="orgca3c2d6"></a>

## Specific lines in buffer

<kbd> : # , # FILENAME </kbd> to save the lines # through # to specific FILENAME


<a id="org07d0670"></a>

## Inserting file in current position

<kbd> : r FILENAME </kbd> retrieves file FILENAME and inserts it into buffer at current position


<a id="org640d531"></a>

# Exiting


<a id="orge51feeb"></a>

## Saving changes

<kbd> : q a ! </kbd>


<a id="org63439f2"></a>

## Without saving

<kbd> : w q a </kbd>

