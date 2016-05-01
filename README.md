# xlsx2html-frontend
xlsx to XHTML and CSV converter, front end

```
git clone https://github.com/transpect/xlsx2html-frontend --recursive
```

Usage:
```
xlsxconv [options ...] <xlsx file>
```

Creates an XHTML and a CSV file from an .xlsx file

Option | Description
------ | -----------
   -c  | CSV cell separator (tab \| comma \| semicolon; default: tab)
   -d  | debug
   -l  | CSV line separator (LF \| CRLF; default: CRLF)
   -o  | output directory (default: directory of input file)
   -s  | CSV sheet separator (hyphens \| none; default: hyphens)

## Prerequisites

* Java 1.7+
* Bash

Sorry there is no Windows .bat file yet. For the time being, Windows users can invoke calabash.bat like this, from the xlsx2html-frontend directory:

```
calabash/calabash.bat -o result=out.xhtml -o csv=out.csv lib/xpl/xlsx2html.xpl in-file=path/to/file.xlsx
```
