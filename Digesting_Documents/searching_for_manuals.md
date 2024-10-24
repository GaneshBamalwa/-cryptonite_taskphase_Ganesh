# CTF Challenge: searching_for_manuals

## Table of Content

- commands-executed: man man , man -K challenge , /challenge/challenge --morphs 963
- flag :pwn.college{Y96Z3mUorQphs7M_ZctauOkc4Ep.dZTM4QDLzETN0czW}





### Output:
```console
hacker@man~searching-for-manuals:~$ man man
MAN(1)                        Manual pager utils                        MAN(1)

NAME
       man - an interface to the system reference manuals

SYNOPSIS
       man [man options] [[section] page ...] ...
       man -k [apropos options] regexp ...
       man -K [man options] [section] term ...
       man -f [whatis options] page ...
       man -l [man options] file ...
       man -w|-W [man options] page ...

DESCRIPTION
       man  is  the system's manual pager.  Each page argument given to man is
       normally the name of a program, utility or function.  The  manual  page
       associated with each of these arguments is then found and displayed.  A
       section, if provided, will direct man to look only in that  section  of
       the  manual.   The  default action is to search in all of the available
       sections following a pre-defined order (see DEFAULTS), and to show only
       the first page found, even if page exists in several sections.

       The table below shows the section numbers of the manual followed by the
       types of pages they contain.

       1   Executable programs or shell commands
       2   System calls (functions provided by the kernel)
       3   Library calls (functions within program libraries)
       4   Special files (usually found in /dev)
       5   File formats and conventions, e.g. /etc/passwd
       6   Games
       7   Miscellaneous (including  macro  packages  and  conventions),  e.g.
           man(7), groff(7)
       8   System administration commands (usually only for root)
       9   Kernel routines [Non standard]

       A manual page consists of several sections.

       Conventional  section  names include NAME, SYNOPSIS, CONFIGURATION, DE‐
       SCRIPTION, OPTIONS,  EXIT STATUS,  RETURN VALUE,  ERRORS,  ENVIRONMENT,
       FILES,  VERSIONS,  CONFORMING TO,  NOTES,  BUGS,  EXAMPLE, AUTHORS, and
       SEE ALSO.

       The following conventions apply to the SYNOPSIS section and can be used
       as a guide in other sections.

       bold text          type exactly as shown.
       italic text        replace with appropriate argument.
       [-abc]             any or all arguments within [ ] are optional.
       -a|-b              options delimited by | cannot be used together.
       argument ...       argument is repeatable.
       [expression] ...   entire expression within [ ] is repeatable.

       Exact rendering may vary depending on the output device.  For instance,
       man will usually not be able to render italics when running in a termi‐
       nal, and will typically use underlined or coloured text instead.

       The command or function illustration is a pattern that should match all
       possible invocations.  In some cases it is advisable to illustrate sev‐
       eral  exclusive invocations as is shown in the SYNOPSIS section of this
       manual page.

EXAMPLES
       man ls
           Display the manual page for the item (program) ls.

       man man.7
           Display the manual page for  macro  package  man  from  section  7.
           (This is an alternative spelling of "man 7 man".)

       man 'man(7)'
           Display  the  manual  page  for  macro  package man from section 7.
           (This is another alternative spelling of "man 7 man".   It  may  be
           more convenient when copying and pasting cross-references to manual
           pages.  Note that the parentheses must normally be quoted  to  pro‐
           tect them from the shell.)

       man -a intro
           Display,  in  succession,  all  of the available intro manual pages
           contained within the manual.  It is possible to quit  between  suc‐
           cessive displays or skip any of them.

       man -t bash | lpr -Pps
           Format  the  manual  page  for bash into the default troff or groff
           format and pipe it to the printer named ps.  The default output for
           groff  is usually PostScript.  man --help should advise as to which
           processor is bound to the -t option.

       man -l -Tdvi ./foo.1x.gz > ./foo.1x.dvi
           This command will decompress and format  the  nroff  source  manual
           page  ./foo.1x.gz  into a device independent (dvi) file.  The redi‐
           rection is necessary as the -T flag causes output to be directed to
           stdout  with  no  pager.  The output could be viewed with a program
           such as xdvi or further processed into PostScript using  a  program
           such as dvips.

       man -k printf
           Search the short descriptions and manual page names for the keyword
           printf as regular expression.  Print out any  matches.   Equivalent
           to apropos printf.

       man -f smail
           Lookup the manual pages referenced by smail and print out the short
           descriptions of any found.  Equivalent to whatis smail.

OVERVIEW
       Many options are available to man in order to give as much  flexibility
       as  possible to the user.  Changes can be made to the search path, sec‐
       tion order, output processor, and other behaviours and  operations  de‐
       tailed below.

       If set, various environment variables are interrogated to determine the
       operation of man.  It is  possible  to  set  the  "catch-all"  variable
       $MANOPT  to  any string in command line format, with the exception that
       any spaces used as part of an option's argument must be  escaped  (pre‐
       ceded by a backslash).  man will parse $MANOPT prior to parsing its own
       command line.  Those options requiring an argument will  be  overridden
       by the same options found on the command line.  To reset all of the op‐
       tions set in $MANOPT, -D can be specified as the initial  command  line
       option.  This will allow man to "forget" about the options specified in
       $MANOPT, although they must still have been valid.

       Manual pages are normally stored in nroff(1) format under  a  directory
       such  as /usr/share/man.  In some installations, there may also be pre‐
       formatted cat pages to improve performance.  See manpath(5) for details
       of where these files are stored.

       This package supports manual pages in multiple languages, controlled by
       your locale.  If your system did not set this up for you automatically,
       then  you may need to set $LC_MESSAGES, $LANG, or another system-depen‐
       dent environment variable to indicate your  preferred  locale,  usually
       specified in the POSIX format:

       <language>[_<territory>[.<character-set>[,<version>]]]

       If  the  desired page is available in your locale, it will be displayed
       in lieu of the standard (usually American English) page.

       If you find that the translations supplied with this  package  are  not
       available  in  your  native language and you would like to supply them,
       please contact the maintainer who will be coordinating such activity.

       Individual manual pages are normally  written  and  maintained  by  the
       maintainers  of  the  program, function, or other topic that they docu‐
       ment, and are not included with this package.  If you find that a  man‐
       ual  page is missing or inadequate, please report that to the maintain‐
       ers of the package in question.

       For information regarding other features and extensions available  with
       this manual pager, please read the documents supplied with the package.

DEFAULTS
       The  order  of  sections to search may be overridden by the environment
       variable $MANSECT or by the SECTION directive  in  /etc/manpath.config.
       By default it is as follows:

              1 n l 8 3 2 3posix 3pm 3perl 3am 5 4 9 6 7

       The  formatted  manual  page  is  displayed using a pager.  This can be
       specified in a number of ways, or else will fall back to a default (see
       option -P for details).

       The  filters are deciphered by a number of means.  Firstly, the command
       line option -p or the environment variable $MANROFFSEQ is interrogated.
       If  -p  was not used and the environment variable was not set, the ini‐
       tial line of the nroff file is parsed for a  preprocessor  string.   To
       contain a valid preprocessor string, the first line must resemble

       '\" <string>

       where  string  can be any combination of letters described by option -p
       below.

       If none of the above methods provide any filter information, a  default
       set is used.

       A  formatting  pipeline is formed from the filters and the primary for‐
       matter (nroff or [tg]roff with -t) and executed.  Alternatively, if  an
       executable program mandb_nfmt (or mandb_tfmt with -t) exists in the man
       tree root, it is executed instead.  It gets passed  the  manual  source
       file, the preprocessor string, and optionally the device specified with
       -T or -E as arguments.

OPTIONS
       Non-argument options that are duplicated either on the command line, in
       $MANOPT,  or  both, are not harmful.  For options that require an argu‐
       ment, each duplication will override the previous argument value.

   General options
       -C file, --config-file=file
              Use this user configuration file  rather  than  the  default  of
              ~/.manpath.

       -d, --debug
              Print debugging information.

       -D, --default
              This  option is normally issued as the very first option and re‐
              sets man's behaviour to its default.  Its use is to reset  those
              options  that  may  have  been set in $MANOPT.  Any options that
              follow -D will have their usual effect.

       --warnings[=warnings]
              Enable warnings from groff.  This may be used to perform  sanity
              checks on the source text of manual pages.  warnings is a comma-
              separated list of warning names; if it is not supplied, the  de‐
              fault  is  "mac".   See  the “Warnings” node in info groff for a
              list of available warning names.

   Main modes of operation
       -f, --whatis
              Equivalent to whatis.  Display a short description from the man‐
              ual page, if available.  See whatis(1) for details.

       -k, --apropos
              Equivalent  to  apropos.   Search the short manual page descrip‐
              tions for keywords and display any matches.  See apropos(1)  for
              details.

       -K, --global-apropos
              Search  for  text  in  all  manual pages.  This is a brute-force
              search, and is likely to take some time; if you can, you  should
              specify  a section to reduce the number of pages that need to be
              searched.  Search terms may be simple strings (the default),  or
              regular expressions if the --regex option is used.

              Note that this searches the sources of the manual pages, not the
              rendered text, and so may include false positives due to  things
              like  comments  in  source  files.   Searching the rendered text
              would be much slower.

       -l, --local-file
              Activate "local" mode.  Format and display  local  manual  files
              instead  of  searching  through  the system's manual collection.
              Each manual page argument will be interpreted as an nroff source
              file in the correct format.  No cat file is produced.  If '-' is
              listed as one of the arguments, input will be taken from  stdin.
              When this option is not used, and man fails to find the page re‐
              quired, before displaying the error message, it attempts to  act
              as if this option was supplied, using the name as a filename and
              looking for an exact match.

       -w, --where, --path, --location
              Don't actually display the manual page, but do print  the  loca‐
              tion  of  the source nroff file that would be formatted.  If the
              -a option is also used, then print the locations of  all  source
              files that match the search criteria.

       -W, --where-cat, --location-cat
              Don't  actually  display the manual page, but do print the loca‐
              tion of the preformatted cat file that would be  displayed.   If
              the -a option is also used, then print the locations of all pre‐
              formatted cat files that match the search criteria.

              If -w and -W are both used, then print both source file and  cat
              file  separated  by a space.  If all of -w, -W, and -a are used,
              then do this for each possible match.

       -c, --catman
              This option is not for general use and should only  be  used  by
              the catman program.

       -R encoding, --recode=encoding
              Instead  of  formatting the manual page in the usual way, output
              its source converted to the specified encoding.  If you  already
              know  the  encoding  of  the  source file, you can also use man‐
              conv(1) directly.  However, this option allows  you  to  convert
              several  manual pages to a single encoding without having to ex‐
              plicitly state the encoding of each, provided that they were al‐
              ready  installed in a structure similar to a manual page hierar‐
              chy.

              Consider using man-recode(1)  instead  for  converting  multiple
              manual  pages,  since it has an interface designed for bulk con‐
              version and so can be much faster.


hacker@man~searching-for-manuals:~$ man -K challenge

CHALLENGE(1)                  Challenge Commands                  CHALLENGE(1)

NAME
       /challenge/challenge - print the flag!

SYNOPSIS
       challenge OPTION

DESCRIPTION
       Output the flag when called with the right arguments.

       --fortune
              read a fortune

       --version
              output version information and exit

       --morphs NUM
              print the flag if NUM is 963
```
AUTHOR
       Written by Zardus.
--Man-- next: mysql(1) [ view (return) | skip (Ctrl-D) | quit (Ctrl-C) ]
^C
hacker@man~searching-for-manuals:~$ /challenge/challenge --morphs 963
Correct usage! Your flag: pwn.college{Y96Z3mUorQphs7M_ZctauOkc4Ep.dZTM4QDLzETN0czW}
