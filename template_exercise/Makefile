##
# gmt-zusammenfassung
#
# @file
# @version 0.1

COMPILER=lualatex
FILENAME=exercise.tex

.PHONY: all
all:
	$(COMPILER) $(FILENAME)

.PHONY: full
full:
	# To refresh everything (page numbers, toc, etc.) we have to compile 3 times
	$(COMPILER) $(FILENAME)
	$(COMPILER) $(FILENAME)
	$(COMPILER) $(FILENAME)

.PHONY: test
test:
	time $(COMPILER) $(FILENAME)

.PHONY: silent
silent:
	$(COMPILER) -interaction=batchmode $(FILENAME)

# end
