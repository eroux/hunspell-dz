all: oxt

# https://wiki.openoffice.org/wiki/Documentation/DevGuide/Extensions/File_Format

FILES=dictionaries.xcu description.xml package-description.txt

oxt: $(FILES) ../README.md ../CHANGELOG.md ../dz.dic ../dz.aff META-INF/manifest.xml
	@echo "Making oxt file for LibreOffice..."
	@cp ../dz.dic ../dz.aff .
	@cp ../README.md .
	@zip -rq dzongkha-spellchecker.oxt dz.dic dz.aff $(FILES) META-INF README.md CHANGELOG.md

clean:
	@rm -f bo.dic bo.aff README.md CHANGELOG.md dzongkha-spellchecker.oxt
