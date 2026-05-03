---
description: Holds a set of reusable objects for different aspects of the OAS. All objects defined within the Components Object have no effect on the API unless they are explicitly referenced from outside the Components Object.
layout: schema
name: OpenAPI Components Object
properties_list:
- description: An object to hold reusable Schema Objects.
  name: schemas
  type: object
- description: An object to hold reusable Response Objects.
  name: responses
  type: object
- description: An object to hold reusable Parameter Objects.
  name: parameters
  type: object
- description: An object to hold reusable Example Objects.
  name: examples
  type: object
- description: An object to hold reusable Request Body Objects.
  name: requestBodies
  type: object
- description: An object to hold reusable Header Objects.
  name: headers
  type: object
- description: An object to hold reusable Security Scheme Objects.
  name: securitySchemes
  type: object
- description: An object to hold reusable Link Objects.
  name: links
  type: object
- description: An object to hold reusable Callback Objects.
  name: callbacks
  type: object
- description: An object to hold reusable Path Item Objects.
  name: pathItems
  type: object
provider_name: OpenAPI
provider_slug: openapi
schema_file: json-schema/openapi-components.json
slug: openapi-components
source_filename: openapi-components.json
source_heading: JSON Schema
source_json: "{\n  \"$id\": \"openapi-components.json\",\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"OpenAPI Components Object\",\n  \"description\": \"Holds a set of reusable objects for different aspects of the OAS. All objects defined within the Components Object have no effect on the API unless they are explicitly referenced from outside the Components Object.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"schemas\": {\n      \"type\": \"object\",\n      \"description\": \"An object to hold reusable Schema Objects.\",\n      \"additionalProperties\": {}\n    },\n    \"responses\": {\n      \"type\": \"object\",\n      \"description\": \"An object to hold reusable Response Objects.\",\n      \"additionalProperties\": {\n        \"$ref\": \"openapi-response.json\"\n      }\n    },\n    \"parameters\": {\n      \"type\": \"object\",\n      \"description\": \"An object to hold reusable Parameter Objects.\",\n      \"additionalProperties\": {\n\
  \        \"$ref\": \"openapi-parameter.json\"\n      }\n    },\n    \"examples\": {\n      \"type\": \"object\",\n      \"description\": \"An object to hold reusable Example Objects.\",\n      \"additionalProperties\": {\n        \"$ref\": \"openapi-example.json\"\n      }\n    },\n    \"requestBodies\": {\n      \"type\": \"object\",\n      \"description\": \"An object to hold reusable Request Body Objects.\",\n      \"additionalProperties\": {\n        \"$ref\": \"openapi-request-body.json\"\n      }\n    },\n    \"headers\": {\n      \"type\": \"object\",\n      \"description\": \"An object to hold reusable Header Objects.\",\n      \"additionalProperties\": {\n        \"$ref\": \"openapi-header.json\"\n      }\n    },\n    \"securitySchemes\": {\n      \"type\": \"object\",\n      \"description\": \"An object to hold reusable Security Scheme Objects.\",\n      \"additionalProperties\": {\n        \"$ref\": \"openapi-security-scheme.json\"\n      }\n    },\n    \"links\": {\n      \"\
  type\": \"object\",\n      \"description\": \"An object to hold reusable Link Objects.\",\n      \"additionalProperties\": {\n        \"$ref\": \"openapi-link.json\"\n      }\n    },\n    \"callbacks\": {\n      \"type\": \"object\",\n      \"description\": \"An object to hold reusable Callback Objects.\",\n      \"additionalProperties\": {\n        \"$ref\": \"openapi-path-item.json\"\n      }\n    },\n    \"pathItems\": {\n      \"type\": \"object\",\n      \"description\": \"An object to hold reusable Path Item Objects.\",\n      \"additionalProperties\": {\n        \"$ref\": \"openapi-path-item.json\"\n      }\n    }\n  },\n  \"patternProperties\": {\n    \"^x-\": {}\n  },\n  \"additionalProperties\": false\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/openapi/refs/heads/main/json-schema/openapi-components.json
tags:
- Documentation
- REST
- Specification
title: OpenAPI Components Object
---
