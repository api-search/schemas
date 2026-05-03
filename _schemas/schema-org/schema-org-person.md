---
description: A person (alive, dead, undead, or fictional). Extends Thing with properties specific to individuals.
layout: schema
name: Schema.org Person
properties_list:
- description: The Schema.org type.
  name: '@type'
  type: string
- description: The JSON-LD context URL.
  name: '@context'
  type: string
- description: The name of the person.
  name: name
  type: string
- description: Given name (first name).
  name: givenName
  type: string
- description: Family name (last name).
  name: familyName
  type: string
- description: An additional name for a Person, can be used for a middle name.
  name: additionalName
  type: string
- description: An honorific prefix preceding a Person's name such as Dr/Mrs/Mr.
  name: honorificPrefix
  type: string
- description: An honorific suffix following a Person's name such as M.D./PhD/MSCSW.
  name: honorificSuffix
  type: string
- description: Email address.
  name: email
  type: string
- description: The telephone number.
  name: telephone
  type: string
- description: URL of the person's page.
  name: url
  type: string
- description: An image of the person.
  name: image
  type: object
- description: A description of the person.
  name: description
  type: string
- description: The job title of the person.
  name: jobTitle
  type: string
- description: Organizations that the person works for.
  name: worksFor
  type: object
- description: An organization that this person is affiliated with.
  name: affiliation
  type: object
- description: An organization that the person is an alumni of.
  name: alumniOf
  type: object
- description: Date of birth.
  name: birthDate
  type: string
- description: Date of death.
  name: deathDate
  type: string
- description: The place where the person was born.
  name: birthPlace
  type: object
- description: Gender of the person.
  name: gender
  type: string
- description: Nationality of the person.
  name: nationality
  type: string
- description: Physical address of the person.
  name: address
  type: object
- description: A contact point for a person.
  name: contactPoint
  type: object
- description: A colleague of the person.
  name: colleague
  type: object
- description: The most generic bi-directional social/work relation.
  name: knows
  type: object
- description: The most generic uni-directional social relation.
  name: follows
  type: object
- description: URL of a reference Web page that unambiguously indicates the item's identity.
  name: sameAs
  type: object
- description: The identifier property represents any kind of identifier.
  name: identifier
  type: string
- description: An award won by or for this person.
  name: award
  type: object
- description: The Person's occupation.
  name: hasOccupation
  type: object
