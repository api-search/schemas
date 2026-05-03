---
description: An application programming interface accessible over Web/Internet technologies, as defined by the Schema.org WebAPI type.
layout: schema
name: Schema.org WebAPI
properties_list:
- description: The Schema.org type.
  name: '@type'
  type: string
- description: The JSON-LD context URL.
  name: '@context'
  type: string
- description: The name of the API.
  name: name
  type: string
- description: A description of the API.
  name: description
  type: string
- description: URL of the API.
  name: url
  type: string
- description: Further documentation describing the Web API in more detail.
  name: documentation
  type: object
- description: Human-readable terms of service documentation.
  name: termsOfService
  type: string
- description: The service provider, service operator, or service performer.
  name: provider
  type: object
- description: A means of accessing the service.
  name: availableChannel
  type: object
- description: A category for the API.
  name: category
  type: string
- description: An offer to provide this API, including pricing and access information.
  name: offers
  type: object
- description: An intended audience for the API.
  name: audience
  type: object
provider_name: Schema.org
provider_slug: schema-org
schema_file: json-schema/schema-org-web-api-schema.json
slug: schema-org-web-api
source_filename: schema-org-web-api-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://schema.org/schemas/web-api.json\",\n  \"title\": \"Schema.org WebAPI\",\n  \"description\": \"An application programming interface accessible over Web/Internet technologies, as defined by the Schema.org WebAPI type.\",\n  \"type\": \"object\",\n  \"required\": [\"@type\", \"name\"],\n  \"properties\": {\n    \"@type\": {\n      \"type\": \"string\",\n      \"description\": \"The Schema.org type.\",\n      \"const\": \"WebAPI\"\n    },\n    \"@context\": {\n      \"type\": \"string\",\n      \"description\": \"The JSON-LD context URL.\",\n      \"default\": \"https://schema.org\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the API.\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"A description of the API.\"\n    },\n    \"url\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"description\"\
  : \"URL of the API.\"\n    },\n    \"documentation\": {\n      \"oneOf\": [\n        {\n          \"type\": \"string\",\n          \"format\": \"uri\"\n        },\n        {\n          \"$ref\": \"#/$defs/CreativeWork\"\n        }\n      ],\n      \"description\": \"Further documentation describing the Web API in more detail.\"\n    },\n    \"termsOfService\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"description\": \"Human-readable terms of service documentation.\"\n    },\n    \"provider\": {\n      \"oneOf\": [\n        {\n          \"$ref\": \"#/$defs/Organization\"\n        },\n        {\n          \"$ref\": \"#/$defs/Person\"\n        }\n      ],\n      \"description\": \"The service provider, service operator, or service performer.\"\n    },\n    \"availableChannel\": {\n      \"$ref\": \"#/$defs/ServiceChannel\",\n      \"description\": \"A means of accessing the service.\"\n    },\n    \"category\": {\n      \"type\": \"string\",\n      \"description\"\
  : \"A category for the API.\"\n    },\n    \"offers\": {\n      \"oneOf\": [\n        {\n          \"$ref\": \"#/$defs/Offer\"\n        },\n        {\n          \"type\": \"array\",\n          \"items\": {\n            \"$ref\": \"#/$defs/Offer\"\n          }\n        }\n      ],\n      \"description\": \"An offer to provide this API, including pricing and access information.\"\n    },\n    \"audience\": {\n      \"$ref\": \"#/$defs/Audience\",\n      \"description\": \"An intended audience for the API.\"\n    }\n  },\n  \"$defs\": {\n    \"CreativeWork\": {\n      \"type\": \"object\",\n      \"description\": \"The most generic kind of creative work.\",\n      \"properties\": {\n        \"@type\": {\n          \"type\": \"string\",\n          \"const\": \"CreativeWork\"\n        },\n        \"name\": {\n          \"type\": \"string\",\n          \"description\": \"The name of the documentation.\"\n        },\n        \"url\": {\n          \"type\": \"string\",\n          \"format\": \"\
  uri\",\n          \"description\": \"URL of the documentation.\"\n        },\n        \"encodingFormat\": {\n          \"type\": \"string\",\n          \"description\": \"Media type of the documentation (e.g., text/html, application/pdf).\"\n        }\n      }\n    },\n    \"Organization\": {\n      \"type\": \"object\",\n      \"description\": \"An organization such as a company, institution, or NGO.\",\n      \"properties\": {\n        \"@type\": {\n          \"type\": \"string\",\n          \"const\": \"Organization\"\n        },\n        \"name\": {\n          \"type\": \"string\",\n          \"description\": \"The name of the organization.\"\n        },\n        \"url\": {\n          \"type\": \"string\",\n          \"format\": \"uri\",\n          \"description\": \"URL of the organization.\"\n        }\n      }\n    },\n    \"Person\": {\n      \"type\": \"object\",\n      \"description\": \"A person.\",\n      \"properties\": {\n        \"@type\": {\n          \"type\": \"string\"\
  ,\n          \"const\": \"Person\"\n        },\n        \"name\": {\n          \"type\": \"string\",\n          \"description\": \"The name of the person.\"\n        }\n      }\n    },\n    \"ServiceChannel\": {\n      \"type\": \"object\",\n      \"description\": \"A means for accessing a service.\",\n      \"properties\": {\n        \"@type\": {\n          \"type\": \"string\",\n          \"const\": \"ServiceChannel\"\n        },\n        \"serviceUrl\": {\n          \"type\": \"string\",\n          \"format\": \"uri\",\n          \"description\": \"The website to access the service.\"\n        },\n        \"providesService\": {\n          \"type\": \"string\",\n          \"description\": \"The service provided by this channel.\"\n        }\n      }\n    },\n    \"Offer\": {\n      \"type\": \"object\",\n      \"description\": \"An offer to transfer some rights to an item or to provide a service.\",\n      \"properties\": {\n        \"@type\": {\n          \"type\": \"string\",\n   \
  \       \"const\": \"Offer\"\n        },\n        \"price\": {\n          \"type\": \"number\",\n          \"description\": \"The offer price.\"\n        },\n        \"priceCurrency\": {\n          \"type\": \"string\",\n          \"description\": \"The currency of the price (ISO 4217).\",\n          \"pattern\": \"^[A-Z]{3}$\"\n        },\n        \"description\": {\n          \"type\": \"string\",\n          \"description\": \"A description of the offer.\"\n        }\n      }\n    },\n    \"Audience\": {\n      \"type\": \"object\",\n      \"description\": \"The target group associated with a given audience.\",\n      \"properties\": {\n        \"@type\": {\n          \"type\": \"string\",\n          \"const\": \"Audience\"\n        },\n        \"audienceType\": {\n          \"type\": \"string\",\n          \"description\": \"The target group associated with a given audience.\"\n        }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/schema-org/refs/heads/main/json-schema/schema-org-web-api-schema.json
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
title: Schema.org WebAPI
---
