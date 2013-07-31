---
tags: bash
---

-   `$1`, `$2`...: parameter 1, parameter 2 etc
-   `$#`: count of params
-   `$@`: all params
-   `$*`: same as `$@`
-   `${@:2}`: params 2 through N
-   `${@:2:5}`: 5 params, starting at param 2
-   `"$@"`: quoted params 2 through N (ie. `"$1" "$2" "$3"`...)
-   `"$*"`: quoted params 2 through N, joined using the first character of `$IFS` (ie. `"$1 $2 $3"`...)

# Related

-   `$_`: last argument of last command (eg. `echo foo && echo $_` prints "foo" twice)

# See also

-   <http://wiki.bash-hackers.org/scripting/posparams>
