DataAnalysis.nb.html: DataAnalysis.Rmd ../data/datout.rds
	R -e "rmarkdown::render('DataAnalysis.Rmd', 'html_notebook', 'DataAnalysis.nb.html')"
../data/datout.rds: DataPrep.Rmd
	R -e "rmarkdown::render('DataPrep.Rmd')"