# date-rdf

Make date RDF for VIVO

Simple Python CLI program for generating date RDF for VIVO in a specified date range.  Generates year, year month and
year month day precision date time values for VIVO.  Each value has three triples:

    uri a vivo:DateTimeValue
    uri vivo:dateTimePrecision prec
    uri vivo:dateTime val^"xsd:dateTime"
    
where prec is one of the three VIVO dateTimePrecision uris, and val is the isoformat datetime value

uri have the format

    http://openvivo.org/a/date
    
followed by the val

## Creating the RDF

To create the RDF

1. Edit the start_year and stop_year values in `gen_date_rdf.py`
2. `python gen_date_rdf.py`
3. Load the file `dates.rdf` to VIVO
