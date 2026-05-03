---
description: A chemical compound record from the RSC ChemSpider database
layout: schema
name: ChemSpider Compound
properties_list:
- description: ChemSpider record ID (CSID)
  name: id
  type: integer
- description: SMILES representation of the compound structure
  name: smiles
  type: string
- description: Molecular formula (e.g., C6H12O6)
  name: formula
  type: string
- description: Average molecular mass in g/mol
  name: averageMass
  type: number
- description: Molecular weight in g/mol
  name: molecularWeight
  type: number
- description: Monoisotopic mass in g/mol
  name: monoisotopicMass
  type: number
- description: Nominal mass (integer) in g/mol
  name: nominalMass
  type: integer
- description: Common or IUPAC name of the compound
  name: commonName
  type: string
- description: Total number of references in ChemSpider
  name: referenceCount
  type: integer
- description: Number of external data sources containing this compound
  name: dataSourceCount
  type: integer
- description: Number of PubMed articles referencing this compound
  name: pubmedCount
  type: integer
- description: Number of RSC publications referencing this compound
  name: rscCount
  type: integer
- description: 2D MOL file representation of the compound
  name: mol2D
  type: string
- description: 3D MOL file representation of the compound
  name: mol3D
  type: string
provider_name: RSC
provider_slug: rsc
schema_file: json-schema/rsc-compound-schema.json
slug: rsc-compound
source_filename: rsc-compound-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://api.rsc.org/schemas/compound\",\n  \"title\": \"ChemSpider Compound\",\n  \"description\": \"A chemical compound record from the RSC ChemSpider database\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"integer\",\n      \"description\": \"ChemSpider record ID (CSID)\"\n    },\n    \"smiles\": {\n      \"type\": \"string\",\n      \"description\": \"SMILES representation of the compound structure\"\n    },\n    \"formula\": {\n      \"type\": \"string\",\n      \"description\": \"Molecular formula (e.g., C6H12O6)\"\n    },\n    \"averageMass\": {\n      \"type\": \"number\",\n      \"description\": \"Average molecular mass in g/mol\"\n    },\n    \"molecularWeight\": {\n      \"type\": \"number\",\n      \"description\": \"Molecular weight in g/mol\"\n    },\n    \"monoisotopicMass\": {\n      \"type\": \"number\",\n      \"description\": \"Monoisotopic\
  \ mass in g/mol\"\n    },\n    \"nominalMass\": {\n      \"type\": \"integer\",\n      \"description\": \"Nominal mass (integer) in g/mol\"\n    },\n    \"commonName\": {\n      \"type\": \"string\",\n      \"description\": \"Common or IUPAC name of the compound\"\n    },\n    \"referenceCount\": {\n      \"type\": \"integer\",\n      \"description\": \"Total number of references in ChemSpider\",\n      \"minimum\": 0\n    },\n    \"dataSourceCount\": {\n      \"type\": \"integer\",\n      \"description\": \"Number of external data sources containing this compound\",\n      \"minimum\": 0\n    },\n    \"pubmedCount\": {\n      \"type\": \"integer\",\n      \"description\": \"Number of PubMed articles referencing this compound\",\n      \"minimum\": 0\n    },\n    \"rscCount\": {\n      \"type\": \"integer\",\n      \"description\": \"Number of RSC publications referencing this compound\",\n      \"minimum\": 0\n    },\n    \"mol2D\": {\n      \"type\": \"string\",\n      \"description\"\
  : \"2D MOL file representation of the compound\"\n    },\n    \"mol3D\": {\n      \"type\": \"string\",\n      \"description\": \"3D MOL file representation of the compound\"\n    }\n  },\n  \"required\": [\"id\", \"formula\"]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/rsc/refs/heads/main/json-schema/rsc-compound-schema.json
tags:
- Chemistry
- Cheminformatics
- Chemical Data
- Science
title: ChemSpider Compound
---
