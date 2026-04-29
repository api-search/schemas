---
description: Schema representing an AWS Shield protection resource. A protection enables AWS Shield Advanced DDoS protection for a specific AWS resource such as an Elastic IP, CloudFront distribution, or Application Load Balancer.
layout: schema
name: Amazon Shield Protection
properties_list:
- description: The unique identifier (ID) of the protection.
  name: Id
  type: string
- description: The name of the protection.
  name: Name
  type: string
- description: The ARN of the AWS resource that is protected.
  name: ResourceArn
  type: string
- description: The ARN of the protection.
  name: ProtectionArn
  type: string
- description: The unique identifiers for the health check associations.
  name: HealthCheckIds
  type: array
- description: ''
  name: ApplicationLayerAutomaticResponseConfiguration
  type: object
- description: Tags associated with the protection.
  name: Tags
  type: array
provider_name: Amazon Shield
provider_slug: amazon-shield
schema_file: json-schema/amazon-shield-protection-schema.json
slug: amazon-shield-protection
source_filename: amazon-shield-protection-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$id\": \"https://schema.api.io/amazon-shield/amazon-shield-protection-schema.json\",\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Amazon Shield Protection\",\n  \"description\": \"Schema representing an AWS Shield protection resource. A protection enables AWS Shield Advanced DDoS protection for a specific AWS resource such as an Elastic IP, CloudFront distribution, or Application Load Balancer.\",\n  \"type\": \"object\",\n  \"required\": [\n    \"Name\",\n    \"ResourceArn\"\n  ],\n  \"properties\": {\n    \"Id\": {\n      \"type\": \"string\",\n      \"description\": \"The unique identifier (ID) of the protection.\"\n    },\n    \"Name\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the protection.\",\n      \"minLength\": 1,\n      \"maxLength\": 128\n    },\n    \"ResourceArn\": {\n      \"type\": \"string\",\n      \"description\": \"The ARN of the AWS resource that is protected.\"\n    },\n    \"ProtectionArn\"\
  : {\n      \"type\": \"string\",\n      \"description\": \"The ARN of the protection.\",\n      \"pattern\": \"^arn:aws:shield::[0-9]{12}:protection/[a-zA-Z0-9-]+$\"\n    },\n    \"HealthCheckIds\": {\n      \"type\": \"array\",\n      \"description\": \"The unique identifiers for the health check associations.\",\n      \"items\": {\n        \"type\": \"string\"\n      }\n    },\n    \"ApplicationLayerAutomaticResponseConfiguration\": {\n      \"$ref\": \"#/$defs/ApplicationLayerAutomaticResponseConfiguration\"\n    },\n    \"Tags\": {\n      \"type\": \"array\",\n      \"description\": \"Tags associated with the protection.\",\n      \"items\": {\n        \"$ref\": \"#/$defs/Tag\"\n      }\n    }\n  },\n  \"$defs\": {\n    \"ApplicationLayerAutomaticResponseConfiguration\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"Status\": {\n          \"type\": \"string\",\n          \"description\": \"Indicates whether automatic application layer DDoS mitigation is enabled.\"\
  ,\n          \"enum\": [\"ENABLED\", \"DISABLED\"]\n        },\n        \"Action\": {\n          \"type\": \"object\",\n          \"description\": \"Specifies the action setting for the automatic response.\",\n          \"properties\": {\n            \"Block\": {\n              \"type\": \"object\",\n              \"description\": \"Specifies that Shield Advanced should block requests.\"\n            },\n            \"Count\": {\n              \"type\": \"object\",\n              \"description\": \"Specifies that Shield Advanced should count requests.\"\n            }\n          }\n        }\n      }\n    },\n    \"Tag\": {\n      \"type\": \"object\",\n      \"required\": [\"Key\"],\n      \"properties\": {\n        \"Key\": {\n          \"type\": \"string\",\n          \"minLength\": 1,\n          \"maxLength\": 128\n        },\n        \"Value\": {\n          \"type\": \"string\",\n          \"maxLength\": 256\n        }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-shield/refs/heads/main/json-schema/amazon-shield-protection-schema.json
tags:
- AWS
- DDoS Protection
- Networking
- Security
title: Amazon Shield Protection
---
