Problem of `history.back()` is that it’s possible that there is nothing to go
back and you don't know where it goes to.

To avoid this problem, make the current page take an optional parameter for
where to go back.

Same applies to `StackActions.pop()` or `Referrer`.
