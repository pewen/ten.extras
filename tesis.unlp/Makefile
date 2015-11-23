#target: prerequisites
#    shell_script arg1 arg2 arg3
# pandoc -V documentclass=book (book, article, extarticle)
# pandoc --chapters
# extarticle
# article
# margen setup: https://stackoverflow.com/questions/13515893/set-margin-size-when-converting-from-markdown-to-pdf-with-pandoc#13516042


TITLE="TEN. Monografía HPC UNLP"

%.html: %.md
	pandoc -s -f markdown -t html --css pandoc.css -T $(TITLE) -s -o $@ $<
#	sed -i "s/%DATE%/$(DATE)/" index.html

%.pdf: %.md
	pandoc -T $(TITLE) -N --latex-engine=xelatex -s -S --toc --chapters --standalone --from markdown --variable version=1.10 -V papersize=A4 -s -V geometry:margin=1in -V fontsize=12pt --template=latexES -o $@ $<

clean:
	rm *.html
	rm *.pdf
