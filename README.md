This is a test of makefile
-----
In terminal, go to the directory *MakeTest/code*, then run *make*.

First, I run `make` when *DataAnalysis.Rmd* only does `hist(datout, nclass = 100)`, the `make` command returns DataAnalysis.nb.html exactly as expected. 

Then, I add `summary(datout)` to *DataAnalysis.Rmd* file, then run `make` again. It turns out that *DataAnalysis.nb.html* was not updated, instead, the terminal returned a message 

`make: 'DataAnalysis.nb.html' is up to date.`

Things work out fine if I change file *DataPrep.Rmd*, for example, changing `set.seed(1)` to `set.seed(2)`, then *DataAnalysis.nb.html* got updated every time.