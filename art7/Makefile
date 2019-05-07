all:article article_wrapper
	
article:
	latexmk -pdf -silent -pdflatex="xelatex %O %S" article
article_wrapper:
	latexmk -pdf -silent -pdflatex="xelatex %O %S" article_wrapper

clean:
	latexmk -C article
	latexmk -C article_wrapper
	rm -f article.bbl
	rm -f article_wrapper.bbl

distclean:
	find . -regex ".*\.\(aux.*\|lof\|log\|lot\|fls\|out\|toc\|dvi\|bbl\|bcf\|blg\|brf\|run.xml\|fdb_latexmk\|synctex.*\|pdfsync\|alg\|loa\|thm\|nav\|snm\|vrb\|acn\|acr\|glg\|glo\|gls\|lol\|ilg\|ind\|ist\|maf\|mtc.*\|pyg\|mw\|fmt\|nlo\|sagetex.*\|sout\|sympy\|upa\|upb\|pytxcode\|texpadtmp\|dpth\|md5\|tdo\|xdy\|bak\|sav\|ttt\|fff\|ps\)" -delete