provider_name: Schema.org
provider_slug: schema-org
schema_file: json-schema/schema-org-person-schema.json
slug: schema-org-person
source_filename: schema-org-person-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://schema.org/schemas/person.json\",\n  \"title\": \"Schema.org Person\",\n  \"description\": \"A person (alive, dead, undead, or fictional). Extends Thing with properties specific to individuals.\",\n  \"type\": \"object\",\n  \"required\": [\"@type\", \"name\"],\n  \"properties\": {\n    \"@type\": {\n      \"type\": \"string\",\n      \"const\": \"Person\",\n      \"description\": \"The Schema.org type.\"\n    },\n    \"@context\": {\n      \"type\": \"string\",\n      \"description\": \"The JSON-LD context URL.\",\n      \"default\": \"https://schema.org\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the person.\"\n    },\n    \"givenName\": {\n      \"type\": \"string\",\n      \"description\": \"Given name (first name).\"\n    },\n    \"familyName\": {\n      \"type\": \"string\",\n      \"description\": \"Family name (last name).\"\n \
  \   },\n    \"additionalName\": {\n      \"type\": \"string\",\n      \"description\": \"An additional name for a Person, can be used for a middle name.\"\n    },\n    \"honorificPrefix\": {\n      \"type\": \"string\",\n      \"description\": \"An honorific prefix preceding a Person's name such as Dr/Mrs/Mr.\"\n    },\n    \"honorificSuffix\": {\n      \"type\": \"string\",\n      \"description\": \"An honorific suffix following a Person's name such as M.D./PhD/MSCSW.\"\n    },\n    \"email\": {\n      \"type\": \"string\",\n      \"format\": \"email\",\n      \"description\": \"Email address.\"\n    },\n    \"telephone\": {\n      \"type\": \"string\",\n      \"description\": \"The telephone number.\"\n    },\n    \"url\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"description\": \"URL of the person's page.\"\n    },\n    \"image\": {\n      \"oneOf\": [\n        { \"type\": \"string\", \"format\": \"uri\" },\n        { \"$ref\": \"schema-org-image-object-schema.json\"\
  \ }\n      ],\n      \"description\": \"An image of the person.\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"A description of the person.\"\n    },\n    \"jobTitle\": {\n      \"type\": \"string\",\n      \"description\": \"The job title of the person.\"\n    },\n    \"worksFor\": {\n      \"$ref\": \"schema-org-organization-schema.json\",\n      \"description\": \"Organizations that the person works for.\"\n    },\n    \"affiliation\": {\n      \"$ref\": \"schema-org-organization-schema.json\",\n      \"description\": \"An organization that this person is affiliated with.\"\n    },\n    \"alumniOf\": {\n      \"oneOf\": [\n        { \"$ref\": \"schema-org-organization-schema.json\" },\n        { \"type\": \"array\", \"items\": { \"$ref\": \"schema-org-organization-schema.json\" } }\n      ],\n      \"description\": \"An organization that the person is an alumni of.\"\n    },\n    \"birthDate\": {\n      \"type\": \"string\",\n      \"format\"\
  : \"date\",\n      \"description\": \"Date of birth.\"\n    },\n    \"deathDate\": {\n      \"type\": \"string\",\n      \"format\": \"date\",\n      \"description\": \"Date of death.\"\n    },\n    \"birthPlace\": {\n      \"$ref\": \"schema-org-place-schema.json\",\n      \"description\": \"The place where the person was born.\"\n    },\n    \"gender\": {\n      \"type\": \"string\",\n      \"description\": \"Gender of the person.\"\n    },\n    \"nationality\": {\n      \"type\": \"string\",\n      \"description\": \"Nationality of the person.\"\n    },\n    \"address\": {\n      \"oneOf\": [\n        { \"type\": \"string\" },\n        { \"$ref\": \"schema-org-postal-address-schema.json\" }\n      ],\n      \"description\": \"Physical address of the person.\"\n    },\n    \"contactPoint\": {\n      \"oneOf\": [\n        { \"$ref\": \"schema-org-contact-point-schema.json\" },\n        { \"type\": \"array\", \"items\": { \"$ref\": \"schema-org-contact-point-schema.json\" } }\n      ],\n\
  \      \"description\": \"A contact point for a person.\"\n    },\n    \"colleague\": {\n      \"oneOf\": [\n        { \"type\": \"string\", \"format\": \"uri\" },\n        { \"type\": \"array\", \"items\": { \"type\": \"string\", \"format\": \"uri\" } }\n      ],\n      \"description\": \"A colleague of the person.\"\n    },\n    \"knows\": {\n      \"oneOf\": [\n        { \"$ref\": \"#\" },\n        { \"type\": \"array\", \"items\": { \"$ref\": \"#\" } }\n      ],\n      \"description\": \"The most generic bi-directional social/work relation.\"\n    },\n    \"follows\": {\n      \"oneOf\": [\n        { \"$ref\": \"#\" },\n        { \"type\": \"array\", \"items\": { \"$ref\": \"#\" } }\n      ],\n      \"description\": \"The most generic uni-directional social relation.\"\n    },\n    \"sameAs\": {\n      \"oneOf\": [\n        { \"type\": \"string\", \"format\": \"uri\" },\n        { \"type\": \"array\", \"items\": { \"type\": \"string\", \"format\": \"uri\" } }\n      ],\n      \"description\"\
  : \"URL of a reference Web page that unambiguously indicates the item's identity.\"\n    },\n    \"identifier\": {\n      \"type\": \"string\",\n      \"description\": \"The identifier property represents any kind of identifier.\"\n    },\n    \"award\": {\n      \"oneOf\": [\n        { \"type\": \"string\" },\n        { \"type\": \"array\", \"items\": { \"type\": \"string\" } }\n      ],\n      \"description\": \"An award won by or for this person.\"\n    },\n    \"hasOccupation\": {\n      \"type\": \"object\",\n      \"description\": \"The Person's occupation.\",\n      \"properties\": {\n        \"@type\": { \"type\": \"string\", \"const\": \"Occupation\" },\n        \"name\": { \"type\": \"string\", \"description\": \"The name of the occupation.\" },\n        \"occupationalCategory\": { \"type\": \"string\", \"description\": \"A category describing the job.\" }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/schema-org/refs/heads/main/json-schema/schema-org-person-schema.json
tags:
- Schema.org
- Structured Data
- Linked Data
- JSON-LD
- Vocabulary
- SEO
- Web Standards
- RDF
- Ontology
title: Schema.org Person
---
