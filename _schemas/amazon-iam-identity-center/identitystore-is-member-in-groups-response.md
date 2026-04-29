---
description: IsMemberInGroupsResponse schema from AWS IAM Identity Center
layout: schema
name: IsMemberInGroupsResponse
properties_list:
- description: ''
  name: Results
  type: object
provider_name: Amazon IAM Identity Center
provider_slug: amazon-iam-identity-center
schema_file: json-schema/identitystore-is-member-in-groups-response-schema.json
slug: identitystore-is-member-in-groups-response
source_filename: identitystore-is-member-in-groups-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iam-identity-center/refs/heads/main/json-schema/identitystore-is-member-in-groups-response-schema.json\",\n  \"title\": \"IsMemberInGroupsResponse\",\n  \"description\": \"IsMemberInGroupsResponse schema from AWS IAM Identity Center\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Results\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/GroupMembershipExistenceResults\"\n        },\n        {\n          \"description\": \"A list containing the results of membership existence checks.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"Results\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iam-identity-center/refs/heads/main/json-schema/identitystore-is-member-in-groups-response-schema.json
tags:
- Access Control
- Authentication
- AWS
- Identity Management
- Single Sign-On
title: IsMemberInGroupsResponse
---
