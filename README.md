# Shell01
Piscine

ex07: 

!Write a command line that displays the output of a cat /etc/passwd command     > cat /etc/passwd

!removing comments,     > sed -e '/#/d'

!every other line starting from the second line (skip the first, show the second)     > sed -n "n;p"

!reversing each login,    > rev

!sorted in reverse alphabetical order,    > sort -r

!and keeping only logins between FT_LINE1 and FT_LINE2 included,    > sed -n "$FT_LINE1,$FT_LINE2 p"
 
!and they must separated by ", " (without quotation marks),     > tr /\n/,/

!and the output must end with a ".".    > sed "s/, /./"

!alleen het deel van de login naam "_*:"    > 
