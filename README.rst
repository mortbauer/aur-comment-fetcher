aur-comment-fetcher
###################
This is just a very simple script for lazy archlinux users. 

Sometimes, or quite often if some package won't build from AUR as you one
expects it is usefull to read the comments, if you are lazy like me and don't
wanna leave the command line this script will fetch the latest comments for you
and print it nicely. It uses the python3-aur package to query aur if you didn't
specify the correct name of the package at first place.

Actually there might be already better tools out there to do exactly that, but
well I couldn't find any.

so go ahead and type::

    aur-comment-fetch dvtm-git

which will result in a nicely formatted::

    2013-04-05 21:03: Comment by jsst
      The config header file in this package must be removed or updated to
      support dvtm-0.9.

Requirements:

    python-click
    python-requests
    python-beautifulsoup4
    python-lxml
    python3-aur


