## Background

The intention is to archive https://ipcuk.events which was built in Drupal 7 for the International Permaculture Convergence in London in 2015.

This flat-file site was converted from Drupal 7 by http://www.httrack.com on 2.3.22.

## Issues

Internal links now point to targets with /index.html at the end eg

a href="../../about/convergences/index.html"

This results in the display of /index.html in the address bar, which is ugly. We want

http://localhost/ipcuk.events/about/convergences
to display in the address bar.

A solution is described in this blog https://www.aczoom.com/archive-2016/blog/2014-11-27/creating-a-static-drupal-site.

I think it is suggesting to search the site for all 'a' tags and remove the /index.html from the end. So

a href="../../about/convergences/index.html"

would become

a href="../../about/convergences".

Such urls display correctly already eg
http://localhost/ipcuk.events/about/convergences
will display in the address bar without the /index.html.

Unfortunately the description of the steps to implement the solution is not described in enough detail for me to replicate them.
