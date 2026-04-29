---
description: Retrieve specific attributes for users belonging to a particular group, filtered using the group-based filter.
layout: schema
name: list_users_in_particular_group
properties_list:
- description: Group-based filter.
  name: filter
  type: object
- description: user attributes part of the response
  name: attrs
  type: array
provider_name: Palo Alto Networks
provider_slug: palo-alto-networks
schema_file: json-schema/cloud-identity-engine-api-list_users_in_particular_group-schema.json
slug: cloud-identity-engine-api-list_users_in_particular_group
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"list_users_in_particular_group\",\n  \"description\": \"Retrieve specific attributes for users belonging to a particular group, filtered using the group-based filter.\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/cloud-identity-engine-api-list_users_in_particular_group-schema.json\",\n  \"properties\": {\n    \"filter\": {\n      \"type\": \"object\",\n      \"description\": \"Group-based filter.\",\n      \"required\": [\n        \"type\",\n        \"name\",\n        \"level\"\n      ],\n      \"properties\": {\n        \"type\": {\n          \"type\": \"string\",\n          \"enum\": [\n            \"group\"\n          ]\n        },\n        \"name\": {\n          \"type\": \"object\",\n          \"description\": \"Attribute-based filter.\",\n          \"required\": [\n            \"attrName\",\n            \"attrValue\",\n\
  \            \"match\"\n          ],\n          \"properties\": {\n            \"attrName\": {\n              \"description\": \"Attribute name\",\n              \"type\": \"string\",\n              \"enum\": [\n                \"User Principal Name\",\n                \"Common-Name\",\n                \"Name\",\n                \"Distinguished Name\",\n                \"SAM Account Name\",\n                \"Unique Identifier\"\n              ],\n              \"example\": \"Distinguished Name\"\n            },\n            \"attrValue\": {\n              \"description\": \"Attribute value\",\n              \"type\": \"string\",\n              \"example\": \"CN=Jack,UID=Park,DC=example,DC=com\"\n            },\n            \"match\": {\n              \"description\": \"Value you want to match.\",\n              \"type\": \"string\",\n              \"enum\": [\n                \"equal\",\n                \"textSearch\"\n              ],\n              \"example\": \"equal\"\n         \
  \   }\n          }\n        },\n        \"level\": {\n          \"type\": \"string\",\n          \"enum\": [\n            \"immediate\",\n            \"recursive\"\n          ]\n        }\n      }\n    },\n    \"attrs\": {\n      \"type\": \"array\",\n      \"description\": \"user attributes part of the response\",\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"example\": [\n        \"Common-Name\",\n        \"Mail\",\n        \"Unique Identifier\",\n        \"Manager\",\n        \"User Principal Name\",\n        \"Name\",\n        \"Distinguished Name\",\n        \"SAM Account Name\"\n      ]\n    }\n  },\n  \"required\": [\n    \"filter\"\n  ],\n  \"allOf\": [\n    {\n      \"type\": \"object\",\n      \"description\": \"Domain name for a specific directory.\",\n      \"required\": [\n        \"domain\"\n      ],\n      \"properties\": {\n        \"domain\": {\n          \"type\": \"string\",\n          \"description\": \"Domain name of the target directory.\",\n\
  \          \"example\": \"paloaltonetworks.com\"\n        }\n      }\n    },\n    {\n      \"type\": \"object\",\n      \"description\": \"Optional pagination parameters.\",\n      \"properties\": {\n        \"pageNum\": {\n          \"type\": \"integer\",\n          \"description\": \"Page number to retrieve (starting from page 1).\",\n          \"example\": 1\n        },\n        \"pageSz\": {\n          \"type\": \"integer\",\n          \"description\": \"Number of records per page (max is 1000 per page).\",\n          \"example\": 500\n        }\n      }\n    }\n  ],\n  \"type\": \"object\"\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/cloud-identity-engine-api-list_users_in_particular_group-schema.json
tags:
- Cloud Security
- Cybersecurity
- Firewall
- Network Security
- SASE
- SOAR
- Threat Intelligence
- XDR
title: list_users_in_particular_group
---
