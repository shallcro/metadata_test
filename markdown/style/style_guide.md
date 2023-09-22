# ICPSR Curated Study Metadata Style Guide

**Completeness:** Regardless of whether a metadata element is technically required, curators should strive to include information for as many elements as possible. While PI-provided information often informs the metadata, curators should attempt to produce complete metadata text whenever possible (especially for elements such as "Description of Variables" or "Purpose of the Study" where the curators’ knowledge should be sufficient without PI-provided text). 

**Links:** In general, URLs should not be displayed in the metadata when referring to an online resource; instead, a hyperlink should be attached to appropriate descriptive text, as this is friendlier to screen readers and web scrapers. As an example, use "more information is available at [the project website](https://example.com)", rather than "more information is available at the project website: [https://example.com/project](https://example.com/project)". When referring to ICPSR studies, the ICPSR identifier (e.g., study number) should be used for the descriptive text, with the ICPSR DOI used as the link (see below for additional information). *Note:* formal citations are an important exception to this rule; the URL (preferably a persistent identifier, like a DOI) should always be included for the cited resource.

**How to correctly refer to ICPSR studies within metadata text:** When using an identifier (study number) within metadata text, "ICPSR" should precede the number, e.g., "This collection continues the work of ICPSR 23421." Four digit numbers do not require a leading 0 when they are referenced with study metadata (but please note that DOIs DO contain leading 0s). Also, using a version number within metadata text is not common; if necessary, simply append the version to the study number (e.g., ICPSR 23421-v2).

As noted above in the "Links" section, when an ICPSR identifier is referenced in metadata text, the study DOI should be included as a hyperlink. (See below for details on using a DOI within metadata text). 

**Using a DOI within metadata text:** All DOIs have both "versioned" formats and "unversioned" formats. When referencing DOIs or including them as links, the unversioned DOI (e.g., https://doi.org/10.3886/ICPSR06425) is typically preferred over the versioned form ( e.g., https://doi.org/10.3886/ICPSR06425**.v1**), as the unversioned form (also referred to as "v0") will always resolve to the latest version of a study. A versioned DOI *should* be used, however, if the goal is to highlight a unique feature in the metadata for a specific version (which may change in future versions). 

**Versioning:** Any update with a change to the version number must come with a corresponding addition to the "Changes to the Collection" element.

The standard ICPSR Version Statement consists of the designation ICPSR (uppercase) plus the full 5-digit study number (including any leading zeros), a dash followed by a lowercase "v", and the version number.

The Version element is used as the source of the version identifier for the Citation element. Each version also receives a unique DOI (unversioned DOIs redirect to the current version). 

**Authority Control and VIAF:** In general, the following hierarchy of resources should be used when checking potential values for elements subject to name "authority control" (e.g.,  PI Names, PI Affiliations, Distributors, and Funding Agencies):

1. The ICPSR Personal Name Authority List or ICPSR Organization Name Authority List.
2. Previous ICPSR studies if the personal/organizational name is not in an ICPSR Authority List.
3. The [Virtual International Authority File](https://viaf.org) (VIAF)
4. Information from an official source, such as a personal CV on an institutional website, or the "About" page on an organization’s website.

We should always try to maintain consistency within our own catalog first, and then check external sources for the correct usage of a personal or organizational name.

VIAF is an effort to link the various national authority files (that is, catalogs of authoritative names such as the [Library of Congress Name Authority File](https://id.loc.gov/authorities/names.html)) into a single international collective. Once the record for the entity is found, those inputting metadata should click on the link next to the American flag (which will lead to the Library of Congress entry), and use the name in the 100 field (for personal names) or 110 field (for organizational names) of the MARC record displayed. If there are only foreign catalog entries, use of those are acceptable. 

If a name is not available in either our catalog or VIAF, use your best judgment to verify it with a different source. Most PI’s have pages with their home institution that can be used to seek past publications for use of a middle initial. Organizations typically have an About page, that uses the full name of the organization.

**Tense:** Use past tense when describing the process of collecting the data.  Use present tense when necessary, such as when you are describing the data: "The MIDUS Refresher collection is split into two datasets."

**Numbers:** Always use numerals versus spelling numbers out. Spelling out the number can sometimes be used for emphasis, but in that case, the number should also be used in parenthesis--for example, "Two thousand (2,000)".

**Sampling vs. Universe:**
- **Example 1**
  - **Sampling:** The data collection is a pooled cross-sectional time-series of bank robberies in 50 states over a period of 6 years (1970-1975), resulting in 300 observations.  
  - **Universe:** Bank robberies in the 50 states.
- **Example 2**
  - **Sampling:** Three target groups were identified: lawyers 36 years of age and above who were members of the American Bar Association (ABA), all the remaining members of the ABA excluding law students, and all lawyers in the nonmember files kept by the ABA. A systematic random probability sample was drawn to represent each of the three groups. The group of young lawyers was oversampled. 
  - **Universe:** Lawyers in the United States in 1984. 