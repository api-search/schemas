---
description: Represents a business glossary term in the Microsoft Purview Data Map. Glossary terms provide standardized business vocabulary for data governance.
layout: schema
name: Microsoft Purview Glossary Term
properties_list:
- description: The globally unique identifier of the glossary term
  name: guid
  type: string
- description: The fully qualified name of the glossary term
  name: qualifiedName
  type: string
- description: The display name of the glossary term
  name: name
  type: string
- description: A brief description of the term
  name: shortDescription
  type: string
- description: A detailed description of the term
  name: longDescription
  type: string
- description: The abbreviation of the term
  name: abbreviation
  type: string
- description: Usage guidance for the term
  name: usage
  type: string
- description: The approval status of the term
  name: status
  type: string
- description: Reference to the parent glossary
  name: anchor
  type: object
- description: Categories the term belongs to
  name: categories
  type: array
- description: Classifications applied to the term
  name: classifications
  type: array
- description: Entities assigned to this term
  name: assignedEntities
  type: array
- description: Related glossary terms
  name: seeAlso
  type: array
- description: Synonym terms
  name: synonyms
  type: array
- description: Antonym terms
  name: antonyms
  type: array
- description: External resources related to the term
  name: resources
  type: array
- description: Contact information for the term
  name: contacts
  type: object
provider_name: Microsoft Purview
provider_slug: microsoft-purview
schema_file: json-schema/microsoft-purview-glossary-term-schema.json
slug: microsoft-purview-glossary-term
source_filename: microsoft-purview-glossary-term-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://github.com/api-search/microsoft-purview/json-schema/microsoft-purview-glossary-term-schema.json\",\n  \"title\": \"Microsoft Purview Glossary Term\",\n  \"description\": \"Represents a business glossary term in the Microsoft Purview Data Map. Glossary terms provide standardized business vocabulary for data governance.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"guid\": {\n      \"type\": \"string\",\n      \"format\": \"uuid\",\n      \"description\": \"The globally unique identifier of the glossary term\"\n    },\n    \"qualifiedName\": {\n      \"type\": \"string\",\n      \"description\": \"The fully qualified name of the glossary term\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The display name of the glossary term\"\n    },\n    \"shortDescription\": {\n      \"type\": \"string\",\n      \"description\": \"A brief description of the\
  \ term\"\n    },\n    \"longDescription\": {\n      \"type\": \"string\",\n      \"description\": \"A detailed description of the term\"\n    },\n    \"abbreviation\": {\n      \"type\": \"string\",\n      \"description\": \"The abbreviation of the term\"\n    },\n    \"usage\": {\n      \"type\": \"string\",\n      \"description\": \"Usage guidance for the term\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"description\": \"The approval status of the term\",\n      \"enum\": [\"Draft\", \"Approved\", \"Alert\", \"Expired\"]\n    },\n    \"anchor\": {\n      \"type\": \"object\",\n      \"description\": \"Reference to the parent glossary\",\n      \"properties\": {\n        \"displayText\": {\n          \"type\": \"string\"\n        },\n        \"glossaryGuid\": {\n          \"type\": \"string\",\n          \"format\": \"uuid\"\n        },\n        \"relationGuid\": {\n          \"type\": \"string\",\n          \"format\": \"uuid\"\n        }\n      }\n    },\n    \"\
  categories\": {\n      \"type\": \"array\",\n      \"description\": \"Categories the term belongs to\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"categoryGuid\": {\n            \"type\": \"string\",\n            \"format\": \"uuid\"\n          },\n          \"description\": {\n            \"type\": \"string\"\n          },\n          \"displayText\": {\n            \"type\": \"string\"\n          },\n          \"relationGuid\": {\n            \"type\": \"string\",\n            \"format\": \"uuid\"\n          },\n          \"status\": {\n            \"type\": \"string\"\n          }\n        }\n      }\n    },\n    \"classifications\": {\n      \"type\": \"array\",\n      \"description\": \"Classifications applied to the term\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"typeName\": {\n            \"type\": \"string\"\n          },\n          \"attributes\": {\n            \"type\": \"object\"\
  ,\n            \"additionalProperties\": true\n          }\n        }\n      }\n    },\n    \"assignedEntities\": {\n      \"type\": \"array\",\n      \"description\": \"Entities assigned to this term\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"displayText\": {\n            \"type\": \"string\"\n          },\n          \"guid\": {\n            \"type\": \"string\",\n            \"format\": \"uuid\"\n          },\n          \"typeName\": {\n            \"type\": \"string\"\n          },\n          \"relationshipGuid\": {\n            \"type\": \"string\",\n            \"format\": \"uuid\"\n          },\n          \"relationshipStatus\": {\n            \"type\": \"string\",\n            \"enum\": [\"ACTIVE\", \"DELETED\"]\n          }\n        }\n      }\n    },\n    \"seeAlso\": {\n      \"type\": \"array\",\n      \"description\": \"Related glossary terms\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n\
  \          \"displayText\": {\n            \"type\": \"string\"\n          },\n          \"termGuid\": {\n            \"type\": \"string\",\n            \"format\": \"uuid\"\n          },\n          \"relationGuid\": {\n            \"type\": \"string\",\n            \"format\": \"uuid\"\n          }\n        }\n      }\n    },\n    \"synonyms\": {\n      \"type\": \"array\",\n      \"description\": \"Synonym terms\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"displayText\": {\n            \"type\": \"string\"\n          },\n          \"termGuid\": {\n            \"type\": \"string\",\n            \"format\": \"uuid\"\n          },\n          \"relationGuid\": {\n            \"type\": \"string\",\n            \"format\": \"uuid\"\n          }\n        }\n      }\n    },\n    \"antonyms\": {\n      \"type\": \"array\",\n      \"description\": \"Antonym terms\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n\
  \          \"displayText\": {\n            \"type\": \"string\"\n          },\n          \"termGuid\": {\n            \"type\": \"string\",\n            \"format\": \"uuid\"\n          },\n          \"relationGuid\": {\n            \"type\": \"string\",\n            \"format\": \"uuid\"\n          }\n        }\n      }\n    },\n    \"resources\": {\n      \"type\": \"array\",\n      \"description\": \"External resources related to the term\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"displayName\": {\n            \"type\": \"string\"\n          },\n          \"url\": {\n            \"type\": \"string\",\n            \"format\": \"uri\"\n          }\n        }\n      }\n    },\n    \"contacts\": {\n      \"type\": \"object\",\n      \"description\": \"Contact information for the term\",\n      \"properties\": {\n        \"expert\": {\n          \"type\": \"array\",\n          \"items\": {\n            \"type\": \"object\",\n            \"\
  properties\": {\n              \"id\": { \"type\": \"string\" },\n              \"info\": { \"type\": \"string\" }\n            }\n          }\n        },\n        \"steward\": {\n          \"type\": \"array\",\n          \"items\": {\n            \"type\": \"object\",\n            \"properties\": {\n              \"id\": { \"type\": \"string\" },\n              \"info\": { \"type\": \"string\" }\n            }\n          }\n        }\n      }\n    }\n  },\n  \"required\": [\"name\"]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/microsoft-purview/refs/heads/main/json-schema/microsoft-purview-glossary-term-schema.json
tags:
- Compliance
- Data Catalog
- Data Classification
- Data Governance
- Data Loss Prevention
- Information Protection
title: Microsoft Purview Glossary Term
---
