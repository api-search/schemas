---
description: <p>A JSON object containing one or more of the following fields:</p> <ul> <li> <p> <a>DeleteChapCredentialsInput$InitiatorName</a> </p> </li> <li> <p> <a>DeleteChapCredentialsInput$TargetARN</a> </p> </li> </ul>
layout: schema
name: DeleteChapCredentialsInput
properties_list:
- description: ''
  name: TargetARN
  type: object
- description: ''
  name: InitiatorName
  type: object
provider_name: Amazon Storage Gateway
provider_slug: amazon-storage-gateway
schema_file: json-schema/amazon-storage-gateway-delete-chap-credentials-input-schema.json
slug: amazon-storage-gateway-delete-chap-credentials-input
source_filename: amazon-storage-gateway-delete-chap-credentials-input-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-storage-gateway/refs/heads/main/json-schema/amazon-storage-gateway-delete-chap-credentials-input-schema.json\",\n  \"title\": \"DeleteChapCredentialsInput\",\n  \"description\": \"<p>A JSON object containing one or more of the following fields:</p> <ul> <li> <p> <a>DeleteChapCredentialsInput$InitiatorName</a> </p> </li> <li> <p> <a>DeleteChapCredentialsInput$TargetARN</a> </p> </li> </ul>\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"TargetARN\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TargetARN\"\n        },\n        {\n          \"description\": \"The Amazon Resource Name (ARN) of the iSCSI volume target. Use the <a>DescribeStorediSCSIVolumes</a> operation to return to retrieve the TargetARN for specified VolumeARN.\"\n        }\n      ]\n    },\n    \"InitiatorName\": {\n      \"allOf\": [\n\
  \        {\n          \"$ref\": \"#/components/schemas/IqnName\"\n        },\n        {\n          \"description\": \"The iSCSI initiator that connects to the target.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"TargetARN\",\n    \"InitiatorName\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-storage-gateway/refs/heads/main/json-schema/amazon-storage-gateway-delete-chap-credentials-input-schema.json
tags:
- Backup
- File Storage
- Gateway
- Hybrid Cloud
- Storage
title: DeleteChapCredentialsInput
---
