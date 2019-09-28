# git --
{:data-section="shell"}
{:data-date="September 28, 2019"}
{:data-extra="Um Pages"}

things i can't remember in git

## UPDATE FORK
`git remote add ddnet https://github.com/ddnet/ddnet.git`
: i used to call those upstream but since there is ddnet and vanilla ddnet is fine

`git fetch ddnet && git checkout master && git reset --hard ddnet/master && git push origin master`
: hard reset to master deleting own commits on master
: do this on contribution branches

`git fetch ddnet && git checkout master && git rebase ddnet/master && git push origin master`
: this is used for ZillyWoods to keep master always in front of upstream to look up to date

## WARNING

all updates mess up locally cloned repos and pullrequests made prior to the merge/rebase

## FETCH PULLREQUEST

`git pull origin pull/939/head`
: 939 being the pr id and origin the remote (idk what head is tho xd)
: remote has to be fetched first
