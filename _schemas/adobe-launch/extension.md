---
description: An extension is an installed instance of an extension package within a property. Extensions provide additional capabilities to tags, including new data element types, rule component types (events, conditions, actions), and shared modules. Each extension is derived from an extension package and configured with property-specific settings.
layout: schema
name: Adobe Experience Platform Tags Extension
properties_list:
- description: The unique identifier for the extension.
  name: id
  type: string
- description: The resource type identifier.
  name: type
  type: string
- description: ''
  name: attributes
  type: object
- description: Related resources linked to this extension.
  name: relationships
  type: object
- description: ''
  name: links
  type: object
provider_name: Adobe Launch
provider_slug: adobe-launch
schema_file: json-schema/extension.json
slug: extension
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://github.com/kinlane/adobe-launch/json-schema/extension.json\",\n  \"title\": \"Adobe Experience Platform Tags Extension\",\n  \"description\": \"An extension is an installed instance of an extension package within a property. Extensions provide additional capabilities to tags, including new data element types, rule component types (events, conditions, actions), and shared modules. Each extension is derived from an extension package and configured with property-specific settings.\",\n  \"type\": \"object\",\n  \"required\": [\n    \"id\",\n    \"type\",\n    \"attributes\"\n  ],\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"The unique identifier for the extension.\",\n      \"examples\": [\n        \"EX1234567890abcdef\"\n      ]\n    },\n    \"type\": {\n      \"type\": \"string\",\n      \"const\": \"extensions\",\n      \"description\": \"\
  The resource type identifier.\"\n    },\n    \"attributes\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"name\": {\n          \"type\": \"string\",\n          \"description\": \"The unique name of the extension, matching the extension package name.\",\n          \"examples\": [\n            \"core\",\n            \"adobe-analytics\",\n            \"adobe-target\",\n            \"adobe-mcid\"\n          ]\n        },\n        \"display_name\": {\n          \"type\": \"string\",\n          \"description\": \"The human-readable display name shown in the UI.\",\n          \"examples\": [\n            \"Core\",\n            \"Adobe Analytics\",\n            \"Adobe Target\"\n          ]\n        },\n        \"version\": {\n          \"type\": \"string\",\n          \"description\": \"The version of the installed extension, following semantic versioning.\",\n          \"pattern\": \"^\\\\d+\\\\.\\\\d+\\\\.\\\\d+$\",\n          \"examples\": [\n            \"1.0.0\",\n\
  \            \"2.5.3\"\n          ]\n        },\n        \"delegate_descriptor_id\": {\n          \"type\": \"string\",\n          \"description\": \"The descriptor ID for the extension's configuration view.\",\n          \"examples\": [\n            \"adobe-analytics::extensionConfiguration::config\"\n          ]\n        },\n        \"settings\": {\n          \"type\": \"string\",\n          \"description\": \"A JSON-encoded string of configuration settings specific to this extension instance.\",\n          \"examples\": [\n            \"{\\\"trackingServer\\\":\\\"metrics.example.com\\\",\\\"reportSuites\\\":[\\\"examplesuite\\\"]}\"\n          ]\n        },\n        \"enabled\": {\n          \"type\": \"boolean\",\n          \"default\": true,\n          \"description\": \"Whether the extension is enabled.\"\n        },\n        \"published\": {\n          \"type\": \"boolean\",\n          \"description\": \"Whether the extension has been published.\",\n          \"readOnly\": true\n\
  \        },\n        \"dirty\": {\n          \"type\": \"boolean\",\n          \"description\": \"Whether the extension has unpublished changes.\",\n          \"readOnly\": true\n        },\n        \"revision_number\": {\n          \"type\": \"integer\",\n          \"minimum\": 0,\n          \"description\": \"The current revision number.\",\n          \"readOnly\": true\n        },\n        \"deleted_at\": {\n          \"type\": [\n            \"string\",\n            \"null\"\n          ],\n          \"format\": \"date-time\",\n          \"description\": \"When the extension was deleted. Null if the extension is active. Deleted extensions remain retrievable.\",\n          \"readOnly\": true\n        },\n        \"created_at\": {\n          \"type\": \"string\",\n          \"format\": \"date-time\",\n          \"description\": \"When the extension was created.\",\n          \"readOnly\": true\n        },\n        \"updated_at\": {\n          \"type\": \"string\",\n          \"format\"\
  : \"date-time\",\n          \"description\": \"When the extension was last updated.\",\n          \"readOnly\": true\n        }\n      }\n    },\n    \"relationships\": {\n      \"type\": \"object\",\n      \"description\": \"Related resources linked to this extension.\",\n      \"properties\": {\n        \"property\": {\n          \"$ref\": \"#/$defs/relationship\",\n          \"description\": \"The property where this extension is installed.\"\n        },\n        \"extension_package\": {\n          \"$ref\": \"#/$defs/relationship\",\n          \"description\": \"The extension package from which this extension was installed.\"\n        },\n        \"libraries\": {\n          \"$ref\": \"#/$defs/relationship\",\n          \"description\": \"Libraries that include this extension.\"\n        },\n        \"revisions\": {\n          \"$ref\": \"#/$defs/relationship\",\n          \"description\": \"Previous revisions of this extension.\"\n        },\n        \"origin\": {\n          \"$ref\"\
  : \"#/$defs/relationship\",\n          \"description\": \"The previous revision from which this extension was derived.\"\n        }\n      }\n    },\n    \"links\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"self\": {\n          \"type\": \"string\",\n          \"format\": \"uri\",\n          \"description\": \"The canonical URL for this extension resource.\"\n        }\n      }\n    }\n  },\n  \"$defs\": {\n    \"relationship\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"data\": {\n          \"oneOf\": [\n            {\n              \"type\": \"object\",\n              \"properties\": {\n                \"id\": {\n                  \"type\": \"string\"\n                },\n                \"type\": {\n                  \"type\": \"string\"\n                }\n              }\n            },\n            {\n              \"type\": \"array\",\n              \"items\": {\n                \"type\": \"object\",\n                \"properties\"\
  : {\n                  \"id\": {\n                    \"type\": \"string\"\n                  },\n                  \"type\": {\n                    \"type\": \"string\"\n                  }\n                }\n              }\n            }\n          ]\n        },\n        \"links\": {\n          \"type\": \"object\",\n          \"properties\": {\n            \"related\": {\n              \"type\": \"string\",\n              \"format\": \"uri\"\n            }\n          }\n        }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adobe-launch/refs/heads/main/json-schema/extension.json
tags:
- Data Collection
- Edge Network
- Event Forwarding
- Marketing Technology
- Tag Management
title: Adobe Experience Platform Tags Extension
---
