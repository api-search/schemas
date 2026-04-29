---
description: A data element is a variable that points to a piece of data within your application, such as query strings, URLs, cookie values, JavaScript variables, or DOM elements. Data elements are used within rules to provide dynamic values and serve as the data dictionary for tag management.
layout: schema
name: Adobe Experience Platform Tags Data Element
properties_list:
- description: The unique identifier for the data element.
  name: id
  type: string
- description: The resource type identifier.
  name: type
  type: string
- description: ''
  name: attributes
  type: object
- description: Related resources linked to this data element.
  name: relationships
  type: object
- description: ''
  name: links
  type: object
provider_name: Adobe Launch
provider_slug: adobe-launch
schema_file: json-schema/data-element.json
slug: data-element
source_filename: data-element.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://github.com/kinlane/adobe-launch/json-schema/data-element.json\",\n  \"title\": \"Adobe Experience Platform Tags Data Element\",\n  \"description\": \"A data element is a variable that points to a piece of data within your application, such as query strings, URLs, cookie values, JavaScript variables, or DOM elements. Data elements are used within rules to provide dynamic values and serve as the data dictionary for tag management.\",\n  \"type\": \"object\",\n  \"required\": [\n    \"id\",\n    \"type\",\n    \"attributes\"\n  ],\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"The unique identifier for the data element.\",\n      \"examples\": [\n        \"DE1234567890abcdef\"\n      ]\n    },\n    \"type\": {\n      \"type\": \"string\",\n      \"const\": \"data_elements\",\n      \"description\": \"The resource type identifier.\"\n    },\n   \
  \ \"attributes\": {\n      \"type\": \"object\",\n      \"required\": [\n        \"name\",\n        \"delegate_descriptor_id\"\n      ],\n      \"properties\": {\n        \"name\": {\n          \"type\": \"string\",\n          \"description\": \"The human-readable name of the data element. Used to reference it in rules with %name% syntax.\",\n          \"minLength\": 1,\n          \"examples\": [\n            \"Page Name\",\n            \"User ID\",\n            \"Cart Total\"\n          ]\n        },\n        \"delegate_descriptor_id\": {\n          \"type\": \"string\",\n          \"description\": \"The descriptor ID that identifies which data element type from an extension package provides this data element's behavior.\",\n          \"pattern\": \"^[a-zA-Z0-9_-]+::[a-zA-Z0-9_-]+::[a-zA-Z0-9_-]+$\",\n          \"examples\": [\n            \"core::dataElements::javascript-variable\",\n            \"core::dataElements::dom-attribute\",\n            \"core::dataElements::cookie\"\n    \
  \      ]\n        },\n        \"default_value\": {\n          \"type\": \"string\",\n          \"description\": \"The default value returned when the data element resolves to no value.\",\n          \"examples\": [\n            \"unknown\",\n            \"0\",\n            \"\"\n          ]\n        },\n        \"settings\": {\n          \"type\": \"string\",\n          \"description\": \"A JSON-encoded string of settings specific to the data element type. The structure depends on the delegate_descriptor_id.\",\n          \"examples\": [\n            \"{\\\"path\\\":\\\"window.digitalData.page.pageName\\\"}\",\n            \"{\\\"elementSelector\\\":\\\"#main-title\\\",\\\"elementProperty\\\":\\\"textContent\\\"}\"\n          ]\n        },\n        \"storage_duration\": {\n          \"type\": \"string\",\n          \"enum\": [\n            \"pageview\",\n            \"session\",\n            \"visitor\"\n          ],\n          \"default\": \"pageview\",\n          \"description\": \"\
  How long the data element value persists. Pageview clears on navigation, session clears when the browser closes, visitor persists across sessions.\"\n        },\n        \"force_lower_case\": {\n          \"type\": \"boolean\",\n          \"default\": false,\n          \"description\": \"Whether to force the resolved value to lowercase.\"\n        },\n        \"clean_text\": {\n          \"type\": \"boolean\",\n          \"default\": false,\n          \"description\": \"Whether to remove leading and trailing whitespace from the resolved value.\"\n        },\n        \"enabled\": {\n          \"type\": \"boolean\",\n          \"default\": true,\n          \"description\": \"Whether the data element is enabled.\"\n        },\n        \"published\": {\n          \"type\": \"boolean\",\n          \"description\": \"Whether the data element has been published.\",\n          \"readOnly\": true\n        },\n        \"dirty\": {\n          \"type\": \"boolean\",\n          \"description\": \"\
  Whether the data element has unpublished changes.\",\n          \"readOnly\": true\n        },\n        \"revision_number\": {\n          \"type\": \"integer\",\n          \"minimum\": 0,\n          \"description\": \"The current revision number.\",\n          \"readOnly\": true\n        },\n        \"created_at\": {\n          \"type\": \"string\",\n          \"format\": \"date-time\",\n          \"description\": \"When the data element was created.\",\n          \"readOnly\": true\n        },\n        \"updated_at\": {\n          \"type\": \"string\",\n          \"format\": \"date-time\",\n          \"description\": \"When the data element was last updated.\",\n          \"readOnly\": true\n        }\n      }\n    },\n    \"relationships\": {\n      \"type\": \"object\",\n      \"description\": \"Related resources linked to this data element.\",\n      \"properties\": {\n        \"property\": {\n          \"$ref\": \"#/$defs/relationship\",\n          \"description\": \"The property\
  \ that owns this data element.\"\n        },\n        \"extension\": {\n          \"$ref\": \"#/$defs/relationship\",\n          \"description\": \"The extension that provides this data element type.\"\n        },\n        \"libraries\": {\n          \"$ref\": \"#/$defs/relationship\",\n          \"description\": \"Libraries that include this data element.\"\n        },\n        \"revisions\": {\n          \"$ref\": \"#/$defs/relationship\",\n          \"description\": \"Previous revisions of this data element.\"\n        },\n        \"origin\": {\n          \"$ref\": \"#/$defs/relationship\",\n          \"description\": \"The previous revision from which this data element was derived.\"\n        },\n        \"notes\": {\n          \"$ref\": \"#/$defs/relationship\",\n          \"description\": \"Notes associated with this data element.\"\n        }\n      }\n    },\n    \"links\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"self\": {\n          \"type\": \"string\"\
  ,\n          \"format\": \"uri\",\n          \"description\": \"The canonical URL for this data element resource.\"\n        }\n      }\n    }\n  },\n  \"$defs\": {\n    \"relationship\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"data\": {\n          \"oneOf\": [\n            {\n              \"type\": \"object\",\n              \"properties\": {\n                \"id\": {\n                  \"type\": \"string\"\n                },\n                \"type\": {\n                  \"type\": \"string\"\n                }\n              }\n            },\n            {\n              \"type\": \"array\",\n              \"items\": {\n                \"type\": \"object\",\n                \"properties\": {\n                  \"id\": {\n                    \"type\": \"string\"\n                  },\n                  \"type\": {\n                    \"type\": \"string\"\n                  }\n                }\n              }\n            }\n          ]\n        },\n\
  \        \"links\": {\n          \"type\": \"object\",\n          \"properties\": {\n            \"related\": {\n              \"type\": \"string\",\n              \"format\": \"uri\"\n            }\n          }\n        }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adobe-launch/refs/heads/main/json-schema/data-element.json
tags:
- Data Collection
- Edge Network
- Event Forwarding
- Marketing Technology
- Tag Management
title: Adobe Experience Platform Tags Data Element
---
