SVGS = $(wildcard *.svg)
PNGS = $(SVGS:%.svg=../gtk-3.0/img/%.png) $(SVGS:%.svg=../gtk-3.0/img/%@2.png)

all: $(PNGS)

clean:
	-rm -f $(PNGS)

../gtk-3.0/img/%.png: %.svg
	inkscape --export-dpi=90 --export-background-opacity=0 --export-filename=$@ $<

../gtk-3.0/img/%@2.png: %.svg
	inkscape --export-dpi=180 --export-background-opacity=0 --export-filename=$@ $<
