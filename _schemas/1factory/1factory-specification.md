---
description: Specification that defines feature to be measured.
layout: schema
name: Specification
properties_list:
- description: Balloon number for feature.
  name: bln_no
  type: string
- description: Sheet and zone of the specification
  name: sheet_zone
  type: string
- description: Place number - for features that have multiple places, feature specification is repeated for each place.
  name: place
  type: integer
- description: Characteristic being measured, or, in the case of a note, the text of the note.
  name: characteristic
  type: string
- description: Type of characteristic being measured.
  name: characteristic_type
  type: string
- description: Dimension type for this specification - Standard, Manufacturing or Deviation.
  name: dimension_type
  type: string
- description: Balloon number of specification that this feature references, for example a manufacturing dimension referencing the actual drawing dimension it corresponds to.
  name: referenced_feature
  type: string
- description: How the data for this specification is recorded - numerically, as a pass/fail, or calculated from other features.
  name: data_type
  type: string
- description: Nominal value for this specification.
  name: nominal
  type: number
- description: Lower specification limit for the feature.
  name: lower_spec_limit
  type: number
- description: Upper specification limit for the feature.
  name: upper_spec_limit
  type: number
- description: Unit of measure for this feature.
  name: unit
  type: string
- description: Descriptor of feature. For GD&T, this is used to record the datum.
  name: descriptor_datum
  type: string
- description: For GD&T features, defines the material condition for evaluating bonus tolerance, if applicable.
  name: bonus_tolerance
  type: string
- description: Optional label to add more information to the specification.
  name: label
  type: string
- description: How the feature should be inspected.
  name: inspection_method
  type: string
- description: How frequently should the feature be checked.
  name: sampling_rule
  type: string
- description: Manufacturing operation for the feature.
  name: operation
  type: string
- description: Indicates if feature is key for quality.
  name: is_key
  type: boolean
provider_name: 1Factory
provider_slug: 1factory
schema_file: json-schema/1factory-specification-schema.json
slug: 1factory-specification
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/1factory/refs/heads/main/json-schema/1factory-specification-schema.json\",\n  \"title\": \"Specification\",\n  \"description\": \"Specification that defines feature to be measured.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"bln_no\": {\n      \"type\": \"string\",\n      \"nullable\": false,\n      \"description\": \"Balloon number for feature.\",\n      \"example\": \"1\"\n    },\n    \"sheet_zone\": {\n      \"type\": \"string\",\n      \"nullable\": false,\n      \"description\": \"Sheet and zone of the specification\",\n      \"example\": \"1 : B1\"\n    },\n    \"place\": {\n      \"type\": \"integer\",\n      \"minimum\": 1,\n      \"description\": \"Place number - for features that have multiple places, feature specification is repeated for each place.\",\n      \"example\": 1\n    },\n    \"characteristic\": {\n      \"type\"\
  : \"string\",\n      \"nullable\": false,\n      \"description\": \"Characteristic being measured, or, in the case of a note, the text of the note.\",\n      \"example\": \"True position\"\n    },\n    \"characteristic_type\": {\n      \"type\": \"string\",\n      \"nullable\": false,\n      \"enum\": [\n        \"Nom \\u00b1 Tol\",\n        \"GD&T\",\n        \"Basic\",\n        \"Min - Max\",\n        \"Note\",\n        \"Nom++Tol\",\n        \"Nom -- Tol\",\n        \"Reference\"\n      ],\n      \"description\": \"Type of characteristic being measured.\",\n      \"example\": \"GD&T\"\n    },\n    \"dimension_type\": {\n      \"type\": \"string\",\n      \"nullable\": false,\n      \"enum\": [\n        \"STD\",\n        \"MFG\",\n        \"DVN\"\n      ],\n      \"description\": \"Dimension type for this specification - Standard, Manufacturing or Deviation.\",\n      \"example\": \"STD\"\n    },\n    \"referenced_feature\": {\n      \"type\": \"string\",\n      \"nullable\": true,\n\
  \      \"description\": \"Balloon number of specification that this feature references, for example a manufacturing dimension referencing the actual drawing dimension it corresponds to.\",\n      \"example\": \"1\"\n    },\n    \"data_type\": {\n      \"type\": \"string\",\n      \"nullable\": false,\n      \"enum\": [\n        \"NUM\",\n        \"P/F\",\n        \"CALC\"\n      ],\n      \"description\": \"How the data for this specification is recorded - numerically, as a pass/fail, or calculated from other features.\",\n      \"example\": \"NUM\"\n    },\n    \"nominal\": {\n      \"type\": \"number\",\n      \"nullable\": true,\n      \"description\": \"Nominal value for this specification.\",\n      \"example\": 1.12\n    },\n    \"lower_spec_limit\": {\n      \"type\": \"number\",\n      \"nullable\": true,\n      \"description\": \"Lower specification limit for the feature.\",\n      \"example\": 1.11\n    },\n    \"upper_spec_limit\": {\n      \"type\": \"number\",\n      \"nullable\"\
  : true,\n      \"description\": \"Upper specification limit for the feature.\",\n      \"example\": 1.14\n    },\n    \"unit\": {\n      \"type\": \"string\",\n      \"nullable\": true,\n      \"description\": \"Unit of measure for this feature.\",\n      \"example\": \"mm\"\n    },\n    \"descriptor_datum\": {\n      \"type\": \"string\",\n      \"nullable\": true,\n      \"description\": \"Descriptor of feature. For GD&T, this is used to record the datum.\",\n      \"example\": \"A\"\n    },\n    \"bonus_tolerance\": {\n      \"type\": \"string\",\n      \"nullable\": true,\n      \"enum\": [\n        \"MMC\",\n        \"LMC\"\n      ],\n      \"description\": \"For GD&T features, defines the material condition for evaluating bonus tolerance, if applicable.\",\n      \"example\": \"MMC\"\n    },\n    \"label\": {\n      \"type\": \"string\",\n      \"nullable\": true,\n      \"description\": \"Optional label to add more information to the specification.\",\n      \"example\": \"COUNTERSINK\"\
  \n    },\n    \"inspection_method\": {\n      \"type\": \"string\",\n      \"nullable\": true,\n      \"description\": \"How the feature should be inspected.\",\n      \"example\": \"CMM\"\n    },\n    \"sampling_rule\": {\n      \"type\": \"string\",\n      \"nullable\": true,\n      \"description\": \"How frequently should the feature be checked.\",\n      \"example\": \"1 in 10\"\n    },\n    \"operation\": {\n      \"type\": \"string\",\n      \"nullable\": true,\n      \"description\": \"Manufacturing operation for the feature.\",\n      \"example\": \"OP10\"\n    },\n    \"is_key\": {\n      \"type\": \"boolean\",\n      \"nullable\": false,\n      \"description\": \"Indicates if feature is key for quality.\",\n      \"example\": true\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/1factory/refs/heads/main/json-schema/1factory-specification-schema.json
tags:
- Analytics
- Data Collection
- Manufacturing
- Monitoring
- Quality
title: Specification
---
