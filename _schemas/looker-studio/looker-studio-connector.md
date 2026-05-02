---
description: Represents a Looker Studio community connector configuration, defining how the connector authenticates, presents configuration options, declares its data schema, and serves data to Looker Studio.
layout: schema
name: Looker Studio Community Connector
properties_list:
- description: The display name of the connector.
  name: name
  type: string
- description: URL to the connector's logo image.
  name: logoUrl
  type: string
- description: The company or organization that developed the connector.
  name: company
  type: string
- description: URL to the developer's website.
  name: companyUrl
  type: string
- description: URL to the connector's Apps Script project.
  name: addonUrl
  type: string
- description: URL to the connector's support page.
  name: supportUrl
  type: string
- description: A text description of what the connector does.
  name: description
  type: string
- description: The authentication type required by the connector.
  name: authType
  type: string
- description: The Google Drive folder ID where the connector project is stored.
  name: folderId
  type: string
- description: Whether the current user is an admin of this connector.
  name: isAdminUser
  type: boolean
- description: The user-configurable parameters for the connector.
  name: configParams
  type: array
- description: Whether the connector requires a date range to be specified.
  name: dateRangeRequired
  type: boolean
- description: The field definitions that make up the connector's data schema.
  name: schema
  type: array
provider_name: Looker Studio
provider_slug: looker-studio
schema_file: json-schema/looker-studio-connector-schema.json
slug: looker-studio-connector
source_filename: looker-studio-connector-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://github.com/api-evangelist/looker-studio/json-schema/looker-studio-connector-schema.json\",\n  \"title\": \"Looker Studio Community Connector\",\n  \"description\": \"Represents a Looker Studio community connector configuration, defining how the connector authenticates, presents configuration options, declares its data schema, and serves data to Looker Studio.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The display name of the connector.\"\n    },\n    \"logoUrl\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"description\": \"URL to the connector's logo image.\"\n    },\n    \"company\": {\n      \"type\": \"string\",\n      \"description\": \"The company or organization that developed the connector.\"\n    },\n    \"companyUrl\": {\n      \"type\": \"string\",\n      \"format\": \"uri\"\
  ,\n      \"description\": \"URL to the developer's website.\"\n    },\n    \"addonUrl\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"description\": \"URL to the connector's Apps Script project.\"\n    },\n    \"supportUrl\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"description\": \"URL to the connector's support page.\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"A text description of what the connector does.\"\n    },\n    \"authType\": {\n      \"type\": \"string\",\n      \"description\": \"The authentication type required by the connector.\",\n      \"enum\": [\n        \"NONE\",\n        \"OAUTH2\",\n        \"KEY\",\n        \"USER_PASS\",\n        \"USER_TOKEN\",\n        \"PATH_USER_PASS\",\n        \"PATH_KEY\"\n      ]\n    },\n    \"folderId\": {\n      \"type\": \"string\",\n      \"description\": \"The Google Drive folder ID where the connector project is stored.\"\n    },\n    \"\
  isAdminUser\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the current user is an admin of this connector.\"\n    },\n    \"configParams\": {\n      \"type\": \"array\",\n      \"description\": \"The user-configurable parameters for the connector.\",\n      \"items\": {\n        \"$ref\": \"#/$defs/ConfigParam\"\n      }\n    },\n    \"dateRangeRequired\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the connector requires a date range to be specified.\"\n    },\n    \"schema\": {\n      \"type\": \"array\",\n      \"description\": \"The field definitions that make up the connector's data schema.\",\n      \"items\": {\n        \"$ref\": \"#/$defs/Field\"\n      }\n    }\n  },\n  \"required\": [\n    \"name\",\n    \"authType\"\n  ],\n  \"$defs\": {\n    \"ConfigParam\": {\n      \"type\": \"object\",\n      \"description\": \"A single configuration parameter definition.\",\n      \"properties\": {\n        \"type\": {\n          \"type\": \"\
  string\",\n          \"description\": \"The type of UI element to render.\",\n          \"enum\": [\n            \"TEXTINPUT\",\n            \"TEXTAREA\",\n            \"SELECT_SINGLE\",\n            \"SELECT_MULTIPLE\",\n            \"CHECKBOX\",\n            \"INFO\"\n          ]\n        },\n        \"name\": {\n          \"type\": \"string\",\n          \"description\": \"The unique identifier for this parameter.\"\n        },\n        \"displayName\": {\n          \"type\": \"string\",\n          \"description\": \"The label displayed to the user.\"\n        },\n        \"helpText\": {\n          \"type\": \"string\",\n          \"description\": \"Help text shown below the input element.\"\n        },\n        \"placeholder\": {\n          \"type\": \"string\",\n          \"description\": \"Placeholder text for text input elements.\"\n        },\n        \"isDynamic\": {\n          \"type\": \"boolean\",\n          \"description\": \"Whether this parameter triggers a re-fetch of config\
  \ when changed.\"\n        },\n        \"options\": {\n          \"type\": \"array\",\n          \"description\": \"Available options for SELECT_SINGLE and SELECT_MULTIPLE types.\",\n          \"items\": {\n            \"type\": \"object\",\n            \"properties\": {\n              \"label\": {\n                \"type\": \"string\",\n                \"description\": \"Display label for the option.\"\n              },\n              \"value\": {\n                \"type\": \"string\",\n                \"description\": \"The value submitted when this option is selected.\"\n              }\n            },\n            \"required\": [\n              \"label\",\n              \"value\"\n            ]\n          }\n        }\n      },\n      \"required\": [\n        \"type\",\n        \"name\"\n      ]\n    },\n    \"Field\": {\n      \"type\": \"object\",\n      \"description\": \"Defines a single field in the connector's data schema.\",\n      \"properties\": {\n        \"name\": {\n  \
  \        \"type\": \"string\",\n          \"description\": \"The unique identifier for the field.\"\n        },\n        \"label\": {\n          \"type\": \"string\",\n          \"description\": \"The display name for the field.\"\n        },\n        \"description\": {\n          \"type\": \"string\",\n          \"description\": \"A text description of the field's contents.\"\n        },\n        \"dataType\": {\n          \"type\": \"string\",\n          \"description\": \"The data type of the field values.\",\n          \"enum\": [\n            \"STRING\",\n            \"NUMBER\",\n            \"BOOLEAN\"\n          ]\n        },\n        \"conceptType\": {\n          \"type\": \"string\",\n          \"description\": \"Whether the field is a dimension or metric.\",\n          \"enum\": [\n            \"DIMENSION\",\n            \"METRIC\"\n          ]\n        },\n        \"semanticType\": {\n          \"type\": \"string\",\n          \"description\": \"The semantic type describing\
  \ the meaning of the field values.\"\n        },\n        \"defaultAggregationType\": {\n          \"type\": \"string\",\n          \"description\": \"The default aggregation type for metric fields.\",\n          \"enum\": [\n            \"AVG\",\n            \"COUNT\",\n            \"COUNT_DISTINCT\",\n            \"MAX\",\n            \"MIN\",\n            \"SUM\",\n            \"AUTO\",\n            \"NONE\"\n          ]\n        },\n        \"group\": {\n          \"type\": \"string\",\n          \"description\": \"An optional group name for organizing related fields.\"\n        },\n        \"formula\": {\n          \"type\": \"string\",\n          \"description\": \"An optional calculated field formula.\"\n        },\n        \"isHidden\": {\n          \"type\": \"boolean\",\n          \"description\": \"Whether the field is hidden from the user interface.\"\n        }\n      },\n      \"required\": [\n        \"name\",\n        \"dataType\",\n        \"conceptType\"\n      ]\n  \
  \  }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/looker-studio/refs/heads/main/json-schema/looker-studio-connector-schema.json
tags:
- Analytics
- Business Intelligence
- Dashboards
- Data Visualization
- Google
- Reports
title: Looker Studio Community Connector
---
