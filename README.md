# 🐝 M2iOR: Database of Insect Olfactory Receptors – Molecule Measurements

**Search and download the latest data: [m2ior.chemsensim.fr](https://m2ior.chemsensim.fr)**

### 🔬 Why M2iOR?

In insects, olfactory perception relies on interactions between odorant molecules and olfactory receptors (ORs) expressed in olfactory sensory neurons. 
But these data are scattered across the literature, with heterogeneous species, experimental systems, and reporting standards. Hard to analyze systematically.

**M2iOR centralizes and standardizes it all.**

It’s a curated, publicly accessible resource that currently compiles **30,000+ bioassay experiments** extracted from peer-reviewed publications and public databases.

### ✨ What’s inside

- **Ligand structures + receptor sequences**
- **Species annotations + mixture information**
- **Detailed experimental metadata**
- **Flexible query tools**: search by molecule, receptor, species, or assay system
- **Advanced filters + batch search** for high-throughput analysis
- **Visualization & export**: curated aggregation + binarized combinatorial representation ready for ML

> M2iOR = a comprehensive framework for data-driven research in insect olfaction and comparative chemosensory biology.

---

## 📊 Database Overview

M2iOR is organized into **5 data categories**:

### 🧬 **Receptor & Co-Receptor**
All about the tested receptor: species, OR/Orco gene name, Uniprot/Genbank ID, mutations if any, protein sequence.  
*The sequence = standard OR identifier.*

### 🧪 **Molecule**
Odorant description: name, PubChem CID, CAS, InChIKey, SMILES.  
Handles single compounds, isomer blends, and complex mixtures.  
*InChIKey = standard molecular identifier in M2iOR.*

### 📈 **Response**
The result: agonist yes/no, measurement type `primary` / `secondary` / `dose-response`, EC50 or raw value, unit, tested concentration, number of replicates.

### ⚙️ **Bioassay**
Full protocol: technique `SSR` / `voltage clamp`, expression system `Xenopus oocytes` / `Drosophila` /  `HEK293`, odor delivery system, flow rates, stimulation duration, co-transfection… 14 fields total.

### 📚 **Resources**
Full traceability: bibliographic reference, source DOI, precise location.

---

### 📄 License
Data is licensed under **CC BY 4.0**. Please cite M2iOR if you use it.

### 🤝 Contributing
Issues and pull requests are welcome! See `CONTRIBUTING.md`.
