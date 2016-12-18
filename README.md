# ipa-dictionary
Machine-readable tab-delimited dictionary files mapping words to their phonetic spellings

* Because much of this data is adapted from Wikipedia, these files are made available under the [CC-BY-SA 3.0 license](https://creativecommons.org/licenses/by-sa/3.0/)

* Vocabulary is selected for inclusion based on the [General Service List](http://jbauman.com/gsl.html) and arranged in order of GSL utility. Working from the top down in this fashion makes more important vocabulary available before less important vocabulary.

* Additional vocabulary found to be important to TTS applications are placed at the end of the list after a blank line, in alphabetical order.

* The en_US.txt file attempts to capture the most neutral, generally-accepted, non-regional American English pronunciation. There is some ambiguity about word stress; we don't include multiple word stresses, so we attempt to find the simplest and most natural-sounding solution.

* I will accept pull requests for other regions, such as en_UK, and other languages, such as zn_CH, as long as they are formatted the same way.

* Heteronyms are a significant problem for text-to-speech applications. If a certain spelling has multiple different pronunciations depending on the grammar or context, the most common use is listed first, and the others are listed in additional columns. The goal is for a "dumb" converter that reads only the first and second column to have the best general utility.

* Because much of producing the list is manual, there will be many untouched GSL words left in the list. Parsers will need to either work with a modified version of this file, or ignore lines which start with a number.
