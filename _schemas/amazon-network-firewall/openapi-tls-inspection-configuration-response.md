---
description: The high-level properties of a TLS inspection configuration. This, along with the <code>TLSInspectionConfiguration</code>, define the TLS inspection configuration. You can retrieve all objects for a TLS inspection configuration by calling <code>DescribeTLSInspectionConfiguration</code>.
layout: schema
name: TLSInspectionConfigurationResponse
properties_list:
- description: ''
  name: TLSInspectionConfigurationArn
  type: object
- description: ''
  name: TLSInspectionConfigurationName
  type: object
- description: ''
  name: TLSInspectionConfigurationId
  type: object
- description: ''
  name: TLSInspectionConfigurationStatus
  type: object
- description: ''
  name: Description
  type: object
- description: ''
  name: Tags
  type: object
- description: ''
  name: LastModifiedTime
  type: object
- description: ''
  name: NumberOfAssociations
  type: object
- description: ''
  name: EncryptionConfiguration
  type: object
- description: ''
  name: Certificates
  type: object
provider_name: Amazon Network Firewall
provider_slug: amazon-network-firewall
schema_file: json-schema/openapi-tls-inspection-configuration-response-schema.json
slug: openapi-tls-inspection-configuration-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-network-firewall/refs/heads/main/json-schema/openapi-tls-inspection-configuration-response-schema.json\",\n  \"title\": \"TLSInspectionConfigurationResponse\",\n  \"description\": \"The high-level properties of a TLS inspection configuration. This, along with the <code>TLSInspectionConfiguration</code>, define the TLS inspection configuration. You can retrieve all objects for a TLS inspection configuration by calling <code>DescribeTLSInspectionConfiguration</code>.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"TLSInspectionConfigurationArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ResourceArn\"\n        },\n        {\n          \"description\": \"The Amazon Resource Name (ARN) of the TLS inspection configuration.\"\n        }\n      ]\n    },\n    \"TLSInspectionConfigurationName\": {\n    \
  \  \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ResourceName\"\n        },\n        {\n          \"description\": \"The descriptive name of the TLS inspection configuration. You can't change the name of a TLS inspection configuration after you create it.\"\n        }\n      ]\n    },\n    \"TLSInspectionConfigurationId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ResourceId\"\n        },\n        {\n          \"description\": \"A unique identifier for the TLS inspection configuration. This ID is returned in the responses to create and list commands. You provide it to operations such as update and delete.\"\n        }\n      ]\n    },\n    \"TLSInspectionConfigurationStatus\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ResourceStatus\"\n        },\n        {\n          \"description\": \"Detailed information about the current status of a <a>TLSInspectionConfiguration</a>. You can retrieve this for\
  \ a TLS inspection configuration by calling <a>DescribeTLSInspectionConfiguration</a> and providing the TLS inspection configuration name and ARN.\"\n        }\n      ]\n    },\n    \"Description\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Description\"\n        },\n        {\n          \"description\": \"A description of the TLS inspection configuration. \"\n        }\n      ]\n    },\n    \"Tags\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TagList\"\n        },\n        {\n          \"description\": \"The key:value pairs to associate with the resource.\"\n        }\n      ]\n    },\n    \"LastModifiedTime\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/LastUpdateTime\"\n        },\n        {\n          \"description\": \"The last time that the TLS inspection configuration was changed.\"\n        }\n      ]\n    },\n    \"NumberOfAssociations\": {\n      \"allOf\": [\n        {\n   \
  \       \"$ref\": \"#/components/schemas/NumberOfAssociations\"\n        },\n        {\n          \"description\": \"The number of firewall policies that use this TLS inspection configuration.\"\n        }\n      ]\n    },\n    \"EncryptionConfiguration\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/EncryptionConfiguration\"\n        },\n        {\n          \"description\": \"A complex type that contains the Amazon Web Services KMS encryption configuration settings for your TLS inspection configuration.\"\n        }\n      ]\n    },\n    \"Certificates\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Certificates\"\n        },\n        {\n          \"description\": \"A list of the certificates associated with the TLS inspection configuration.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"TLSInspectionConfigurationArn\",\n    \"TLSInspectionConfigurationName\",\n    \"TLSInspectionConfigurationId\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-network-firewall/refs/heads/main/json-schema/openapi-tls-inspection-configuration-response-schema.json
tags:
- AWS
- Firewall
- Intrusion Detection
- Network Security
- VPC
title: TLSInspectionConfigurationResponse
---
