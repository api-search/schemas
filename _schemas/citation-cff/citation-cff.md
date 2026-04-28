---
description: A pragmatic JSON Schema profile of the Citation File Format 1.2.0 capturing the most commonly used fields. The authoritative schema is published at https://github.com/citation-file-format/citation-file-format.
layout: schema
name: Citation File Format (CFF) - Subset Profile
properties_list:
- description: The version of the CFF schema this file complies with.
  name: cff-version
  type: string
- description: Human-readable message instructing how to cite the software.
  name: message
  type: string
- description: The name of the software or dataset being cited.
  name: title
  type: string
- description: The released version being cited.
  name: version
  type: string
- description: DOI of the software or dataset.
  name: doi
  type: string
- description: ISO 8601 date the version was released.
  name: date-released
  type: string
- description: SPDX license identifier.
  name: license
  type: string
- description: URL of the source code repository.
  name: repository-code
  type: string
- description: URL of the software project.
  name: url
  type: string
- description: Short description of the software.
  name: abstract
  type: string
- description: Keywords describing the software.
  name: keywords
  type: array
- description: ''
  name: authors
  type: array
- description: ''
  name: preferred-citation
  type: object
- description: ''
  name: references
  type: array
- description: ''
  name: identifiers
  type: array
- description: ''
  name: type
  type: string
provider_name: Citation File Format
provider_slug: citation-cff
schema_file: json-schema/citation-cff-schema.json
slug: citation-cff
tags:
- Academic
- Citation
- Metadata
- Open Standard
- Repository
- Research
- Software
- YAML
title: Citation File Format (CFF) - Subset Profile
---
