---
description: Describes a trust relationship between an Managed Microsoft AD directory and an external domain.
layout: schema
name: Trust
properties_list:
- description: ''
  name: DirectoryId
  type: object
- description: ''
  name: TrustId
  type: object
- description: ''
  name: RemoteDomainName
  type: object
- description: ''
  name: TrustType
  type: object
- description: ''
  name: TrustDirection
  type: object
- description: ''
  name: TrustState
  type: object
- description: ''
  name: CreatedDateTime
  type: object
- description: ''
  name: LastUpdatedDateTime
  type: object
- description: ''
  name: StateLastUpdatedDateTime
  type: object
- description: ''
  name: TrustStateReason
  type: object
- description: ''
  name: SelectiveAuth
  type: object
provider_name: Amazon Directory Service
provider_slug: amazon-directory-service
schema_file: json-schema/amazon-directory-service-trust-schema.json
slug: amazon-directory-service-trust
source_filename: amazon-directory-service-trust-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-directory-service/refs/heads/main/json-schema/amazon-directory-service-trust-schema.json\",\n  \"title\": \"Trust\",\n  \"description\": \"Describes a trust relationship between an Managed Microsoft AD directory and an external domain.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"DirectoryId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DirectoryId\"\n        },\n        {\n          \"description\": \"The Directory ID of the Amazon Web Services directory involved in the trust relationship.\"\n        }\n      ]\n    },\n    \"TrustId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TrustId\"\n        },\n        {\n          \"description\": \"The unique ID of the trust relationship.\"\n        }\n      ]\n    },\n    \"RemoteDomainName\": {\n      \"allOf\": [\n\
  \        {\n          \"$ref\": \"#/components/schemas/RemoteDomainName\"\n        },\n        {\n          \"description\": \"The Fully Qualified Domain Name (FQDN) of the external domain involved in the trust relationship.\"\n        }\n      ]\n    },\n    \"TrustType\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TrustType\"\n        },\n        {\n          \"description\": \"The trust relationship type. <code>Forest</code> is the default.\"\n        }\n      ]\n    },\n    \"TrustDirection\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TrustDirection\"\n        },\n        {\n          \"description\": \"The trust relationship direction.\"\n        }\n      ]\n    },\n    \"TrustState\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TrustState\"\n        },\n        {\n          \"description\": \"The trust relationship state.\"\n        }\n      ]\n    },\n    \"CreatedDateTime\": {\n\
  \      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/CreatedDateTime\"\n        },\n        {\n          \"description\": \"The date and time that the trust relationship was created.\"\n        }\n      ]\n    },\n    \"LastUpdatedDateTime\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/LastUpdatedDateTime\"\n        },\n        {\n          \"description\": \"The date and time that the trust relationship was last updated.\"\n        }\n      ]\n    },\n    \"StateLastUpdatedDateTime\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/StateLastUpdatedDateTime\"\n        },\n        {\n          \"description\": \"The date and time that the TrustState was last updated.\"\n        }\n      ]\n    },\n    \"TrustStateReason\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TrustStateReason\"\n        },\n        {\n          \"description\": \"The reason for the TrustState.\"\n\
  \        }\n      ]\n    },\n    \"SelectiveAuth\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SelectiveAuth\"\n        },\n        {\n          \"description\": \"Current state of selective authentication for the trust.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-directory-service/refs/heads/main/json-schema/amazon-directory-service-trust-schema.json
tags:
- Active Directory
- Authentication
- AWS
- Directory Services
- Identity Management
title: Trust
---
