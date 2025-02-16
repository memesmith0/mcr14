#!/bin/sh
#Copyright (C) 2025 by john morris beck <john.morris.beck@hotmail.com>
#
#Permission to use, copy, modify, and/or distribute this software for any purpose with or without fee is hereby granted.
#
#THE SOFTWARE IS PROVIDED "AS IS" AND THE AUTHOR DISCLAIMS ALL WARRANTIES WITH REGARD TO THIS SOFTWARE INCLUDING ALL
#
#IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS. IN NO EVENT SHALL THE AUTHOR BE LIABLE FOR ANY SPECIAL, DIRECT, INDIRECT, OR CONSEQUENTIAL DAMAGES OR ANY DAMAGES WHATSOEVER
#
#RESULTING FROM LOSS OF USE, DATA OR PROFITS, WHETHER IN AN ACTION OF CONTRACT, NEGLIGENCE OR OTHER TORTIOUS ACTION, ARISING OUT OF OR IN CONNECTION WITH THE USE OR PERFORMANCE OF

#THIS SOFTWARE.

https://github.com/memesmith0/mcr14
######################################################################################

mcr14 - tiny posix macros - we implement syntax so you don't have to

mcr14 is a prototype for an advanced macro system where the macros have macros.
it adds macros to nearly every programming language

######################################################################################

1. I can attach mcr14 to most languages
2. I can begin writing in that language as I normally do
3. If I find that I want to change the way that language is written, I can write a macro in the middle of my code. even if my code is compiled or if it is interpreted.
4. If I find that I want to change the way that my macros are written, the macros have macros. so in the middle of my code I can modify the macro langauge.
5. if I find I want to create my own macro system instead, mcr14 supports this

######################################################################################

try mcr13 yourself:

https://www.busybox.net/live_bbox/live_bbox.html

https://replit.com/languages/bash

######################################################################################

intro to code:

https://www.khanacademy.org/

######################################################################################

intro to sh:

https://mywiki.wooledge.org/FullBashGuide

https://en.wikipedia.org/wiki/POSIX

https://pubs.opengroup.org/onlinepubs/9799919799/

######################################################################################

an introduction to awk:

https://www.gnu.org/software/gawk/manual/gawk.html

https://www.amazon.com/Programming-Language-Addison-Wesley-Professional-Computing-ebook/dp/B0CCJ1N4X3

######################################################################################

mcr14 source
#!/usr/bin/sh
#Copyright (C) 2025 by john morris beck <john.morris.beck@hotmail.com>
#
#Permission to use, copy, modify, and/or distribute this software for any purpose with or without fee is hereby granted.
#
#THE SOFTWARE IS PROVIDED "AS IS" AND THE AUTHOR DISCLAIMS ALL WARRANTIES WITH REGARD TO THIS SOFTWARE INCLUDING ALL
#
#IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS. IN NO EVENT SHALL THE AUTHOR BE LIABLE FOR ANY SPECIAL, DIRECT, INDIRECT, OR CONSEQUENTIAL DAMAGES OR ANY DAMAGES WHATSOEVER
#
#RESULTING FROM LOSS OF USE, DATA OR PROFITS, WHETHER IN AN ACTION OF CONTRACT, NEGLIGENCE OR OTHER TORTIOUS ACTION, ARISING OUT OF OR IN CONNECTION WITH THE USE OR PERFORMANCE OF

#THIS SOFTWARE.
anymcr(){ if [ "$2" = "" ] ;then sh -c "$1"|sh -c "$1";else sh -c "$1"|sh -c "$1"|sh -c "$2">&2; fi;};mcr14(){ (a="(unset c f;while read -r i;do if [ \"\$i\" = m ] ;then read -r i;c=\"\$c\$i\";read -r i;f=\"\$f\$i\";else echo \"\$i\"|awk \"\$f{o=\\\$0;\$c print o}\"||exit;fi;done;)";if [ "$2" = "" ] ;then if  [ "$1" = "" ] ;then anymcr "$a"; else anymcr "$1"; fi; elif [ "$1" = "" ] ; then anymcr "$a" "$2"; else anymcr "$1" "$2"; fi;)};mcr14sh(){ mcr14 "" "sh";};
mcr14 "$@";

######################################################################################

