# VI-Detailed Description

## History

VI was derived from a sequence of UNIX command line editors, starting with [ed](https://en.wikipedia.org/wiki/Ed_(text_editor)), which was a line editor designed to work well on [teleprinters](https://en.wikipedia.org/wiki/Teleprinter), rather than [display terminals](https://en.wikipedia.org/wiki/Display_terminal). Within [AT&amp;T Corporation](https://en.wikipedia.org/wiki/AT%26T_Corporation), where ed originated, people seemed to be happy with an editor as basic and unfriendly as ed, [George Coulouris](https://en.wikipedia.org/wiki/George_Coulouris_(computer_scientist)) recalls

## Installation

Generally Vi or Vim is present on most linux distros,but if its not present you can use the below mentioned code to get it:

sudo apt-get update sudo apt-get install vim

## Basic Vi Commands

To launch the VI Editor -Open Terminal (CLI) and type:

vi \&lt;filename\_NEW\&gt; or \&lt;filename\_EXISTING\&gt;



## vi Editing commands


Change commands (Input mode)

cw  -Change word (Esc)

cc   -Change line (Esc) - blanks line

c$   -Change to end of line

rc   -Replace character with c

R Replace (Esc) - typeover

. Repeat last change

Changes during insert mode

\&lt;ctrl\&gt;h   - Back one character

\&lt;ctrl\&gt;w  -Back one word

\&lt;ctrl\&gt;u   -Back to beginning of insert





# File management commands

:w - name Write edit buffer to file name

:wq - Write to file and quit

:q! - Quit without saving changes

ZZ - Same as :wq

:sh - Execute shell commands (\&lt;ctrl\&gt;d)



# Window motions

\&lt;ctrl\&gt;d - Scroll down (half a screen)

\&lt;ctrl\&gt;u - Scroll up (half a screen)

\&lt;ctrl\&gt;f - Page forward

\&lt;ctrl\&gt;b - Page backward

/string - Search forward

?string - Search backward

\&lt;ctrl\&gt;l-  Redraw screen

\&lt;ctrl\&gt;g - Display current line number and

file information

n - Repeat search

N - Repeat search reverse

G - Go to last line

nG - Go to line n

:n Go to line n

z\&lt;CR\&gt; - Reposition window: cursor at top

z. - Reposition window: cursor in middle

z- - Reposition window: cursor at bottom





External Image of Vi Command:





# Credit:

[
# https://en.wikipedia.org/wiki/Vi
](https://en.wikipedia.org/wiki/Vi)

# http://www.atmos.albany.edu/daes/atmclasses/atm350/vi\_cheat\_sheet.pdf