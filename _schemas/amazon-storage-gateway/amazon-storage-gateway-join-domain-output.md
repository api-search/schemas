---
description: JoinDomainOutput
layout: schema
name: JoinDomainOutput
properties_list:
- description: ''
  name: GatewayARN
  type: object
- description: ''
  name: ActiveDirectoryStatus
  type: object
provider_name: Amazon Storage Gateway
provider_slug: amazon-storage-gateway
schema_file: json-schema/amazon-storage-gateway-join-domain-output-schema.json
slug: amazon-storage-gateway-join-domain-output
source_filename: amazon-storage-gateway-join-domain-output-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-storage-gateway/refs/heads/main/json-schema/amazon-storage-gateway-join-domain-output-schema.json\",\n  \"title\": \"JoinDomainOutput\",\n  \"description\": \"JoinDomainOutput\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"GatewayARN\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/GatewayARN\"\n        },\n        {\n          \"description\": \"The unique Amazon Resource Name (ARN) of the gateway that joined the domain.\"\n        }\n      ]\n    },\n    \"ActiveDirectoryStatus\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ActiveDirectoryStatus\"\n        },\n        {\n          \"description\": \"<p>Indicates the status of the gateway as a member of the Active Directory domain.</p> <ul> <li> <p> <code>ACCESS_DENIED</code>: Indicates that the <code>JoinDomain</code>\
  \ operation failed due to an authentication error.</p> </li> <li> <p> <code>DETACHED</code>: Indicates that gateway is not joined to a domain.</p> </li> <li> <p> <code>JOINED</code>: Indicates that the gateway has successfully joined a domain.</p> </li> <li> <p> <code>JOINING</code>: Indicates that a <code>JoinDomain</code> operation is in progress.</p> </li> <li> <p> <code>NETWORK_ERROR</code>: Indicates that <code>JoinDomain</code> operation failed due to a network or connectivity error.</p> </li> <li> <p> <code>TIMEOUT</code>: Indicates that the <code>JoinDomain</code> operation failed because the operation didn't complete within the allotted time.</p> </li> <li> <p> <code>UNKNOWN_ERROR</code>: Indicates that the <code>JoinDomain</code> operation failed due to another type of error.</p> </li> </ul>\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-storage-gateway/refs/heads/main/json-schema/amazon-storage-gateway-join-domain-output-schema.json
tags:
- Backup
- File Storage
- Gateway
- Hybrid Cloud
- Storage
title: JoinDomainOutput
---
