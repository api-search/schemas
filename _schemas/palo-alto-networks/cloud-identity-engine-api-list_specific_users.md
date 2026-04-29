---
description: Retrieve specific users matching a name-based filter in a domain. Supports filtering of users based on specific attributes and values (similar to the WHERE clause in SQL).
layout: schema
name: list_specific_users
properties_list:
- description: Attribute-based filter.
  name: name
  type: object
provider_name: Palo Alto Networks
provider_slug: palo-alto-networks
schema_file: json-schema/cloud-identity-engine-api-list_specific_users-schema.json
slug: cloud-identity-engine-api-list_specific_users
source_filename: cloud-identity-engine-api-list_specific_users-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"list_specific_users\",\n  \"description\": \"Retrieve specific users matching a name-based filter in a domain. Supports filtering of users based on specific attributes and values (similar to the WHERE clause in SQL).\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/cloud-identity-engine-api-list_specific_users-schema.json\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"object\",\n      \"description\": \"Attribute-based filter.\",\n      \"required\": [\n        \"attrName\",\n        \"attrValue\",\n        \"match\"\n      ],\n      \"properties\": {\n        \"attrName\": {\n          \"description\": \"Attribute name\",\n          \"type\": \"string\",\n          \"enum\": [\n            \"User Principal Name\",\n            \"Common-Name\",\n            \"Name\",\n            \"Distinguished Name\",\n          \
  \  \"SAM Account Name\",\n            \"Unique Identifier\"\n          ],\n          \"example\": \"Distinguished Name\"\n        },\n        \"attrValue\": {\n          \"description\": \"Attribute value\",\n          \"type\": \"string\",\n          \"example\": \"CN=Jack,UID=Park,DC=example,DC=com\"\n        },\n        \"match\": {\n          \"description\": \"Value you want to match.\",\n          \"type\": \"string\",\n          \"enum\": [\n            \"equal\",\n            \"textSearch\"\n          ],\n          \"example\": \"equal\"\n        }\n      }\n    }\n  },\n  \"required\": [\n    \"name\"\n  ],\n  \"allOf\": [\n    {\n      \"description\": \"Retrieve all attributes for a specific user.\",\n      \"allOf\": [\n        {\n          \"type\": \"object\",\n          \"description\": \"Domain name for a specific directory.\",\n          \"required\": [\n            \"domain\"\n          ],\n          \"properties\": {\n            \"domain\": {\n              \"type\"\
  : \"string\",\n              \"description\": \"Domain name of the target directory.\",\n              \"example\": \"paloaltonetworks.com\"\n            }\n          }\n        },\n        {\n          \"type\": \"object\",\n          \"description\": \"Optional pagination parameters.\",\n          \"properties\": {\n            \"pageNum\": {\n              \"type\": \"integer\",\n              \"description\": \"Page number to retrieve (starting from page 1).\",\n              \"example\": 1\n            },\n            \"pageSz\": {\n              \"type\": \"integer\",\n              \"description\": \"Number of records per page (max is 1000 per page).\",\n              \"example\": 500\n            }\n          }\n        }\n      ],\n      \"properties\": {\n        \"attrs\": {\n          \"type\": \"array\",\n          \"description\": \"User attributes included as part of the response.\",\n          \"items\": {\n            \"type\": \"string\"\n          },\n          \"example\"\
  : [\n            \"Common-Name\",\n            \"Mail\",\n            \"Unique Identifier\",\n            \"Manager\",\n            \"User Principal Name\",\n            \"Name\",\n            \"Distinguished Name\",\n            \"SAM Account Name\"\n          ]\n        },\n        \"useNormalizedAttrs\": {\n          \"description\": \"Use the normalized attribute.\",\n          \"type\": \"string\",\n          \"enum\": [\n            \"True\",\n            \"False\"\n          ],\n          \"example\": \"True\"\n        }\n      },\n      \"example\": {\n        \"domain\": \"paloaltonetworks.com\",\n        \"attrs\": [\n          \"Common-Name\",\n          \"Mail\",\n          \"Unique Identifier\",\n          \"Manager\",\n          \"User Principal Name\",\n          \"Name\",\n          \"Distinguished Name\",\n          \"SAM Account Name\"\n        ],\n        \"useNormalizedAttrs\": \"True\"\n      }\n    }\n  ],\n  \"type\": \"object\"\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/cloud-identity-engine-api-list_specific_users-schema.json
tags:
- Cloud Security
- Cybersecurity
- Firewall
- Network Security
- SASE
- SOAR
- Threat Intelligence
- XDR
title: list_specific_users
---
