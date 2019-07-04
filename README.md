# Shell01
Piscine

ex07: cat /etc/passwd | sed -e "/#/d" | sed -n "n;p" | cut -d : -f1 | rev | sort -r | sed -n "$FT_LINE1,$FT_LINE2 p" | tr '\n' ',' | sed "s/,/& /g" | sed "s/..$/./"

!Write a command line that displays the output of a cat /etc/passwd command     > cat /etc/passwd

!removing comments,     > sed -e "/#/d"

!every other line starting from the second line (skip the first, show the second)     > sed -n "n;p"

! alleen login   > cut -d : -f1

!reversing each login,    > rev

!sorted in reverse alphabetical order,    > sort -r

between FT_LINE1 and FT_LINE2 included,    > sed -n "$FT_LINE1,$FT_LINE2 p"
 
!and they must separated by ", " (without quotation marks),     > tr '\n' ',' | sed "s/,/& /g"

!and the output must end with a ".".    > sed "s/$/./"
