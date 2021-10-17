# plot csv files

> I need this program to plot different csv files for my labs.

Information can be distributed in rows or collumns but the first row or column 
will be used as labes.

In the program the information is distributed in rows, if the information is
distributed in columns the condition for the file to be transposed is that the
last element on the first row should be convertible to float, otherwise I am not
shure what will happen.

The first element will be used as OX label if is not set with the flag.

By default this program will try to plot every csv file from a ./csv folder to 
a ./png folder.

optional arguments:
```
  -h, --help            show this help message and exit
  -v                    verbose
  -d                    debug; output csv file content if something went wrong
  --transpose           transpose csv file, wont plot anything will create a new folder with
                        transposed csv content
  -f FILENAME           plot only one file
  -i DIR                input directory, default ./csv
  -o DIR                output directory, default ./png
  -x 'str'              x label
  -y 'str'              y label
  -t 'str'              title
  --main MAIN           select which of the rows or columns should be used as x axis, 0 will be the
                        first index
  --ignore IGNORE [IGNORE ...]
                        select which of the rows or columns shouldn't be used, 0 will be the first
                        index, -1 will ignore the last element
  --plot PLOT [PLOT ...]
                        choose what columns or rows to use for plotting y axis, 0 will be the first
                        index
```
