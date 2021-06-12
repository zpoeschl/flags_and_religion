I started with Forsyth's data set (flags.csv), then added his headers to it to create flags_with_headers.csv.

We discussed and agreed to aggregate Catholicism and other Christian into "Christianity": flags_with_headers-christianity-aggregated.csv

I got a copy of the Collins Gem Flag guide from 1986 that Forsyth based his dataset on.  We discussed further and agreed to assign the religion of the countries Forsyth marked "Marxist" to the religion listed in the Collins guide.

We further decided to try aggregating countries whose religion was marked "ethnic" as other, resulting in this:

0 = Christianity
1 = Islam
2 = Buddhism
3 = Hinduism
4 = other

v. 4.1 removes a duplicate record for Argentina.

v. 4.2 renames "Germany_DDR" as East_Germany and "Germany_FRG" as West_Germany. This lets the Tableau tooltip for each of these be clickable and reach the Wikipedia entry for that country's flag, instead of an error message.

v. 4.3 removes a row that had been labelled 193 but was otherwise blank.

Chris noticed that about thirty countries had no population, or area, or both and they were getting dropped. I went back to the Collins guide, looked up each of those countries,  and added the area and population listed there to create 

flags_with_headers_v_5.csv