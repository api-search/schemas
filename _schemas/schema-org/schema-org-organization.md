---
description: An organization such as a school, NGO, corporation, club, etc.
layout: schema
name: Schema.org Organization
properties_list:
- description: The Schema.org type.
  name: '@type'
  type: string
- description: The JSON-LD context URL.
  name: '@context'
  type: string
- description: The name of the organization.
  name: name
  type: string
- description: The official name of the organization.
  name: legalName
  type: string
- description: A description of the organization.
  name: description
  type: string
- description: URL of the organization.
  name: url
  type: string
- description: An associated logo.
  name: logo
  type: object
- description: An image of the organization.
  name: image
  type: object
- description: Email address.
  name: email
  type: string
- description: The telephone number.
  name: telephone
  type: string
- description: The fax number.
  name: faxNumber
  type: string
- description: Physical address of the organization.
  name: address
  type: object
- description: A contact point for the organization.
  name: contactPoint
  type: object
- description: A person who founded this organization.
  name: founder
  type: object
- description: The date that this organization was founded.
  name: foundingDate
  type: string
- description: The place where the organization was founded.
  name: foundingLocation
  type: object
- description: The date that this organization was dissolved.
  name: dissolutionDate
  type: string
- description: The number of employees in an organization.
  name: numberOfEmployees
  type: object
- description: A member of an Organization or a ProgramMembership.
  name: member
  type: object
- description: The larger organization that this organization is a subOrganization of.
  name: parentOrganization
  type: object
- description: A relationship between two organizations where the first includes the second.
  name: subOrganization
  type: object
- description: A department within the organization.
  name: department
  type: object
- description: The geographic area where a service or offered item is provided.
  name: areaServed
  type: string
- description: The brand(s) associated with the organization.
  name: brand
  type: object
- description: The Tax / Fiscal ID of the organization.
  name: taxID
  type: string
- description: The Value-Added Tax ID of the organization.
  name: vatID
  type: string
- description: The Dun & Bradstreet DUNS number.
  name: duns
  type: string
- description: The North American Industry Classification System (NAICS) code.
  name: naics
  type: string
- description: The International Standard of Industrial Classification of All Economic Activities (ISIC) code.
  name: isicV4
  type: string
- description: URL of a reference Web page that unambiguously indicates the item's identity.
  name: sameAs
  type: object
- description: The identifier property represents any kind of identifier.
  name: identifier
  type: string
- description: An award won by or for this organization.
  name: award
  type: object
- description: Of a Person, and less typically of an Organization, to indicate a topic that is known about.
  name: knowsAbout
  type: object
