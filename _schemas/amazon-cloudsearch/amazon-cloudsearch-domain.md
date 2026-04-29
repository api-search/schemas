---
description: Represents an Amazon CloudSearch domain with its configuration, index fields, and service endpoints.
layout: schema
name: Amazon CloudSearch Domain
properties_list:
- description: An internally generated unique identifier for a domain.
  name: domainId
  type: string
- description: A string that represents the name of a domain.
  name: domainName
  type: string
- description: The Amazon Resource Name (ARN) of the search domain.
  name: arn
  type: string
- description: True if the search domain is created.
  name: created
  type: boolean
- description: True if the search domain has been deleted.
  name: deleted
  type: boolean
- description: True if processing is being done to activate the current domain configuration.
  name: processing
  type: boolean
- description: True if IndexDocuments needs to be called to activate the current domain configuration.
  name: requiresIndexDocuments
  type: boolean
- description: The number of search instances that are available to process search requests.
  name: searchInstanceCount
  type: integer
- description: The instance type that is being used to process search requests.
  name: searchInstanceType
  type: string
- description: The service endpoint for updating documents in a search domain.
  name: docService
  type: object
- description: The service endpoint for requesting search results from a search domain.
  name: searchService
  type: object
provider_name: Amazon CloudSearch
provider_slug: amazon-cloudsearch
schema_file: json-schema/amazon-cloudsearch-domain-schema.json
slug: amazon-cloudsearch-domain
source_filename: amazon-cloudsearch-domain-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://api-evangelist.com/schemas/amazon/cloudsearch/domain.json\",\n  \"title\": \"Amazon CloudSearch Domain\",\n  \"description\": \"Represents an Amazon CloudSearch domain with its configuration, index fields, and service endpoints.\",\n  \"type\": \"object\",\n  \"required\": [\"domainName\"],\n  \"properties\": {\n    \"domainId\": {\n      \"type\": \"string\",\n      \"description\": \"An internally generated unique identifier for a domain.\"\n    },\n    \"domainName\": {\n      \"type\": \"string\",\n      \"description\": \"A string that represents the name of a domain.\",\n      \"minLength\": 3,\n      \"maxLength\": 28,\n      \"pattern\": \"^[a-z][a-z0-9-]+$\"\n    },\n    \"arn\": {\n      \"type\": \"string\",\n      \"description\": \"The Amazon Resource Name (ARN) of the search domain.\",\n      \"pattern\": \"^arn:aws:cloudsearch:[a-z0-9-]+:[0-9]{12}:domain/.+$\"\n    },\n\
  \    \"created\": {\n      \"type\": \"boolean\",\n      \"description\": \"True if the search domain is created.\"\n    },\n    \"deleted\": {\n      \"type\": \"boolean\",\n      \"description\": \"True if the search domain has been deleted.\"\n    },\n    \"processing\": {\n      \"type\": \"boolean\",\n      \"description\": \"True if processing is being done to activate the current domain configuration.\"\n    },\n    \"requiresIndexDocuments\": {\n      \"type\": \"boolean\",\n      \"description\": \"True if IndexDocuments needs to be called to activate the current domain configuration.\"\n    },\n    \"searchInstanceCount\": {\n      \"type\": \"integer\",\n      \"description\": \"The number of search instances that are available to process search requests.\"\n    },\n    \"searchInstanceType\": {\n      \"type\": \"string\",\n      \"description\": \"The instance type that is being used to process search requests.\"\n    },\n    \"docService\": {\n      \"type\": \"object\",\n\
  \      \"description\": \"The service endpoint for updating documents in a search domain.\",\n      \"properties\": {\n        \"endpoint\": {\n          \"type\": \"string\",\n          \"description\": \"The endpoint to which service requests can be submitted.\"\n        }\n      }\n    },\n    \"searchService\": {\n      \"type\": \"object\",\n      \"description\": \"The service endpoint for requesting search results from a search domain.\",\n      \"properties\": {\n        \"endpoint\": {\n          \"type\": \"string\",\n          \"description\": \"The endpoint to which service requests can be submitted.\"\n        }\n      }\n    }\n  },\n  \"additionalProperties\": false\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-cloudsearch/refs/heads/main/json-schema/amazon-cloudsearch-domain-schema.json
tags:
- AWS
- CloudSearch
- Search
- Full-Text Search
- Managed
title: Amazon CloudSearch Domain
---
