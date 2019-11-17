# epstopdf
epstopdf (and epstopdf-base) package for including EPS in pdftex and luatex


## Note

`epstopdf-base.sty` is included bu the pdftex and luatex options for
the core graphics package

Separating epspdf to a separate repository is a first step in removing
the dependency of the core paackage on the entire oberdiek bundle.

Currenlt the dependency is still present due to 


    \RequirePackage{infwarerr}[2007/09/09]
    \RequirePackage{grfext}\relax
    \RequirePackage{kvoptions}[2007/10/02]
    \RequirePackage{pdftexcmds}[2007/11/11]

However it should be possible in a future release to move the option
handling to (just) the full `epstopdf` package and remove the other
dependencies so that the core graphics package will only require this
distribution.
