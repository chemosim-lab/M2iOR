# Contributing Guide - Sharing Experimental Data (M2iOR)

Welcome to the **M2iOR** GitHub repository! We sincerely thank you for your contribution and your willingness to share your experimental data with the scientific community.

This guide outlines the procedure for submitting your olfaction and olfactory receptor (OR) data to be integrated into our database.

---

## 📋 Table of Contents
1. [Prerequisites & Template Files](#1-prerequisites--template-files)
2. [Data Structure & Description](#2-data-structure--description)
3. [Filling Instructions](#3-filling-instructions)
4. [Email Submission Procedure](#4-email-submission-procedure)
5. [Validation & Integration Process](#5-validation--integration-process)

---

## 1. Prerequisites & Template Files

To submit your data, please use one of the template files provided in this repository:
* **Excel Format (`.xlsx`)**: `M2iOR_Experiment_Table_Empty.xlsx` (recommended; contains description sheets and the input table).
* **CSV Format (`.csv`)**: `M2iOR_Experiment_Table_Empty_semicolon.csv` (semicolon-delimited `;`).

You can also refer to the file [M2iOR_Description_Fields.md](https://github.com/chemosim-lab/M2iOR/blob/main/templates/M2iOR_Description_Fields.md) to view the complete list of expected metadata, their definitions, and whether they are mandatory.

---

## 2. Data Structure & Description

The data table contains **41 columns** organized into several key thematic categories:

### A. Receptor and Co-Receptor Information
* **Species**: Taxon name of the species from which the OR originates.
* **Receptor Name**: Gene name of the given OR/Orco.
* **Accession** (Mandatory `*`): Identifier in the UniProtKB or GenBank database.
* **Mutation**: Mutation realized by authors on protein sequence.
* **Sequence** (Mandatory `*`): Protein sequence of the given OR.
* *The corresponding `.1` columns are dedicated to the Co-receptor (e.g., Orco).*

### B. Molecule / Ligand
* **Molecule Name**: Name of the molecule as reported in the source (standardized via PubChem).
* **CID** (Mandatory `*`): Compound Identifier from PubChem.
* **CAS**: CAS Registry Number.
* **InChIKey**: International Chemistry Identifier Key from PubChem (standardized identifier).
* **SMILES**: Simplified Molecular-Input Line-Entry System representation.
* **Mixture**: Indicates whether it is a mixture.

### C. Experimental Results & Parameters
* **Responsive**: Indicates whether the receptor responds to the ligand (Yes/No).
* **Parameter** (Mandatory `*`): Type of parameter measured (e.g., primary, secondary, dose-response).
* **Value** & **Unit** (Mandatory `*`): Numerical value measured and its unit.
* **Value Nature**: Specification on the nature of the value (e.g., mean, single value).
* **Concentration** & **Concentration Unit** (Mandatory `*`): Concentration of the tested substance.
* **Nbr. Measurement**: Number of replicated measurements.

### D. Protocol & Expression System
* **Experimental technique** (Mandatory `*`): Experimental technique used (e.g., *Xenopus* oocytes, HEK293, calcium imaging, electrophysiology).
* **Recording system** / **Type** / **Expression System** / **Expression Cell Type** / **Expression Driver** / **Co-Transfection**.
* **Odor delivery system** / **Stimulation Flux** / **Main Flux** / **Stimulation Duration** (with respective units).

### E. Bibliographic Reference
* **Reference**: Authors and title of the source publication.
* **DOI** (Mandatory `*`): Digital Object Identifier of the article.
* **Reference Position**: Figure, table, or section number corresponding in the article.

---

## 3. Filling Instructions

1. **Fill out the table** row by row for each experiment or receptor/molecule combination.
2. Strictly respect cell formats, especially for mandatory identifiers (`*`) such as the **UniProt Accession**, **Protein Sequence**, and **PubChem CID**.
3. Use the semicolon (`;`) as a separator if you are working with the CSV file.
4. Do not modify the header row (column names) of the template file, as it is used for automated database importing.

---

## 4. Email Submission Procedure

Once your file is completed and verified:

1. Rename your file following this naming convention:  
   `M2iOR_Submission_[YourLastName]_[YYYYMMDD].[xlsx or csv]`
2. Draft an email addressed to the curation team:
   * **Email Address**: `contact_at_chemsensim.fr` (replace _\_at\__ by _@_)
   * **Email Subject**: `[M2iOR Data Submission] - Author_Name - Article_DOI`
   * **Email Body**: Please briefly state the title of your associated paper, the DOI, and any helpful contextual information.
3. **Attach your completed file** (`.xlsx` or `.csv`) to the email.

---

## 5. Validation & Integration Process

* **Acknowledgment**: You will receive an acknowledgment of receipt within 48-72 business hours max.
* **Curation & Quality Control**: Our team will validate data consistency (PubChem CID matching, UniProt sequence validity, parameter formats). If any anomalies are found, we will contact you via email to adjust the file. Scientific content will never be modified without consulting the contributor.
* **Integration**: Once validated, your data will be integrated into the next M2iOR release version, and you will be credited as a source contributor.

---

## 6. Data ownership

Contributors retain the authorship of their published work.

By submitting the completed template, contributors confirm that:

- the submitted data originate from a published article or that they have the right to share them;
- M2iOR may curate, standardize and redistribute the submitted metadata as part of the database;
- the original publication will always be cited through its DOI and bibliographic reference.

Thank you for contributing to open science and the structuring of olfaction data!
