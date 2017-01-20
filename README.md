# drush-master
Drush Master
==============

`drush-master updatedb`
`drush-master cc all`

We are facing an issue when running drush -y @sites updatedb to do the update to all existed sites.
The problem is when the number of the sites is big (~1000), the script stopped even the memory limit was increased to 2Gb.

We can fix the multi aliases running algorithm by running below script
`drush-master updatedb`

The issue has been reported in Drush without any actions so I decided to fix this. Issue is located here https://github.com/drush-ops/drush/issues/2424


P/s: I also recommend to use tmux to run it in a background session.
