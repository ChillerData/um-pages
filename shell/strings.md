# strings --
{:data-section="shell"}
{:data-date="February 07, 2020"}
{:data-extra="Um Pages"}

## STRING INDECIES
`foo=xxxfoo;echo ${foo:3}`
: chop of the first 3 characters

`foo=xxxxxxfooxxxxxx;echo ${foo:6:3}`
: chop of the first 6(offset) and continue 3(len)


## STRIP SLASHES
`shopt -s extglob # needed for globbing`
`echo ${url%%+(/)}" # strip trailing slash`
: strips all trailing slashes

# PREFIX AND SUFFIX
`${var#*/}`
`"foo/bar/baz" -> "bar/baz"`
: remove prefix ending in first "/"

`${var##*/}`
`"foo/bar/baz" -> "baz"`
: remove prefix ending in last "/"

`${var%/*}`
`"foo/bar/baz" -> "foo/bar"`
: remove suffix starting with last "/"


`${var%%/*}`
`"foo/bar/baz" -> "foo"`
: remove suffix starting with first "/"

