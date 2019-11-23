# epstopdf
epstopdf (and epstopdf-base) package for including EPS in pdftex and luatex


## Note

`epstopdf-base.sty` is included by the pdftex and luatex options for
the core graphics package

Separating epspdf to a separate repository is a first step in removing
the dependency of the core package on the entire oberdiek bundle.

Currently the dependency is still present due to 


    \RequirePackage{infwarerr}[2007/09/09]
    \RequirePackage{grfext}\relax
    \RequirePackage{kvoptions}[2007/10/02]
    \RequirePackage{pdftexcmds}[2007/11/11]