mcr14sh source
#!/usr/bin/sh
#Copyright (C) 2025 by john morris beck <john.morris.beck@hotmail.com>
#
#Permission to use, copy, modify, and/or distribute this software for any purpose with or without fee is hereby granted.
#
#THE SOFTWARE IS PROVIDED "AS IS" AND THE AUTHOR DISCLAIMS ALL WARRANTIES WITH REGARD TO THIS SOFTWARE INCLUDING ALL
#
#IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS. IN NO EVENT SHALL THE AUTHOR BE LIABLE FOR ANY SPECIAL, DIRECT, INDIRECT, OR CONSEQUENTIAL DAMAGES OR ANY DAMAGES WHATSOEVER
#
#RESULTING FROM LOSS OF USE, DATA OR PROFITS, WHETHER IN AN ACTION OF CONTRACT, NEGLIGENCE OR OTHER TORTIOUS ACTION, ARISING OUT OF OR IN CONNECTION WITH THE USE OR PERFORMANCE OF
#
#THIS SOFTWARE.
anymcr(){ if [ "$2" = "" ] ;then sh -c "$1"|sh -c "$1";else sh -c "$1"|sh -c "$1"|sh -c "$2">&2; fi;};mcr14(){ (a="(unset c f;while read -r i;do if [ \"\$i\" = m ] ;then read -r i;c=\"\$c\$i\";read -r i;f=\"\$f\$i\";else echo \"\$i\"|awk \"\$f{o=\\\$0;\$c print o}\"||exit;fi;done;)";if [ "$2" = "" ] ;then if  [ "$1" = "" ] ;then anymcr "$a"; else anymcr "$1"; fi; elif [ "$1" = "" ] ; then anymcr "$a" "$2"; else anymcr "$1" "$2"; fi;)};mcr14sh(){ mcr14 "" "sh";};
mcr14sh;

######################################################################################
mcr14_installer.sh source
#!/bin/sh
#Copyright (C) 2025 by john morris beck <john.morris.beck@hotmail.com>
#
#Permission to use, copy, modify, and/or distribute this software for any purpose with or without fee is hereby granted.
#
#THE SOFTWARE IS PROVIDED "AS IS" AND THE AUTHOR DISCLAIMS ALL WARRANTIES WITH REGARD TO THIS SOFTWARE INCLUDING ALL
#
#IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS. IN NO EVENT SHALL THE AUTHOR BE LIABLE FOR ANY SPECIAL, DIRECT, INDIRECT, OR CONSEQUENTIAL DAMAGES OR ANY DAMAGES WHATSOEVER
#
#RESULTING FROM LOSS OF USE, DATA OR PROFITS, WHETHER IN AN ACTION OF CONTRACT, NEGLIGENCE OR OTHER TORTIOUS ACTION, ARISING OUT OF OR IN CONNECTION WITH THE USE OR PERFORMANCE OF

#THIS SOFTWARE.

https://github.com/memesmith0/mcr14
######################################################################################

mcr14 - tiny posix macros - we implement syntax so you don't have to

mcr14 is a prototype for an advanced macro system where the macros have macros.
it adds macros to nearly every programming language

######################################################################################

1. I can attach mcr14 to most languages
2. I can begin writing in that language as I normally do
3. If I find that I want to change the way that language is written, I can write a macro in the middle of my code. even if my code is compiled or if it is interpreted.
4. If I find that I want to change the way that my macros are written, the macros have macros. so in the middle of my code I can modify the macro langauge.
5. if I find I want to create my own macro system instead, mcr14 supports this

######################################################################################

try mcr13 yourself:

https://www.busybox.net/live_bbox/live_bbox.html

https://replit.com/languages/bash

######################################################################################

intro to code:

https://www.khanacademy.org/

######################################################################################

intro to sh:

https://mywiki.wooledge.org/FullBashGuide

https://en.wikipedia.org/wiki/POSIX

https://pubs.opengroup.org/onlinepubs/9799919799/

######################################################################################

an introduction to awk:

https://www.gnu.org/software/gawk/manual/gawk.html

https://www.amazon.com/Programming-Language-Addison-Wesley-Professional-Computing-ebook/dp/B0CCJ1N4X3

######################################################################################

mcr14 source
#!/usr/bin/sh
#Copyright (C) 2025 by john morris beck <john.morris.beck@hotmail.com>
#
#Permission to use, copy, modify, and/or distribute this software for any purpose with or without fee is hereby granted.
#
#THE SOFTWARE IS PROVIDED "AS IS" AND THE AUTHOR DISCLAIMS ALL WARRANTIES WITH REGARD TO THIS SOFTWARE INCLUDING ALL
#
#IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS. IN NO EVENT SHALL THE AUTHOR BE LIABLE FOR ANY SPECIAL, DIRECT, INDIRECT, OR CONSEQUENTIAL DAMAGES OR ANY DAMAGES WHATSOEVER
#
#RESULTING FROM LOSS OF USE, DATA OR PROFITS, WHETHER IN AN ACTION OF CONTRACT, NEGLIGENCE OR OTHER TORTIOUS ACTION, ARISING OUT OF OR IN CONNECTION WITH THE USE OR PERFORMANCE OF

