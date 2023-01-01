## POSIX re

Besides, BRE and ERE, POSIX RE’s also has an enhanced mode. i.e. BRE, ERE,
Enhanced BRE, Enhanced ERE.

ERE usually means Enhanced ERE.

The difference between BRE and Enhanced BRE is that:

1. BRE doesn’t have `\|`
2. `\+` has to become `\{1,\}`
3. `\?` has to become `\{0,1\}`
4. `\{` and `\}` forms a bound
5. `\(` and `\)` forms a group
6. `^` and `$` are only special at the begin and the end
7. `*` isn’t special at the begin, or right after `\(`
8. Enhanced BRE has back reference, i.e. `\1`, ..., `\9`

However `man` doesn’t distinguish between BRE and Enhanced BRE.

BRE:

- `expr` `:`
- `less` `/`
- `sed`

Enhanced BRE:

- `grep`

Extended ERE:

- `sed -E`
- `grep -E`
