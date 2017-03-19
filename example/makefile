DOCUMENT_NAME = dokumentation
OUTPUT_DIR    = output

all: outputdir-legacy report-legacy

# Create LaTeX output directory.
outputdir-legacy:
	$(shell mkdir $(OUTPUT_DIR) 2>/dev/null)

# Generate PDF output from LaTeX input files.
report-legacy: 
	pdflatex -interaction=errorstopmode -output-directory=$(OUTPUT_DIR) $(DOCUMENT_NAME)
