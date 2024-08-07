# Package:   CMT

# Function:  An ISPF Edit Macro that simplifies the entry of comment lines
           within the data set currently being edited. The comment format
           is appropriate to the language type.

           Current language types supported include:
                ASM
                C
                CLIST
                COBOL
                DOC
                HTML
                JCL
                REXX
                SAS
                PL/I
            These are dynamically determined by 'looking' at the data
            in the data set being edited.

# Components:
            CMT      - the REXX Exec and ISPF Edit Macro
                       (copy into your SYSEXEC or SYSPROC library)
            CMTPANEL - the ISPF Panel
                       (copy into your ISPPLIB library)
            LINEMAC  - optional and provided thanks to Doug Nadel
                       http://somebody.home.mindspring.com/
                       see "LINEMAC Notes" below for usage notes.

# Warranty:   None.  Use at your own risk.
            Before using in any production mode be sure to verify that
            this works in your environment.

# Author:    Lionel B. Dyck
             lbdyck@gmail.com

# Additions: Bill George
           billgeo@bigfoot.com

# Thanks:  To Doug Nadel for sharing his LINEMAC ISPF Edit Macro which
           we have included within the CMT exec.

           Linemac Notes:
           LINEMAC is an edit macro that works in conjunction with
           Doug Nagle's LMAC or UMAC process to allow for user
           developed line commands.
           Please see http://www.mindspring.com/~somebody/
           "A few ISPF or OS/390 tools and toys" for a complete
           desciption of how to use and setup either LMAC or UMAC so
           the LINEMAC macro may be called to process user define
           line commands.

           The LINEMAC macro included here is an enhanced version
           of Mr. Nagle's original LINEMAC macro. This version contains
           many additional line commands including the ability to
           to CMT as a line command.
