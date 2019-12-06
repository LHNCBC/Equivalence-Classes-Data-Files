# Equivalence Classes for LOINC Terms (LOINC version 2.66)

For some purposes, such as a Clinical or EHR flowsheet, it is useful to regard
groups of [LOINC](https://loinc.org/) terms as equivalent.  We call these groups
"equivalence classes", and have defined a set of rules for generating them.  The
rules vary between the various LOINC "classes" (e.g. CHEM, DRUG/TOX, etc.), so
the equivalence classes generated by applying those rules are are organized in
this package by LOINC class, with one spreadsheet of equivalence classes per
LOINC class.

The spreadsheets are formatted for easy review of the generated equivalence
classes, with header rows for each (generated) equivalence class name over the
rows of LOINC terms placed into that equivalence class.  The columns include the
LOINC number and the component, as well as columns for fields used in grouping
the terms into classes.  For example, when METHOD_TYP values are grouped as a
part of forming equivalence classes, there will a METHOD_REV ("revised") column
in the spreadsheet next to METHOD_TYP, with the differences highlighted.

For ease of using the spreadsheets programmatically, the equivalence class
names are also present next to each LOINC number in a hidden column.

Documentation for the rationale, approach, and rules used in generating the
equivalence classes (though still a work-in-progress) is available in
Documentation-for-Equivalence-Classes.pdf.

The code for generating these classes is also available at
https://github.com/lhncbc/loinc-equivalence-classes.

Please note that use of LOINC content must conform to the LOINC [terms of
use](https://loinc.org/terms-of-use).
