---
tags: ragel
---

[Ragel 6.1](/wiki/Ragel_6.1) was released on 26 March 2008.

## Changelog (excerpt)

    -Scanners now ensure that any leaving actions at the end of a pattern are
     executed. They are always executed before the pattern action.
    -Added an option -d for turning off the removal of duplicate actions from
     actions lists.
    -Need to unset the final state status of the start state in kleene star if it
     is set. It is possible to crash ragel when the warning is ignored.
    -In the dot file generation we need to print any actions that are in
     State::eofTrans. These come from scanners only.
    -Use @docdir@ for the docdir Makefile variable.
    -Check for ar and ranlib in the configure script.

## See also

-   Full changelog: <http://www.cs.queensu.ca/~thurston/ragel/ChangeLog>
-   Release notes: <http://www.cs.queensu.ca/~thurston/ragel/RELEASE_NOTES_V6>
-   [Upgrading to Ragel 6.1 on Mac OS X 10.5.2 Leopard](/wiki/Upgrading_to_Ragel_6.1_on_Mac_OS_X_10.5.2_Leopard)
