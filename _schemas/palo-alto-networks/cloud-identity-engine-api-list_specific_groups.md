---
description: Retrieve specific groups matching a name-based filter. Supports filtering of groups based on specific attributes and values (similar to the WHERE clause in SQL).
layout: schema
name: list_specific_groups
properties_list:
- description: Attribute-based filter.
  name: name
  type: object
- description: group attributes part of the response
  name: attrs
  type: array
provider_name: Palo Alto Networks
provider_slug: palo-alto-networks
schema_file: json-schema/cloud-identity-engine-api-list_specific_groups-schema.json
slug: cloud-identity-engine-api-list_specific_groups
source_filename: cloud-identity-engine-api-list_specific_groups-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"list_specific_groups\",\n  \"description\": \"Retrieve specific groups matching a name-based filter. Supports filtering of groups based on specific attributes and values (similar to the WHERE clause in SQL).\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/cloud-identity-engine-api-list_specific_groups-schema.json\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"object\",\n      \"description\": \"Attribute-based filter.\",\n      \"required\": [\n        \"attrName\",\n        \"attrValue\",\n        \"match\"\n      ],\n      \"properties\": {\n        \"attrName\": {\n          \"description\": \"Attribute name\",\n          \"type\": \"string\",\n          \"enum\": [\n            \"User Principal Name\",\n            \"Common-Name\",\n            \"Name\",\n            \"Distinguished Name\",\n            \"SAM Account\
  \ Name\",\n            \"Unique Identifier\"\n          ],\n          \"example\": \"Distinguished Name\"\n        },\n        \"attrValue\": {\n          \"description\": \"Attribute value\",\n          \"type\": \"string\",\n          \"example\": \"CN=Jack,UID=Park,DC=example,DC=com\"\n        },\n        \"match\": {\n          \"description\": \"Value you want to match.\",\n          \"type\": \"string\",\n          \"enum\": [\n            \"equal\",\n            \"textSearch\"\n          ],\n          \"example\": \"equal\"\n        }\n      }\n    },\n    \"attrs\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"description\": \"group attributes part of the response\",\n      \"example\": [\n        \"Common-Name\",\n        \"Unique Identifier\",\n        \"Name\",\n        \"Distinguished Name\",\n        \"SAM Account Name\"\n      ]\n    }\n  },\n  \"required\": [\n    \"name\"\n  ],\n  \"allOf\": [\n    {\n      \"description\"\
  : \"Retrieve all groups in a particular domain.\",\n      \"allOf\": [\n        {\n          \"type\": \"object\",\n          \"description\": \"Domain name for a specific directory.\",\n          \"required\": [\n            \"domain\"\n          ],\n          \"properties\": {\n            \"domain\": {\n              \"type\": \"string\",\n              \"description\": \"Domain name of the target directory.\",\n              \"example\": \"paloaltonetworks.com\"\n            }\n          }\n        },\n        {\n          \"type\": \"object\",\n          \"description\": \"Optional pagination parameters.\",\n          \"properties\": {\n            \"pageNum\": {\n              \"type\": \"integer\",\n              \"description\": \"Page number to retrieve (starting from page 1).\",\n              \"example\": 1\n            },\n            \"pageSz\": {\n              \"type\": \"integer\",\n              \"description\": \"Number of records per page (max is 1000 per page).\",\n\
  \              \"example\": 500\n            }\n          }\n        }\n      ],\n      \"required\": [\n        \"attrs\"\n      ],\n      \"properties\": {\n        \"attrs\": {\n          \"type\": \"array\",\n          \"items\": {\n            \"type\": \"string\"\n          },\n          \"description\": \"Group attributes included as part of the response.\",\n          \"example\": [\n            \"Common-Name\",\n            \"Unique Identifier\",\n            \"Name\",\n            \"Distinguished Name\",\n            \"SAM Account Name\"\n          ]\n        },\n        \"useNormalizedAttrs\": {\n          \"type\": \"string\",\n          \"enum\": [\n            \"True\",\n            \"False\"\n          ]\n        }\n      },\n      \"example\": {\n        \"domain\": \"paloaltonetworks.com\",\n        \"pageNum\": \"1,\",\n        \"pageSz\": 80\n      }\n    }\n  ],\n  \"type\": \"object\"\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/cloud-identity-engine-api-list_specific_groups-schema.json
tags:
- Cloud Security
- Cybersecurity
- Firewall
- Network Security
- SASE
- SOAR
- Threat Intelligence
- XDR
title: list_specific_groups
---
