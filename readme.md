# Zeri Foundation data sample

The repository contains two directories including respectively 100 XML files, describing photographs and artworks depicted in photographs, and 100 RDF/XML files, i.e., the output of the convesion of former XML files according to CIDOC-CRM and other few ontologies - see [Ontologies](#ontologies) section.

N.B. Data will be slightly modified soon, so as to be compliant with [aac mapping rules](https://aac-mappings.herokuapp.com).

# The RDF Dataset
The RDF dataset published by the Zeri Foundation is available at the [Zeri & LODE project](w3id.org/zericatalog/) web page. Here you'll find several data access points - like a SPARQL endpoint wherein directly [query](data.fondazionezeri.unibo.it/query) the triplestore, or a [RDF Browser](https://w3id.org/zericatalog/collection/zeri-photo-archive) to browse links in a user-friendly way. A dump can be downloaded from [AMSActa](http://amsacta.unibo.it/5157/) institutional repository.

# Ontologies
Data are mainly converted to RDF/XML according to CIDOC-CRM. Few relations and classes belong to other ontologies, since CIDOC-CRM doesn't provide a comprehensive description of topics that are relevant to understand Zeri's data. Indeed, the aim is to integrate CIDOC-CRM.

All terms belonging to ontologies but CIDOC-CRM, have been imported in two specular ones for the sake of clarity, namely:
	- [F Entry Ontology](http://www.essepuntato.it/2014/03/fentry), for describing specific issues related to the photography domain;
	- [OA Entry Ontology](http://purl.org/emmedi/oaentry), for describing specific issues related to the artwork domain;

Imported ontologies and used as modular, task ontologies, i.e., they are used to cover specific topics, namely:
	- [HiCO Ontology](http://purl.org/emmedi/hico), an extension of the [PROV-O Ontology](https://www.w3.org/TR/prov-o/) for describing sources, motivations and methodology used by cataloguers to support a questionable information (e.g. an authorship attribution);
	- [SPAR Ontologies](http://purl.org/spar/), a suite of modular ontologies for describing the publishing domain, including:
		- [FaBiO](http://purl.org/spar/fabio) an FRBR-aligned model for describing bibliography and archival documents;
		- [CiTO](http://purl.org/spar/cito) for characterizing bibliographic citations;
		- [PRO](http://purl.org/spar/pro) for defining an agent's role in a time-indexed situation;

# Mapping cataloguing rules to RDF
Zeri catalog entries conform two national content standards, called respectively [Scheda F](http://www.iccd.beniculturali.it/index.php?it/473/standard-catalografici/Standard/10) - photography - and [Scheda OA](http://www.iccd.beniculturali.it/index.php?it/473/standard-catalografici/Standard/29) - artwork. 

Two mapping documents have been realized to explain the alignments from content standard fields to CIDOC-CRM and aforementioned ontologies, i.e., [FtoRDF](https://dx.doi.org/10.6084/m9.figshare.3175273.v1) and [OAtoRDF](https://dx.doi.org/10.6084/m9.figshare.3175057.v1).

An graphical overview of the two mappings can be found in "mapping" directory.

# Main publication (forthcoming)
Marilena Daquino, Francesca Mambelli, Silvio Peroni, Francesca Tomasi, Fabio Vitali. 2016. Enhancing semantic expressivity in the cultural heritage domain: exposing the Zeri Photo Archive as Linked Open Data. arXiv.org. [arXiv:1605.01188](https://arxiv.org/abs/1605.01188)