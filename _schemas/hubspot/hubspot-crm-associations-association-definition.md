---
description: Definition of an association type between two object types
layout: schema
name: AssociationDefinition
properties_list:
- description: Unique identifier for the association definition
  name: id
  type: string
- description: Source object type ID
  name: fromObjectTypeId
  type: string
- description: Target object type ID
  name: toObjectTypeId
  type: string
- description: Name of the association type
  name: name
  type: string
- description: Display label for the association
  name: label
  type: string
- description: Label for the inverse association
  name: inverseLabel
  type: string
- description: Category of the association definition
  name: category
  type: string
provider_name: HubSpot
provider_slug: hubspot
schema_file: json-schema/hubspot-crm-associations-association-definition-schema.json
slug: hubspot-crm-associations-association-definition
source_filename: hubspot-crm-associations-association-definition-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"description\": \"Definition of an association type between two object types\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier for the association definition\",\n      \"example\": \"500123\"\n    },\n    \"fromObjectTypeId\": {\n      \"type\": \"string\",\n      \"description\": \"Source object type ID\",\n      \"example\": \"500123\"\n    },\n    \"toObjectTypeId\": {\n      \"type\": \"string\",\n      \"description\": \"Target object type ID\",\n      \"example\": \"500123\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Name of the association type\",\n      \"example\": \"Example Record\"\n    },\n    \"label\": {\n      \"type\": \"string\",\n      \"description\": \"Display label for the association\",\n      \"example\": \"Example Record\"\n    },\n    \"inverseLabel\": {\n      \"type\": \"string\",\n      \"description\": \"Label for the\
  \ inverse association\",\n      \"example\": \"Example Record\"\n    },\n    \"category\": {\n      \"type\": \"string\",\n      \"description\": \"Category of the association definition\",\n      \"example\": \"HUBSPOT_DEFINED\",\n      \"enum\": [\n        \"HUBSPOT_DEFINED\",\n        \"USER_DEFINED\",\n        \"INTEGRATOR_DEFINED\"\n      ]\n    }\n  },\n  \"required\": [\n    \"id\",\n    \"fromObjectTypeId\",\n    \"toObjectTypeId\"\n  ],\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"AssociationDefinition\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/hubspot/refs/heads/main/json-schema/hubspot-crm-associations-association-definition-schema.json
tags:
- Analytics
- Commerce
- Content
- CRM
- Customer Service
- Email Marketing
- Marketing
- Marketing Automation
- Operations
- Sales
title: AssociationDefinition
---
