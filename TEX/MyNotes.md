### several lines in a cell within a table
here is a [link](https://tex.stackexchange.com/questions/40561/table-with-multiple-lines-in-some-cells).  
I use the command `\shortstack`

### reference issues
at first reference dont work. 
The problem is that I tipped some blanks before the `\label` command.  
On deleting these blanks, the reference works perfectly

### about minus sign
use the hyphen for a minus sign seems not a good idea. The symbol is too long. 
use `\newcommand{\minus}{\scalebox{0.75}[1.0]{$-$}}` and shorthand `\minus` instead.  
See the [link](https://tex.stackexchange.com/questions/79141/is-there-a-designated-symbol-for-the-negative-sign-in-say-16/500980)

### text in math mode
include the package `amsmath` and use the command `\text{}` instead.  
Beware that it seems impossible to type german alphabets `äöeß` in the maths environment.  
Only through the text mode can we type those alphabets.

### about contents
after making the titlepage, must include the line `\newpage`, or else, the contents will be empty.  
To change the name of the contents, use the command `\renewcommand{\contentsname}{Inhaltsverzeichnis}`, see [link](https://tex.stackexchange.com/questions/28516/how-to-change-the-title-of-toc)
### on pmatrix
the command `\begin{pmatrix}` has to be enclosed within a math
environment.
### some notion
* prime notion: use `\prime`, for example `f^{\prime}`
* dot notion: use `\d..dot`, for example 2-nd derivative: `\ddot{\theta}`