#THIS SOFTWARE.
anymcr(){ if [ "$2" = "" ] ;then sh -c "$1"|sh -c "$1";else sh -c "$1"|sh -c "$1"|sh -c "$2">&2; fi;};mcr14(){ (a="(unset c f;while read -r i;do if [ \"\$i\" = m ] ;then read -r i;c=\"\$c\$i\";read -r i;f=\"\$f\$i\";else echo \"\$i\"|awk \"\$f{o=\\\$0;\$c print o}\"||exit;fi;done;)";if [ "$2" = "" ] ;then if  [ "$1" = "" ] ;then anymcr "$a"; else anymcr "$1"; fi; elif [ "$1" = "" ] ; then anymcr "$a" "$2"; else anymcr "$1" "$2"; fi;)};mcr14sh(){ mcr14 "" "sh";};
mcr14 "$@";

######################################################################################

mcr14sh source
#!/usr/bin/sh
#Copyright (C) 2025 by john morris beck <john.morris.beck@hotmail.com>
#
#Permission to use, copy, modify, and/or distribute this software for any purpose with or without fee is hereby granted.
#
#THE SOFTWARE IS PROVIDED "AS IS" AND THE AUTHOR DISCLAIMS ALL WARRANTIES WITH REGARD TO THIS SOFTWARE INCLUDING ALL
#
#IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS. IN NO EVENT SHALL THE AUTHOR BE LIABLE FOR ANY SPECIAL, DIRECT, INDIRECT, OR CONSEQUENTIAL DAMAGES OR ANY DAMAGES WHATSOEVER
#
#RESULTING FROM LOSS OF USE, DATA OR PROFITS, WHETHER IN AN ACTION OF CONTRACT, NEGLIGENCE OR OTHER TORTIOUS ACTION, ARISING OUT OF OR IN CONNECTION WITH THE USE OR PERFORMANCE OF
#
#THIS SOFTWARE.
anymcr(){ if [ "$2" = "" ] ;then sh -c "$1"|sh -c "$1";else sh -c "$1"|sh -c "$1"|sh -c "$2">&2; fi;};mcr14(){ (a="(unset c f;while read -r i;do if [ \"\$i\" = m ] ;then read -r i;c=\"\$c\$i\";read -r i;f=\"\$f\$i\";else echo \"\$i\"|awk \"\$f{o=\\\$0;\$c print o}\"||exit;fi;done;)";if [ "$2" = "" ] ;then if  [ "$1" = "" ] ;then anymcr "$a"; else anymcr "$1"; fi; elif [ "$1" = "" ] ; then anymcr "$a" "$2"; else anymcr "$1" "$2"; fi;)};mcr14sh(){ mcr14 "" "sh";};
mcr14sh;

######################################################################################
mcr14_installer.sh source
#!/usr/bin/sh
#Copyright (C) 2025 by john morris beck <john.morris.beck@hotmail.com>
#
#Permission to use, copy, modify, and/or distribute this software for any purpose with or without fee is hereby granted.
#
#THE SOFTWARE IS PROVIDED "AS IS" AND THE AUTHOR DISCLAIMS ALL WARRANTIES WITH REGARD TO THIS SOFTWARE INCLUDING ALL
#
#IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS. IN NO EVENT SHALL THE AUTHOR BE LIABLE FOR ANY SPECIAL, DIRECT, INDIRECT, OR CONSEQUENTIAL DAMAGES OR ANY DAMAGES WHATSOEVER
#
#RESULTING FROM LOSS OF USE, DATA OR PROFITS, WHETHER IN AN ACTION OF CONTRACT, NEGLIGENCE OR OTHER TORTIOUS ACTION, ARISING OUT OF OR IN CONNECTION WITH THE USE OR PERFORMANCE OF
#
#THIS SOFTWARE.
#https://github.com/memesmith0/mcr14
#to run this script type: sh mcr14_installer.sh
mkdir mcr14;
cd mcr14;
wget https://github.com/memesmith0/mcr14/blob/main/mcr14;
wget https://github.com/memesmith0/mcr14/blob/main/mcr14sh;
chmod +x mcr14;
chmod +x mcr14sh;
echo "you may now run mcr14 by typing: sh mcr14sh";

######################################################################################
usage

some code;
some code;
some code;
m
an awk function in one line
a line of awk code to go in the main awk program
more x code. now a new macro is applied to each line.
more macro code
more macro code

######################################################################################
inteactive shell prompt example

mrc3sh;
echo hello
echo goodbye
echo press q to quit top
top
#in a couple of lines the line will be left blank intentionlly do not skip typing this blank line
m
o="echo hello";

echo goodbye
echo anything
top
quit
exit
q
ctrl + c
ctrl + d
ctrl + z

######################################################################################
cat example

mcr3sh
m
o=$0;

echo hello
echo goodbye
type anything
a8j9v8asjo8jsao8jf8osjaf

######################################################################################
prefix example

mrc3sh;
m
o=($1 == "+") ? ($2+$3) : $0;

mrc3sh;
m
o=($1 == "-") ? ($2-$3) : $0;

mrc3sh;
m
o=($1 == "*") ? ($2*$3) : $0;

mrc3sh;
m
o=($1 == "/") ? ($2/$3) : $0;

echo hello
echo goodbye
top
+ 4 4
* 3 9
