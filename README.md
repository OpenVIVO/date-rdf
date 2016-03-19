# date-rdf
Make date RDF fpr Open VIVO

Simple Python CLI program for generating date RDF for OpenVIVO in a specified date range.  Generates year, year month and
year month day precision date time values for VIVO.  Each value has three triples:

    uri a vivo:DateTimeValue
    uri vivo:dateTimePrecision prec
    uri vivo:dateTime val^"xsd:datetime"
    
where prec is one of the three VIVO dateTimePrecision uris, and val is the isoformat datetime value

uri have the format

    http://openvivo.org/a/date
    
followed by the val
