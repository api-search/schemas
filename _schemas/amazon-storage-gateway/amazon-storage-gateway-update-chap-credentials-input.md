---
description: <p>A JSON object containing one or more of the following fields:</p> <ul> <li> <p> <a>UpdateChapCredentialsInput$InitiatorName</a> </p> </li> <li> <p> <a>UpdateChapCredentialsInput$SecretToAuthenticateInitiator</a> </p> </li> <li> <p> <a>UpdateChapCredentialsInput$SecretToAuthenticateTarget</a> </p> </li> <li> <p> <a>UpdateChapCredentialsInput$TargetARN</a> </p> </li> </ul>
layout: schema
name: UpdateChapCredentialsInput
properties_list:
- description: ''
  name: TargetARN
  type: object
- description: ''
  name: SecretToAuthenticateInitiator
  type: object
- description: ''
  name: InitiatorName
  type: object
- description: ''
  name: SecretToAuthenticateTarget
  type: object
provider_name: Amazon Storage Gateway
provider_slug: amazon-storage-gateway
schema_file: json-schema/amazon-storage-gateway-update-chap-credentials-input-schema.json
slug: amazon-storage-gateway-update-chap-credentials-input
source_filename: amazon-storage-gateway-update-chap-credentials-input-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-storage-gateway/refs/heads/main/json-schema/amazon-storage-gateway-update-chap-credentials-input-schema.json\",\n  \"title\": \"UpdateChapCredentialsInput\",\n  \"description\": \"<p>A JSON object containing one or more of the following fields:</p> <ul> <li> <p> <a>UpdateChapCredentialsInput$InitiatorName</a> </p> </li> <li> <p> <a>UpdateChapCredentialsInput$SecretToAuthenticateInitiator</a> </p> </li> <li> <p> <a>UpdateChapCredentialsInput$SecretToAuthenticateTarget</a> </p> </li> <li> <p> <a>UpdateChapCredentialsInput$TargetARN</a> </p> </li> </ul>\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"TargetARN\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TargetARN\"\n        },\n        {\n          \"description\": \"The Amazon Resource Name (ARN) of the iSCSI volume target. Use the <a>DescribeStorediSCSIVolumes</a>\
  \ operation to return the TargetARN for specified VolumeARN.\"\n        }\n      ]\n    },\n    \"SecretToAuthenticateInitiator\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ChapSecret\"\n        },\n        {\n          \"description\": \"<p>The secret key that the initiator (for example, the Windows client) must provide to participate in mutual CHAP with the target.</p> <note> <p>The secret key must be between 12 and 16 bytes when encoded in UTF-8.</p> </note>\"\n        }\n      ]\n    },\n    \"InitiatorName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/IqnName\"\n        },\n        {\n          \"description\": \"The iSCSI initiator that connects to the target.\"\n        }\n      ]\n    },\n    \"SecretToAuthenticateTarget\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ChapSecret\"\n        },\n        {\n          \"description\": \"<p>The secret key that the target must provide\
  \ to participate in mutual CHAP with the initiator (e.g. Windows client).</p> <p>Byte constraints: Minimum bytes of 12. Maximum bytes of 16.</p> <note> <p>The secret key must be between 12 and 16 bytes when encoded in UTF-8.</p> </note>\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"TargetARN\",\n    \"SecretToAuthenticateInitiator\",\n    \"InitiatorName\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-storage-gateway/refs/heads/main/json-schema/amazon-storage-gateway-update-chap-credentials-input-schema.json
tags:
- AWS
- Backup
- File Storage
- Gateway
- Hybrid Cloud
- Storage
title: UpdateChapCredentialsInput
---
