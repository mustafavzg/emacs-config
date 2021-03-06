Introduction
------------
This is my new Emacs configuration (old one can be [found here](https://github.com/ryanwersal/hipplej-emacs)). It currently is still based largely on [Justin Hipple's Emacs configuration](https://github.com/hipplej/hipplej-emacs) but I am hoping it will trend towards becoming a relatively distinct config. As of late, a lot of inspiration has also been taken from [Magnar Sveen's .emacs.d repo](https://github.com/magnars/.emacs.d/).

Why a new config?
-----------------
There are a couple motivations for the new configuration. The largest was that for the past 6-8 months I have been using [Sublime Text 2](http://www.sublimetext.com/). It has mostly been a good experience except I have run into a handful of impactful performance issues largely related to installed plugins (I'm looking at you [SublimeRope](http://www.sublimetext.com/)!) which were admittedly related to conditions outside their control. 

Between that and my growing affection for Clojure (and probably Lisps in general), I've decided to "come back home" to Emacs. 

Install
-------
1. Clone this repo as ~/.emacs.d
2. Run `git submodule update --init`
3. Launch Emacs and `M-x list-packages`, hit `U` then `x` to update the ELPA managed packages.
4. Restart Emacs and you're set to go!

#### Helm
Using [Helm](https://github.com/emacs-helm/helm) on Windows requires installing [Everything](http://www.voidtools.com/download.php) as per the [wiki](https://github.com/emacs-helm/helm/wiki#wiki-windowsspecificity). I ended up having to download both the installer and the standalone es.exe. I just placed all of it in Everything's install directory, added that directory to the PATH, and everything was set. 

#### Flycheck
Flycheck has numerous linters available. This config is currently setup to leverage only three though: python-flake8, emacs-lisp, and javascript-jshint. 
 - python-flake8 will require you to [install flake8](https://pypi.python.org/pypi/flake8) before it works.
 - Emacs-lisp works out of the box.
 - javascript-jshint requires [installing jshint](http://www.jshint.com/install/). You will need to have Node installed first.
