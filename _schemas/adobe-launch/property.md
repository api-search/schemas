---
description: A property in Adobe Experience Platform Tags is a container that holds most tag management resources. A property belongs to exactly one company and can have many rules, data elements, extensions, environments, and libraries. Properties are scoped to a specific platform (web, mobile, or edge).
layout: schema
name: Adobe Experience Platform Tags Property
properties_list:
- description: The unique identifier for the property.
  name: id
  type: string
- description: The resource type identifier.
  name: type
  type: string
- description: ''
  name: attributes
  type: object
- description: Related resources linked to this property.
  name: relationships
  type: object
- description: ''
  name: links
  type: object
provider_name: Adobe Launch
provider_slug: adobe-launch
schema_file: json-schema/property.json
slug: property
source_filename: property.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://github.com/kinlane/adobe-launch/json-schema/property.json\",\n  \"title\": \"Adobe Experience Platform Tags Property\",\n  \"description\": \"A property in Adobe Experience Platform Tags is a container that holds most tag management resources. A property belongs to exactly one company and can have many rules, data elements, extensions, environments, and libraries. Properties are scoped to a specific platform (web, mobile, or edge).\",\n  \"type\": \"object\",\n  \"required\": [\n    \"id\",\n    \"type\",\n    \"attributes\"\n  ],\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"The unique identifier for the property.\",\n      \"examples\": [\n        \"PR1234567890abcdef\"\n      ]\n    },\n    \"type\": {\n      \"type\": \"string\",\n      \"const\": \"properties\",\n      \"description\": \"The resource type identifier.\"\n    },\n    \"attributes\"\
  : {\n      \"type\": \"object\",\n      \"required\": [\n        \"name\",\n        \"platform\"\n      ],\n      \"properties\": {\n        \"name\": {\n          \"type\": \"string\",\n          \"description\": \"The human-readable name of the property.\",\n          \"minLength\": 1,\n          \"examples\": [\n            \"My Website Property\"\n          ]\n        },\n        \"platform\": {\n          \"type\": \"string\",\n          \"enum\": [\n            \"web\",\n            \"mobile\",\n            \"edge\"\n          ],\n          \"description\": \"The platform type. Web properties manage browser-side tags, mobile properties manage mobile app tags, and edge properties manage server-side event forwarding.\"\n        },\n        \"domains\": {\n          \"type\": \"array\",\n          \"items\": {\n            \"type\": \"string\",\n            \"format\": \"hostname\"\n          },\n          \"description\": \"A list of domains associated with the property.\",\n     \
  \     \"examples\": [\n            [\"example.com\", \"www.example.com\"]\n          ]\n        },\n        \"enabled\": {\n          \"type\": \"boolean\",\n          \"default\": true,\n          \"description\": \"Whether the property is enabled.\"\n        },\n        \"development\": {\n          \"type\": \"boolean\",\n          \"default\": false,\n          \"description\": \"Whether the property is in development mode.\"\n        },\n        \"privacy\": {\n          \"type\": \"string\",\n          \"enum\": [\n            \"optin\",\n            \"optout\"\n          ],\n          \"description\": \"The default privacy setting for the property.\"\n        },\n        \"ssl_enabled\": {\n          \"type\": \"boolean\",\n          \"default\": true,\n          \"description\": \"Whether SSL is enabled for tag delivery.\"\n        },\n        \"rule_component_sequencing_enabled\": {\n          \"type\": \"boolean\",\n          \"default\": false,\n          \"description\": \"\
  Whether rule component sequencing is enabled, allowing ordered execution of rule components.\"\n        },\n        \"undefined_vars_return_empty\": {\n          \"type\": \"boolean\",\n          \"default\": false,\n          \"description\": \"Whether undefined data element variables return empty strings instead of undefined.\"\n        },\n        \"token\": {\n          \"type\": \"string\",\n          \"description\": \"A unique token for the property.\",\n          \"readOnly\": true\n        },\n        \"created_at\": {\n          \"type\": \"string\",\n          \"format\": \"date-time\",\n          \"description\": \"When the property was created.\",\n          \"readOnly\": true\n        },\n        \"updated_at\": {\n          \"type\": \"string\",\n          \"format\": \"date-time\",\n          \"description\": \"When the property was last updated.\",\n          \"readOnly\": true\n        }\n      }\n    },\n    \"relationships\": {\n      \"type\": \"object\",\n      \"\
  description\": \"Related resources linked to this property.\",\n      \"properties\": {\n        \"company\": {\n          \"$ref\": \"#/$defs/relationship\",\n          \"description\": \"The company that owns this property.\"\n        },\n        \"callbacks\": {\n          \"$ref\": \"#/$defs/relationship\",\n          \"description\": \"Webhook callbacks configured for this property.\"\n        },\n        \"data_elements\": {\n          \"$ref\": \"#/$defs/relationship\",\n          \"description\": \"Data elements belonging to this property.\"\n        },\n        \"environments\": {\n          \"$ref\": \"#/$defs/relationship\",\n          \"description\": \"Deployment environments for this property.\"\n        },\n        \"extensions\": {\n          \"$ref\": \"#/$defs/relationship\",\n          \"description\": \"Extensions installed in this property.\"\n        },\n        \"hosts\": {\n          \"$ref\": \"#/$defs/relationship\",\n          \"description\": \"Hosting destinations\
  \ for this property.\"\n        },\n        \"libraries\": {\n          \"$ref\": \"#/$defs/relationship\",\n          \"description\": \"Libraries belonging to this property.\"\n        },\n        \"rules\": {\n          \"$ref\": \"#/$defs/relationship\",\n          \"description\": \"Rules defined in this property.\"\n        }\n      }\n    },\n    \"links\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"self\": {\n          \"type\": \"string\",\n          \"format\": \"uri\",\n          \"description\": \"The canonical URL for this property resource.\"\n        }\n      }\n    }\n  },\n  \"$defs\": {\n    \"relationship\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"data\": {\n          \"oneOf\": [\n            {\n              \"type\": \"object\",\n              \"properties\": {\n                \"id\": {\n                  \"type\": \"string\"\n                },\n                \"type\": {\n                  \"type\": \"string\"\
  \n                }\n              }\n            },\n            {\n              \"type\": \"array\",\n              \"items\": {\n                \"type\": \"object\",\n                \"properties\": {\n                  \"id\": {\n                    \"type\": \"string\"\n                  },\n                  \"type\": {\n                    \"type\": \"string\"\n                  }\n                }\n              }\n            }\n          ]\n        },\n        \"links\": {\n          \"type\": \"object\",\n          \"properties\": {\n            \"related\": {\n              \"type\": \"string\",\n              \"format\": \"uri\"\n            }\n          }\n        }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adobe-launch/refs/heads/main/json-schema/property.json
tags:
- Data Collection
- Edge Network
- Event Forwarding
- Marketing Technology
- Tag Management
title: Adobe Experience Platform Tags Property
---
