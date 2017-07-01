# xztools

The xz project comes with a small set of auxiliary tools written as shell
scripts to perform convenience functions, such as showing a diff of the
contents of an xz archive.  These tools are, for some reason, licensed quite
differently from the rest of the xz project.  In the community spirit of the
open source world, we want to help expunge the license philosophy inconsistency
from the xz project by rewriting these tools.  Copyfree all the things!

Of course, rewriting from scratch is more work than just swiping someone else's
code under a friendly license and tweaking to suit.  As such, the current plan
is to lift code for equivalent tools from the bzip2 project and adapt them to
xz, then submit them to xz upstream for inclusion in the project.

The possibility of the submission getting rejected does exist.  If the xz
maintainer rejects the submitted replacement tools with good cause, we'll
endeavor to make reasonable changes to suit.  Otherwise, rejection may just
lead to releasing this set of new tools as a separate package altogether.

## development

1. Modify one of the `bz*` tools to work with xz instead of bzip2.
2. Change the name to the xz equivalent.
3. Commit.
4. . . .
5. Profit!

## testing

We'd really like to test-drive this.  The tools are shell scripts written in
(POSIX-ish) sh.  Any input on how to write tests for that sort of thing (with
copyfree tools) would be nice.

## other

You can get a bzip2 tarball from here:

    http://bzip.org/downloads.html

You can see the tools we want to replace (xzdiff, xzgrep, xzless, xzmore) here:

    https://git.tukaani.org/?p=xz.git;f=src/scripts;hb=HEAD

## copying

This project contains code borrowed from the bzip2 project.  This code is made
available under the terms specified in the LICENSE.bzip2 file.

We should ask the bzip2 devs if they would terribly mind us relicensing under
the terms of the main xztools project license.

The main xztools project license terms are specified in the LICENSE file.  This
includes any new code contributed to this project, and the project as a
whole/collection.

For the sake of convenience, we consider this project as a whole dual-licensed
with the bzip2 license terms at this time as well.
