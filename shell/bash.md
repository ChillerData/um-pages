# bash --
{:data-section="shell"}
{:data-date="December 13, 2019"}
{:data-extra="Um Pages"}

## IF COMMAND IN PATH
`if [ -x "$(command -v git)" ]; then`
: executes the happy path if git is found in path

## ECHO TO STDERR
`echo "Error: git is not installed." >&2`
: redirect output to &2 which is std error

## EXTRACT FILES
`tar xvzf file.tar.gz`
: x=extract v=verbose z=uncompress(gzip) f=filename

`gunzip file.gz`
: easy

`unrar e foo.rar`
: probably install unrar first

`unzip bar.zip`
: easy
