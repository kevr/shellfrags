# shellfrags

This system of scripts allows a user to define partial shell configurations
in different directories. All shell fragments found from a user's current
directory up until root (the base) will be spawned within a subshell, starting
with root and ending at the current directory. When moving around the
filesystem, subshells corresponding to directories you are no longer in are
dropped and new ones are added as they are picked up on directory change.
