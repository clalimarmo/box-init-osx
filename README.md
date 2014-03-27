# Set us up the box

1. install xcode
2. open xcode and agree to license
3. run `./setup`

# Usage

Running any of the scripts included here should be done from the top level
directory - all the relative paths assume this. For example, installing adium
should be `./installers/adium`, and not `./adium`.

The `update/` directory contains scripts for extracting current preferences
into files that can be included here. For example, `update/iterm2-preferences`
copies the current iterm2 config file and converts it from binary to a diffable
thing. The `installers/iterm2` script converts it back, and copies it into place.

# Maintaining

Add an installation script for anything I don't want to have to install
manually on a new OSX machine to the `installers` directory. Update the `setup`
script so that it runs as per the instructions at the top of this document.

Try to keep anything that will require user input at the very beginning or end
of the setup script, so that it can mostly finish, once it's been kicked off.
