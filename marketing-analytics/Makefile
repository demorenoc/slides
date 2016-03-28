R_OPTS=--vanilla --slave -e

index.html: main.rmd content/* img/* _output.yaml styles.css
	R $(R_OPTS) "rmarkdown::render('main.rmd')"
	mv main.html index.html
	
clean:
	rm -rf index.html libs/ main_files/ cache/
