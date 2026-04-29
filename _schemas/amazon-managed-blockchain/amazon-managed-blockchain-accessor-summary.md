---
description: A summary of accessor properties.
layout: schema
name: AccessorSummary
properties_list:
- description: ''
  name: Id
  type: object
- description: ''
  name: Type
  type: object
- description: ''
  name: Status
  type: object
- description: ''
  name: CreationDate
  type: object
- description: ''
  name: Arn
  type: object
provider_name: Amazon Managed Blockchain
provider_slug: amazon-managed-blockchain
schema_file: json-schema/amazon-managed-blockchain-accessor-summary-schema.json
slug: amazon-managed-blockchain-accessor-summary
source_filename: amazon-managed-blockchain-accessor-summary-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-managed-blockchain/refs/heads/main/json-schema/amazon-managed-blockchain-accessor-summary-schema.json\",\n  \"title\": \"AccessorSummary\",\n  \"description\": \"A summary of accessor properties.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Id\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ResourceIdString\"\n        },\n        {\n          \"description\": \"The unique identifier of the accessor.\"\n        }\n      ]\n    },\n    \"Type\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AccessorType\"\n        },\n        {\n          \"description\": \"<p>The type of the accessor.</p> <note> <p>Currently accessor type is restricted to <code>BILLING_TOKEN</code>.</p> </note>\"\n        }\n      ]\n    },\n    \"Status\": {\n      \"allOf\": [\n        {\n        \
  \  \"$ref\": \"#/components/schemas/AccessorStatus\"\n        },\n        {\n          \"description\": \"The current status of the accessor.\"\n        }\n      ]\n    },\n    \"CreationDate\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Timestamp\"\n        },\n        {\n          \"description\": \"The creation date and time of the accessor.\"\n        }\n      ]\n    },\n    \"Arn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ArnString\"\n        },\n        {\n          \"description\": \"The Amazon Resource Name (ARN) of the accessor. For more information about ARNs and their format, see <a href=\\\"https://docs.aws.amazon.com/general/latest/gr/aws-arns-and-namespaces.html\\\">Amazon Resource Names (ARNs)</a> in the <i>Amazon Web Services General Reference</i>.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-managed-blockchain/refs/heads/main/json-schema/amazon-managed-blockchain-accessor-summary-schema.json
tags:
- AWS
- Blockchain
- Distributed Ledger
- Hyperledger Fabric
- Ethereum
title: AccessorSummary
---
