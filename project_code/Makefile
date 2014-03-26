zenimages.min.user.js: zenimages.user.header zenimages.min.js 
	cat $^ > $@

zenimages.user.header: zenimages.user.js
	sed -ne '/==UserScript/,/==\/UserScript/p' < $< > $@

zenimages.min.js: zenimages.user.js
	@echo Cut user.js header from $< 
	@echo Compile with http://closure-compiler.appspot.com/home 
	@echo Save to $@

zenimages.user.js: colorPaletteWidget.js
	@echo Insert $< into $@

colorPaletteWidget.js: colorPaletteWidgetOneLine.html
	sed 's/^/widget.innerHTML='\''/;s/$$/'\'';/' < $< > $@ 

colorPaletteWidgetOneLine.html: colorPaletteWidget.html
	tr -d '\n\t' < $< > $@

colorPaletteWidget.html: tpxColors.html
	@echo Insert $< into $@

tpxColors.html: tpxColors
	awk -F"	" '{print "<div class=\"colorPaletteWidget_color\" id=\"cpw"$$1"\" style=\"background-color:"$$2"\" title=\""$$4" - "$$2"\"></div>"}' < $<  > $@
