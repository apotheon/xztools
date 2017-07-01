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
