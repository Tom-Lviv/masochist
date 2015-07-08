---
tags: hfs os.x
---

Files with extended attributes show up with `@` at the end of their mode string in the output of `ls -l`.

See what the attributes are with: `ls -l@`

Delete an attribute with `xattr -d [attr] [file...]` (eg. `xattr -d com.apple.quarantine *.crt`)