
# Table of Contents

1.  [Movements](#org4169f60)
    1.  [Arrow keys](#org782690d)
        1.  [You can use the arrow keys in Evil mode, it's not the best way but it works :](#orgabf9096)
    2.  [Evil moves](#org5edea99)
        1.  [Spacemacs using Evil helps you improve fast movements with these keys :](#org24c16d9)
2.  [Objects](#org1ba92b5)
3.  [Formatting commands](#org3338cc0)
4.  [Deletion](#orgc7e66bb)
    1.  [Single caracter](#org114549a)
    2.  [Single word](#orgbeae53d)
    3.  [Single line](#org790202b)
5.  [Paste](#org2ba20d7)
6.  [Replace](#orga297dc2)
    1.  [Character](#org312dbb9)
    2.  [Word](#orgfa6b313)
    3.  [Replace mode](#org0bacabf)
7.  [Undos / Redos](#orga2f574a)
8.  [Moving](#orgc8432c3)
    1.  [At bottom of buffer](#org0af8d53)
    2.  [At beginning of buffer](#org0613803)
    3.  [At specific line](#orgef7314c)
9.  [Inserting text](#org65af450)
    1.  [Characters](#org49534ec)
    2.  [Lines](#org97d38d5)
    3.  [Append at line](#orgcf56005)
10. [Searching / Replacing](#org56ee80f)
    1.  [Searching in text](#org6eb9bef)
    2.  [Replacing](#org15080b0)
    3.  [Matching parenthesis](#orgeb76bfd)
11. [Saving / Inserting files](#orgf2a3b85)
    1.  [Current file](#orga959869)
    2.  [Current buffer to specific file](#org7b7a948)
    3.  [Specific lines in buffer](#org918edf4)
    4.  [Inserting file in current position](#orgc5faad2)
12. [Exiting](#org3df88c8)
    1.  [Saving changes](#orge17fd9b)
    2.  [Without saving](#org10d1a8f)



<a id="org4169f60"></a>

# Movements


<a id="org782690d"></a>

## Arrow keys


<a id="orgabf9096"></a>

### You can use the arrow keys in Evil mode, it's not the best way but it works :

<kbd> <left> </kbd>   <kbd> <down> </kbd>   <kbd> <up> </kbd>   <kbd> <right> </kbd> 


<a id="org5edea99"></a>

## Evil moves


<a id="org24c16d9"></a>

### Spacemacs using Evil helps you improve fast movements with these keys :

<kbd> h </kbd>   <kbd> j </kbd>   <kbd> k </kbd>   <kbd> l </kbd> 


<a id="org1ba92b5"></a>

# Objects

Refer a word using <kbd> w </kbd>

Refer a line using <kbd> $ </kbd>


<a id="org3338cc0"></a>

# Formatting commands

Use a command on multiple objects in one row using : [number] [command] [object] OR [command] [number] [object]
Example : <kbd> 5 d w </kbd> deletes five words from cursor


<a id="orgc7e66bb"></a>

# Deletion


<a id="org114549a"></a>

## Single caracter

<kbd> x </kbd> 


<a id="orgbeae53d"></a>

## Single word

<kbd> d w </kbd>


<a id="org790202b"></a>

## Single line

<kbd> d $ </kbd>
<kbd> d d </kbd>


<a id="org2ba20d7"></a>

# Paste

<kbd> p </kbd> puts the deleted/copied/cut text after the cursor


<a id="orga297dc2"></a>

# Replace


<a id="org312dbb9"></a>

## Character

<kbd> r </kbd> replaces the character under the cursor


<a id="orgfa6b313"></a>

## Word

<kbd> c </kbd> replaces the word from the cursor 


<a id="org0bacabf"></a>

## Replace mode

<kbd> R </kbd> to enter replace mode until <kbd> <escape> </kbd> is pressed


<a id="orga2f574a"></a>

# Undos / Redos

Spacemacs remembers your actions to go back in time or move forward again. 
<kbd> u </kbd> to undo last action (keep pressed for multiple)
<kbd> C-r </kbd> to redo last action (keep pressed for multiple) 


<a id="orgc8432c3"></a>

# Moving


<a id="org0af8d53"></a>

## At bottom of buffer

<kbd> G </kbd>


<a id="org0613803"></a>

## At beginning of buffer

<kbd> g g </kbd>  


<a id="orgef7314c"></a>

## At specific line

<kbd> : </kbd>[number] moves you to line [number]


<a id="org65af450"></a>

# Inserting text


<a id="org49534ec"></a>

## Characters

<kbd> i </kbd> will open edit mode to insert a character before current cursor

<kbd> a </kbd> will open edit mode to insert a character after current cursor


<a id="org97d38d5"></a>

## Lines

<kbd> o </kbd> will open edit mode to insert a new line after current cursor

<kbd> O </kbd> will open edit mode to insert a new line before current cursor


<a id="orgcf56005"></a>

## Append at line

<kbd> A </kbd> to append text to the end of the line 


<a id="org56ee80f"></a>

# Searching / Replacing


<a id="org6eb9bef"></a>

## Searching in text

<kbd> / </kbd> followed by a phrase searches FORWARD in text 

<kbd> ? </kbd> followed by a phrase searches BACKWARD in text 


<a id="org15080b0"></a>

## Replacing

<kbd> : s / OLD / NEW </kbd>

<kbd> : s / OLD / NEW / g </kbd>

<kbd> : # , # s / OLD / NEW </kbd>

<kbd> : % s / OLD / NEW / g </kbd>

<kbd> : % s / OLD / NEW / g c </kbd>


<a id="orgeb76bfd"></a>

## Matching parenthesis

Typing <kbd> % </kbd>  while the cursor is on a  (,),[,],{, or }  locates its
matching pair.


<a id="orgf2a3b85"></a>

# Saving / Inserting files


<a id="orga959869"></a>

## Current file

<kbd> : w </kbd> to save current buffer to file


<a id="org7b7a948"></a>

## Current buffer to specific file

<kbd> : w FILENAME </kbd> to save current buffer to specific FILENAME


<a id="org918edf4"></a>

## Specific lines in buffer

<kbd> : # , # FILENAME </kbd> to save the lines # through # to specific FILENAME


<a id="orgc5faad2"></a>

## Inserting file in current position

<kbd> : r FILENAME </kbd> retrieves file FILENAME and inserts it into buffer at current position


<a id="org3df88c8"></a>

# Exiting


<a id="orge17fd9b"></a>

## Saving changes

<kbd> : q a ! </kbd>


<a id="org10d1a8f"></a>

## Without saving

<kbd> : w q a </kbd>

