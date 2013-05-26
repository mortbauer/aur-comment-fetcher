aur-comment-fetcher
###################
This is just a very simple script for lazy archlinux users. 

Sometimes, or quite often if some package won't build from AUR as you one
expects it is usefull to read the comments, if you are lazy like me and don't
wanna leave the command line this script will fetch the latest comments for you
and print it nicely. It does not even search the AUR, so if you give a wrong
name it will fail.

Actually there might be already better tools out there to do exactly that, but
well I couldn't find any.

so go ahead and type::

    aur-comment-fetch dvtm-git

which will result in a nicely formatted::

    2013-04-05 21:03: Comment by jsst
      The config header file in this package must be removed or updated to
      support dvtm-0.9.


