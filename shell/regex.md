# regex --
{:data-section="shell"}
{:data-date="October 19, 2019"}
{:data-extra="Um Pages"}

## BASH

`str="123";patt="^[0-9]*$"; if [[ $str =~ $patt ]]; then echo "matches"; fi`
: requires [[ ]] and is not POSIX-shell compatible


`if [[ "123" =~ ^[0-9]*$ ]]; then echo "matches"; fi`
: no quotes around pattern
