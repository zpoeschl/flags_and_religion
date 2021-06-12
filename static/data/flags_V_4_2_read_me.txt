In the file flags_with_headers_v_4_1.csv, religion is encoded to more closely resemble them as assigned in the 1986 Collins Gem Guide: Flags, which Forsyth based his dataset on, with what he calls "ethnic" and the book calls "native" aggregated as other:

religion:
0 = Christianity
1 = Islam
2 = Buddhism
3 = Hinduism
4 = other

v. 4.1 removes a duplicate record for Argentina.

v. 4.2 renames "Germany_DDR" as East_Germany and "Germany_FRG" as West_Germany. This shouldn't affect machine learning, but lets the Tableau tooltip for each of these be clickable and land on the Wikipedia entry for that country's flag, instead of erroring out.