
# minitools
# RStudio Text Utilities

An R package and collection of Addins designed to streamline text manipulation directly within the RStudio IDE. These scripts leverage the `rstudioapi` to interact with the active document context, allowing users to modify selected text blocks efficiently without leaving their workflow.

---

take a look at my youtube playlist to see some of the functions in this package
my playlist with R Tutorials: 

---

https://www.youtube.com/playlist?list=PLRbCt61PaxX2d0_QXh6Qi6_jAQd66fmcI

---


### Defined Functions

**aligntext**
This function cleans up the formatting of the currently selected text. It splits the selection into individual lines, trims leading and trailing whitespace from each line using `stringr::str_trim`, and then re-inserts the cleaned text back into the RStudio document.

**lowercase**
This function converts all characters in the selected text to lower case. It processes the selection line-by-line, applying the base R `tolower` transformation before updating the document.

**sentencecase**
This function applies sentence-style capitalization to the selected text. Utilizing `stringr::str_to_sentence`, it ensures the first letter of each line (or string segment) is capitalized while the remainder is converted to lower case.

**sortascending**
This function reorders the selected lines of text in ascending alphabetical order (A-Z). It captures the selection, sorts the lines using R's internal sorting logic with `decreasing = FALSE`, and replaces the original selection with the ordered list.

**sortdescending**
This function reorders the selected lines of text in descending alphabetical order (Z-A). Similar to the ascending version, it sorts the captured lines with `decreasing = TRUE` and overwrites the active selection in the editor.

**titlecase**
This function transforms the selected text into title case, where the first letter of every major word is capitalized. It utilizes the `stringr::str_to_title` function to perform the conversion before re-inserting the text into the active document.

**uppercase**
This function converts all characters within the selected text to upper case. It applies the base R `toupper` function to the selection, providing a quick way to emphasize or format headers and constants.

**sortfunctions**
This function inserts current Functions loaded on Global Environment into the active document. 




