ALL: ansol-lona.pdf

%.pdf: %.svg
	inkscape $< -A $@.tmp && gs -dSAFER -dBATCH -dNOPAUSE -dNOCACHE -sDEVICE=pdfwrite -sColorConversionStrategy=CMYK -dProcessColorModel=/DeviceCMYK -sOutputFile=$@ $@.tmp && rm -f $@.tmp

clean:
	rm -f *.pdf
