# Braid_Data_Cleanup
This is a script written to clean data for the knot-theoretic database KnotInfo (http://www.indiana.edu/~knotinfo/). Specifically, it performs the following tasks:

1) Checks given strongly quasipositive and quasipositive braid words for consistency with the braid word given in the "Braid Notation" column for the given knot. The program also checks whether or not the given SQP or QP word represents the mirror image of the associated braid word. It does this by comparing the Jones' polynomials of the two words.

2) Outputs the SQP/QP braid words in a clean, uniform format: the braid itself is surrounded by braces ("{}"), and any maximal SQP or QP bands are also surrounded by braces. Also, if a SQP/QP word is the mirror of the word in the corresponding "Braid Notation" column, then it is prefixed by an "M".

Prior to this cleanup, several errors were found in positivity information in the KnotInfo database. These errors have since been found and corrected. Moreover, braids had previously been entered with a wide-variety of formatting styles; this script uniformizes this format. The mirror-image information had also not previously been recorded.

The hard code is contained in the notebook "braid_clean". For a pseudocode explanation of all subroutines, see the .pdf "braid_clean_pseudocode".
