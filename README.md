# whatisactivism

Website: https://dilancakir.github.io/whatisactivism/

Zotero: https://www.zotero.org/groups/5261383/what_is_activism/library

## About this project

*A curated collection of quotes on activism from various historical and contemporary voices.*

This repository is part of the research project **"Aktivismus und Literatur"**, a postdoctoral (Habilitation) project that explores the relationship between literature and activism across historical contexts. 
The project is currently based at the research cluster of excellence  
[**Temporal Communities – Doing Literature in a Global Perspective**](https://www.temporal-communities.de/)  
at **Freie Universität Berlin**.

The dataset is being built to document, compare, and analyze how activism is defined, narrated, and imagined in literary and para-literary texts. Each entry contains bibliographic metadata and excerpts from a primary sources, along with metadata fields to support further digital analysis.



## Field Documentation (YAML Structure)

| Field name                    | Type              | Description |
|------------------------------|-------------------|-------------|
| `id`                         | String            | Internal ID for the entry. |
| `GND`                        | List of Strings   | GND identifier(s), from the Integrated Authority File (Gemeinsame Normdatei) used in German libraries. |
| `WikiID`                     | List of Strings   | Wikidata ID(s) associated with the person. |
| `country`                    | String            | Country of origin related to the quoted publication. |
| `zotero_key`                 | String            | Key for referencing the entry in Zotero (e.g., for automated citations). |
| `language`                   | String            | Language of the quotation. |
| `person`                     | List of Objects   | List of persons quoted. |
| `person[].name`              | String            | Name of the person. |
| `person[].gender`            | String            | Gender of the person. |
| `person[].gender_provenance`| String (optional) | Indicates how the gender value was obtained. See options below. |
| `year`                       | Integer or String | Year of publication or of the source. |
| `quote`                      | Multi-line Text   | Quotation or excerpt from the source. |
| `bibliographical_info`       | String            | Notes on page of printed source or date of last access of digital source. |

---

### Notes on `gender_provenance`

To ensure transparency, the `gender_provenance` field can be used to indicate where the gender information comes from. Recommended values:

- `"inferred"` – inferred heuristically from the first name  
- `"wikidata"` – taken from a Wikidata entry  
- `"gnd"` – taken from the GND authority file  
- `"explicit"` – stated explicitly in the source  
- `"uncertain"` – unclear or ambiguous


## License

This project is licensed under the [Creative Commons BY-NC-SA 4.0 License](https://creativecommons.org/licenses/by-nc-sa/4.0/).

You are free to share and adapt the material for non-commercial purposes, as long as proper attribution is given and derivative works are licensed under the same terms.

[![License: CC BY-NC-SA 4.0](https://licensebuttons.net/l/by-nc-sa/4.0/88x31.png)](https://creativecommons.org/licenses/by-nc-sa/4.0/)


