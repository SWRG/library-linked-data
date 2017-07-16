# Data Summary

This folder contains the summary of data collected by the aggregator tool.

Data are stored in file `total-stats-summary.csv` in the form of a matrix with 5 columns. For each row:

1. **Resource:** the URI of the resource that the SPARQL endpoint refers to. The exact resource URI is irrelevant to the statistical analysis. In fact, the values of this column have been truncated to a namespace prefix (e.g. `http://id.loc.gov/authorities/sh85049778` has been truncated to `http://id.loc.gov/authorities`).

2. **Endpoint:** the hostname of the SPARQL endpoint that contains the resource  of column 1 in one or more of its triples. The exact URLs of the endpoints can be found in the separate file `endpoints.tsv`.

3. **Predicate:** the predicate used in the triples of the endpoint (column 2) mentioning the resource (column 1). Multiple rows with different predicates per endpoint/resource may exist. For presentation purposes the predicates are abbreviated by using a prefix list stored in file `namespaces.tsv`.

4. **Count:** the number of triples of the endpoint (column 2) that refer to the resource (column 1) having as predicate the value of column 3.

5. **Provider:** a textual label designating the data provider that owns the resource of column 1.




