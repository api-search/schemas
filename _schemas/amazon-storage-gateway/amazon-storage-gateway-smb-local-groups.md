---
description: A list of Active Directory users and groups that have special permissions for SMB file shares on the gateway.
layout: schema
name: SMBLocalGroups
properties_list:
- description: ''
  name: GatewayAdmins
  type: object
provider_name: Amazon Storage Gateway
provider_slug: amazon-storage-gateway
schema_file: json-schema/amazon-storage-gateway-smb-local-groups-schema.json
slug: amazon-storage-gateway-smb-local-groups
source_filename: amazon-storage-gateway-smb-local-groups-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-storage-gateway/refs/heads/main/json-schema/amazon-storage-gateway-smb-local-groups-schema.json\",\n  \"title\": \"SMBLocalGroups\",\n  \"description\": \"A list of Active Directory users and groups that have special permissions for SMB file shares on the gateway.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"GatewayAdmins\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/UserList\"\n        },\n        {\n          \"description\": \"<p>A list of Active Directory users and groups that have local Gateway Admin permissions. Acceptable formats include: <code>DOMAIN\\\\User1</code>, <code>user1</code>, <code>DOMAIN\\\\group1</code>, and <code>group1</code>.</p> <p>Gateway Admins can use the Shared Folders Microsoft Management Console snap-in to force-close files that are open and locked.</p>\"\n      \
  \  }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-storage-gateway/refs/heads/main/json-schema/amazon-storage-gateway-smb-local-groups-schema.json
tags:
- AWS
- Backup
- File Storage
- Gateway
- Hybrid Cloud
- Storage
title: SMBLocalGroups
---
