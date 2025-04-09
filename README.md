# whatisactivism

Website: https://dilancakir.github.io/whatisactivism/

Zotero: https://www.zotero.org/groups/5261383/what_is_activism/library

##YAML 

Field name	Type	Description
id	String	Internal ID or unique identifier for the entry.
GND	List of Strings	GND identifier(s), from the Integrated Authority File (Gemeinsame Normdatei) used in German libraries.
WikiID	List of Strings	Wikipedia or Wikidata ID(s) associated with the entry.
country	String	Country of origin related to the person(s) or the source.
zotero_key	String	Key for referencing the entry in Zotero (e.g., for automated citations).
language	String	Language of the source or quotation.
person	List of Objects	List of persons involved.
person[].name	String	Name of the person.
person[].gender	String	Gender of the person. If not explicitly stated, inferred heuristically from the first name.
person[].gender_provenance	String (optional)	Indicates how the gender value was obtained. See options below.
year	Integer or String	Year of publication or of the source.
quote	Multi-line Text	Quotation or excerpt from the source.
bibliographical_info	String	Full bibliographical reference (e.g., in APA or MLA style).

##Notes on gender_provenance

To ensure transparency, the gender_provenance field can be used to indicate where the gender information comes from. Recommended values:

    "assumed_from_name" – inferred heuristically from the first name

    "wikidata" – taken from a Wikidata entry

    "gnd" – taken from the GND authority file

    "explicit" – stated explicitly in the source

    "uncertain" – unclear or ambiguous

## License

This project is licensed under the [Creative Commons BY-NC-SA 4.0 License](https://creativecommons.org/licenses/by-nc-sa/4.0/).

You are free to share and adapt the material for non-commercial purposes, as long as proper attribution is given and derivative works are licensed under the same terms.

[![License: CC BY-NC-SA 4.0](https://licensebuttons.net/l/by-nc-sa/4.0/88x31.png)](https://creativecommons.org/licenses/by-nc-sa/4.0/)

