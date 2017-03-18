Gentoo Manual
==

1. Use emerge -avt to install packages..
2. Use etc-update to apply new default added USE flags..
3. to install pkg use USE flags other than default:
    1. USE="a -b" emerge -avt pkg..
    2. v /etc/portage/package.use to add terms like
        "><=~path/to/package-version.num flag1 flag2.."
    3. modify /etc/portage/make.conf add/del flags.. and
then we emerge -avtuND world .. to apply new USE flag to
whole system..
4. to know what specific USE flag means, use euses -i flag..
5. to search for certain package and their flags in a quick
way, use eix pkg..