provider_name: Schema.org
provider_slug: schema-org
schema_file: json-schema/schema-org-organization-schema.json
slug: schema-org-organization
source_filename: schema-org-organization-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://schema.org/schemas/organization.json\",\n  \"title\": \"Schema.org Organization\",\n  \"description\": \"An organization such as a school, NGO, corporation, club, etc.\",\n  \"type\": \"object\",\n  \"required\": [\"@type\", \"name\"],\n  \"properties\": {\n    \"@type\": {\n      \"type\": \"string\",\n      \"description\": \"The Schema.org type.\",\n      \"enum\": [\"Organization\", \"Corporation\", \"EducationalOrganization\", \"GovernmentOrganization\", \"MedicalOrganization\", \"NGO\", \"PerformingGroup\", \"SportsOrganization\"]\n    },\n    \"@context\": {\n      \"type\": \"string\",\n      \"description\": \"The JSON-LD context URL.\",\n      \"default\": \"https://schema.org\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the organization.\"\n    },\n    \"legalName\": {\n      \"type\": \"string\",\n      \"description\": \"The\
  \ official name of the organization.\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"A description of the organization.\"\n    },\n    \"url\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"description\": \"URL of the organization.\"\n    },\n    \"logo\": {\n      \"oneOf\": [\n        { \"type\": \"string\", \"format\": \"uri\" },\n        { \"$ref\": \"schema-org-image-object-schema.json\" }\n      ],\n      \"description\": \"An associated logo.\"\n    },\n    \"image\": {\n      \"oneOf\": [\n        { \"type\": \"string\", \"format\": \"uri\" },\n        { \"$ref\": \"schema-org-image-object-schema.json\" }\n      ],\n      \"description\": \"An image of the organization.\"\n    },\n    \"email\": {\n      \"type\": \"string\",\n      \"format\": \"email\",\n      \"description\": \"Email address.\"\n    },\n    \"telephone\": {\n      \"type\": \"string\",\n      \"description\": \"The telephone number.\"\n    },\n \
  \   \"faxNumber\": {\n      \"type\": \"string\",\n      \"description\": \"The fax number.\"\n    },\n    \"address\": {\n      \"oneOf\": [\n        { \"type\": \"string\" },\n        { \"$ref\": \"schema-org-postal-address-schema.json\" }\n      ],\n      \"description\": \"Physical address of the organization.\"\n    },\n    \"contactPoint\": {\n      \"oneOf\": [\n        { \"$ref\": \"schema-org-contact-point-schema.json\" },\n        { \"type\": \"array\", \"items\": { \"$ref\": \"schema-org-contact-point-schema.json\" } }\n      ],\n      \"description\": \"A contact point for the organization.\"\n    },\n    \"founder\": {\n      \"oneOf\": [\n        { \"$ref\": \"schema-org-person-schema.json\" },\n        { \"type\": \"array\", \"items\": { \"$ref\": \"schema-org-person-schema.json\" } }\n      ],\n      \"description\": \"A person who founded this organization.\"\n    },\n    \"foundingDate\": {\n      \"type\": \"string\",\n      \"format\": \"date\",\n      \"description\"\
  : \"The date that this organization was founded.\"\n    },\n    \"foundingLocation\": {\n      \"$ref\": \"schema-org-place-schema.json\",\n      \"description\": \"The place where the organization was founded.\"\n    },\n    \"dissolutionDate\": {\n      \"type\": \"string\",\n      \"format\": \"date\",\n      \"description\": \"The date that this organization was dissolved.\"\n    },\n    \"numberOfEmployees\": {\n      \"type\": \"object\",\n      \"description\": \"The number of employees in an organization.\",\n      \"properties\": {\n        \"@type\": { \"type\": \"string\", \"const\": \"QuantitativeValue\" },\n        \"value\": { \"type\": \"integer\", \"description\": \"The value.\" },\n        \"minValue\": { \"type\": \"integer\", \"description\": \"The lower value of some characteristic.\" },\n        \"maxValue\": { \"type\": \"integer\", \"description\": \"The upper value of some characteristic.\" }\n      }\n    },\n    \"member\": {\n      \"oneOf\": [\n        { \"\
  $ref\": \"schema-org-person-schema.json\" },\n        { \"$ref\": \"#\" },\n        { \"type\": \"array\", \"items\": { \"oneOf\": [{ \"$ref\": \"schema-org-person-schema.json\" }, { \"$ref\": \"#\" }] } }\n      ],\n      \"description\": \"A member of an Organization or a ProgramMembership.\"\n    },\n    \"parentOrganization\": {\n      \"$ref\": \"#\",\n      \"description\": \"The larger organization that this organization is a subOrganization of.\"\n    },\n    \"subOrganization\": {\n      \"oneOf\": [\n        { \"$ref\": \"#\" },\n        { \"type\": \"array\", \"items\": { \"$ref\": \"#\" } }\n      ],\n      \"description\": \"A relationship between two organizations where the first includes the second.\"\n    },\n    \"department\": {\n      \"oneOf\": [\n        { \"$ref\": \"#\" },\n        { \"type\": \"array\", \"items\": { \"$ref\": \"#\" } }\n      ],\n      \"description\": \"A department within the organization.\"\n    },\n    \"areaServed\": {\n      \"type\": \"string\"\
  ,\n      \"description\": \"The geographic area where a service or offered item is provided.\"\n    },\n    \"brand\": {\n      \"type\": \"object\",\n      \"description\": \"The brand(s) associated with the organization.\",\n      \"properties\": {\n        \"@type\": { \"type\": \"string\", \"enum\": [\"Brand\", \"Organization\"] },\n        \"name\": { \"type\": \"string\", \"description\": \"The name of the brand.\" },\n        \"logo\": { \"type\": \"string\", \"format\": \"uri\", \"description\": \"URL of the brand logo.\" }\n      }\n    },\n    \"taxID\": {\n      \"type\": \"string\",\n      \"description\": \"The Tax / Fiscal ID of the organization.\"\n    },\n    \"vatID\": {\n      \"type\": \"string\",\n      \"description\": \"The Value-Added Tax ID of the organization.\"\n    },\n    \"duns\": {\n      \"type\": \"string\",\n      \"description\": \"The Dun & Bradstreet DUNS number.\"\n    },\n    \"naics\": {\n      \"type\": \"string\",\n      \"description\": \"The North\
  \ American Industry Classification System (NAICS) code.\"\n    },\n    \"isicV4\": {\n      \"type\": \"string\",\n      \"description\": \"The International Standard of Industrial Classification of All Economic Activities (ISIC) code.\"\n    },\n    \"sameAs\": {\n      \"oneOf\": [\n        { \"type\": \"string\", \"format\": \"uri\" },\n        { \"type\": \"array\", \"items\": { \"type\": \"string\", \"format\": \"uri\" } }\n      ],\n      \"description\": \"URL of a reference Web page that unambiguously indicates the item's identity.\"\n    },\n    \"identifier\": {\n      \"type\": \"string\",\n      \"description\": \"The identifier property represents any kind of identifier.\"\n    },\n    \"award\": {\n      \"oneOf\": [\n        { \"type\": \"string\" },\n        { \"type\": \"array\", \"items\": { \"type\": \"string\" } }\n      ],\n      \"description\": \"An award won by or for this organization.\"\n    },\n    \"knowsAbout\": {\n      \"oneOf\": [\n        { \"type\": \"\
  string\" },\n        { \"type\": \"array\", \"items\": { \"type\": \"string\" } }\n      ],\n      \"description\": \"Of a Person, and less typically of an Organization, to indicate a topic that is known about.\"\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/schema-org/refs/heads/main/json-schema/schema-org-organization-schema.json
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
title: Schema.org Organization
---
