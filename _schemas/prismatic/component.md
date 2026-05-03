---
description: A component is a reusable unit of functionality (connector) that provides actions, triggers, and data sources for use in integrations.
layout: schema
name: Prismatic Component
properties_list:
- description: Unique identifier for the component
  name: id
  type: string
- description: Unique key used to reference the component
  name: key
  type: string
- description: Display label for the component
  name: label
  type: string
- description: Description of the component and its purpose
  name: description
  type: string
- description: Category the component belongs to
  name: category
  type: string
- description: Whether the component is publicly available or custom
  name: isPublic
  type: boolean
- description: Whether the component requires authorization credentials
  name: authorizationRequired
  type: boolean
- description: URL for the component icon
  name: iconUrl
  type: string
- description: Actions provided by the component
  name: actions
  type: array
- description: Triggers provided by the component
  name: triggers
  type: array
- description: Data sources provided by the component
  name: dataSources
  type: array
- description: Connection definitions for the component
  name: connections
  type: array
- description: Version number of the component
  name: versionNumber
  type: integer
- description: Timestamp when the component was created
  name: createdAt
  type: string
- description: Timestamp when the component was last updated
  name: updatedAt
  type: string
provider_name: Prismatic
provider_slug: prismatic
schema_file: json-schema/component.json
slug: component
source_filename: component.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/prismatic/refs/heads/main/json-schema/component.json\",\n  \"title\": \"Prismatic Component\",\n  \"description\": \"A component is a reusable unit of functionality (connector) that provides actions, triggers, and data sources for use in integrations.\",\n  \"type\": \"object\",\n  \"required\": [\"id\", \"key\", \"label\"],\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier for the component\"\n    },\n    \"key\": {\n      \"type\": \"string\",\n      \"description\": \"Unique key used to reference the component\"\n    },\n    \"label\": {\n      \"type\": \"string\",\n      \"description\": \"Display label for the component\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"Description of the component and its purpose\"\n    },\n    \"category\": {\n\
  \      \"type\": \"string\",\n      \"description\": \"Category the component belongs to\"\n    },\n    \"isPublic\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the component is publicly available or custom\"\n    },\n    \"authorizationRequired\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the component requires authorization credentials\"\n    },\n    \"iconUrl\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"description\": \"URL for the component icon\"\n    },\n    \"actions\": {\n      \"type\": \"array\",\n      \"description\": \"Actions provided by the component\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"id\": {\n            \"type\": \"string\"\n          },\n          \"key\": {\n            \"type\": \"string\"\n          },\n          \"label\": {\n            \"type\": \"string\"\n          },\n          \"description\": {\n            \"type\": \"string\"\
  \n          }\n        }\n      }\n    },\n    \"triggers\": {\n      \"type\": \"array\",\n      \"description\": \"Triggers provided by the component\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"id\": {\n            \"type\": \"string\"\n          },\n          \"key\": {\n            \"type\": \"string\"\n          },\n          \"label\": {\n            \"type\": \"string\"\n          },\n          \"description\": {\n            \"type\": \"string\"\n          }\n        }\n      }\n    },\n    \"dataSources\": {\n      \"type\": \"array\",\n      \"description\": \"Data sources provided by the component\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"id\": {\n            \"type\": \"string\"\n          },\n          \"key\": {\n            \"type\": \"string\"\n          },\n          \"label\": {\n            \"type\": \"string\"\n          },\n          \"description\": {\n          \
  \  \"type\": \"string\"\n          }\n        }\n      }\n    },\n    \"connections\": {\n      \"type\": \"array\",\n      \"description\": \"Connection definitions for the component\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"key\": {\n            \"type\": \"string\"\n          },\n          \"label\": {\n            \"type\": \"string\"\n          },\n          \"oauth2Type\": {\n            \"type\": \"string\",\n            \"enum\": [\"authorization_code\", \"client_credentials\"]\n          }\n        }\n      }\n    },\n    \"versionNumber\": {\n      \"type\": \"integer\",\n      \"description\": \"Version number of the component\"\n    },\n    \"createdAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Timestamp when the component was created\"\n    },\n    \"updatedAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Timestamp when the\
  \ component was last updated\"\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/prismatic/refs/heads/main/json-schema/component.json
tags:
- Embedded iPaaS
- Integrations
- Workflows
title: Prismatic Component
---
