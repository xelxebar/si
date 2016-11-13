# si

The suckless IRC client.

This is a simple bash wrapper script around the ii IRC client from the suckless
project ([suckless.org][1]).

The ii client exposes the IRC protocol to the linux filesystem, and si uses
`tmux` to split a terminal into "input" and "output" areas. The output area is
essentially just `tail` with GNU `grep` to provide some filtering and
colorization.

Input is handled via vim but should act as expected, *i.e.* messages are "sent"
on a carriage return.


## Installation

To install, simply run

    $ make [PREFIX=<prefix>] [SI_CONFIG=<si_conf_dest>] install

where optionally PREFIX specifies where the root for bin/ into which the
executable will be installed and SI_CONFIG optionally specifies the path into
which to install the si configuration file. Note that SI_CONFIG defaults to
$HOME/.config/si/config.


[1]:http://suckless.org/
