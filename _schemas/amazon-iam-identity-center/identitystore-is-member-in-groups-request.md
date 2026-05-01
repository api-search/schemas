---
description: IsMemberInGroupsRequest schema from AWS IAM Identity Center
layout: schema
name: IsMemberInGroupsRequest
properties_list:
- description: ''
  name: IdentityStoreId
  type: object
- description: ''
  name: MemberId
  type: object
- description: ''
  name: GroupIds
  type: object
provider_name: Amazon IAM Identity Center
provider_slug: amazon-iam-identity-center
schema_file: json-schema/identitystore-is-member-in-groups-request-schema.json
slug: identitystore-is-member-in-groups-request
source_filename: identitystore-is-member-in-groups-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iam-identity-center/refs/heads/main/json-schema/identitystore-is-member-in-groups-request-schema.json\",\n  \"title\": \"IsMemberInGroupsRequest\",\n  \"description\": \"IsMemberInGroupsRequest schema from AWS IAM Identity Center\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"IdentityStoreId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/IdentityStoreId\"\n        },\n        {\n          \"description\": \"The globally unique identifier for the identity store.\"\n        }\n      ]\n    },\n    \"MemberId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/MemberId\"\n        },\n        {\n          \"description\": \"An object containing the identifier of a group member.\"\n        }\n      ]\n    },\n    \"GroupIds\": {\n      \"allOf\": [\n        {\n          \"$ref\"\
  : \"#/components/schemas/GroupIds\"\n        },\n        {\n          \"description\": \"A list of identifiers for groups in the identity store.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"IdentityStoreId\",\n    \"MemberId\",\n    \"GroupIds\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iam-identity-center/refs/heads/main/json-schema/identitystore-is-member-in-groups-request-schema.json
tags:
- Access Control
- Authentication
- Identity Management
- Single Sign-On
title: IsMemberInGroupsRequest
---
