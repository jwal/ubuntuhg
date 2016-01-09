# Ubuntuhg: Ubuntu - Mercurial mirror

Ubuntu is a distribution of the GNU/Linux operating system. Much of the
infrastructure of the distribution is based on the same tools as the Debian
distribution such as Apt and Dpkg.

Mercurial, often abbreviated as Hg, is a distributed version control tools
for computer source code and configuration files.

I can be argued that the package management infrastructure of Debian and Ubuntu
implement a rudimentary version control system. Like more traditional version
control it can track multiple versions of the same files with detailed change
histories. Unlike traditional version control it tracks the relationship
between the original source files and the binary files which are generated from
them.

Ubuntuhg explores the idea of modelling the Ubuntu package repository as
a version control system by replicating some of the key data as a Mercurial
repository.

# Motivations

The primary motivation is simply because it is an interesting experiment. There
are some other potential benefits that it might provide, though:

  - Could HTTPS replace Apt-secure file signature verification?

  - Can you time-travel the repository and build an Ubuntu computer from
    a specified historical point-in-time?

  - Would things be a little easier if the tools used JSON instead of RFC822
    messages for the metadata file formats?

# Source code

The script to maintain this repository lives in a separate Mercurial
repository:

  - https://bitbucket.org/jwal/jwallib/src/default/ubuntuhg.py
