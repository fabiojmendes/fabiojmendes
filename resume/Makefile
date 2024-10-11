# Convert all files in this directory that have a .md suffix
SOURCE_DOCS := resume.md

TARGET=fabiojmendes.pdf

PANDOC=pandoc
PANDOC_OPTIONS=--template jb2-modern.latex -f markdown+yaml_metadata_block

$(TARGET): $(SOURCE_DOCS)
	$(PANDOC) $(PANDOC_OPTIONS) -o $@ $^

all: $(TARGET)

clean:
	- rm -rf $(TARGET)
