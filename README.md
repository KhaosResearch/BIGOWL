# BIGOWL: An ontology to support knowledge management in Big Data analytics

[![Explore ontology](https://img.shields.io/badge/explore-WebVOWL-orange.svg?style=flat-square)](www.visualdataweb.de/webvowl/#iri=https://raw.githubusercontent.com/KhaosResearch/BIGOWL/master/BIGOWL.owl)

### ✨ Ontology 

BIGOWL.owl an ontology-driven approach to support knowledge management in Big Data analytics workflows. BIGOWL is designed to cover a wide vocabulary of terms concerning Big Data analytics workflows, including their components and how they are connected, from data sources to the analytics visualization. It also takes into consideration aspects such as parameters, restrictions and formats. This ontology defines not only the taxonomic relationships between the different concepts, but also instances representing specific individuals to guide the users in the design of Big Data analytics workflows.

[BIGOWL.owl](BIGOWL.owl) was developed using Protégé 5.5.0 (beta 5 SNAPSHOT).

#### Summary of features
BIGOWL.owl contains the following features:
1.	A semantic approach to represent and consolidate BIG DATA workflows is proposed.
2.	An OWL Ontology and SWRL rules are developed for reasoning tasks in BIG DATA.
3.	The proposal is validated with real-world knowledge workflows base of BIG DATA.

### 📖 Documentation

Documentation was generated with pyLODE 2.8.3:

```bash
pylode -i bigowl.owl -o ./docs/index.html
```

 ### New version
 BIGOWL has been updated to follow the FAIR principles. Now it has been split into  4 ontologies:
- **BIGOWLData**. This ontology contains all the classes and properties related to data. _Data_ is devoted to annotating all the data flowing throughout the analytic workflow. It is declared as _EquivalentTo IO-Class_ of DMOP. This aligning enables datatypes defined by third parties’ ontologies to be contextualised in the analysis.  BIGOWLData contains the main data properties defined for this class, namely: _path_, to annotate the origin of data; and _hasDataType_, which establishes the relationship with class _DataType_. This last is used to define the data type, i.e. _PrimitiveType_ (Double, Integer, Boolean, etc.) or _StructuredType_ (Graph, Tree, Matrix, Vector, Tuple, etc.).
 - **BIGOWLProblems**. It is used to represent the problem class and its properties. Problem is oriented to the specific problem domain (Smart Cities, Biology, etc.).
 - **BIGOWLAlgorithms**. This ontology covers all possible kinds. It has two main subclasses: _DataMiningAlgorithm_ and _OptimizationAlgorithm_, which are used to distinguish between these two families of algorithms. The former is included in the form of equivalence with the class _DM-Algorithm_, which is linked from DMOP
 - **BIGOWLWorkflows**. It is used to guide the correct orchestration of a workflow, including elements like tasks, components, parameters, etc. This ontology imports BIGOWLData and BIGOWLAlgorithms to define all the pieces in a workflow.

Those new versions are available on: https://github.com/ProyectoAether/BIGOWL

<p align="center">&mdash; ⭐️ &mdash;</p>
<p align="center"><i>Designed & built by Khaos Research (University of Málaga).</i></p>
