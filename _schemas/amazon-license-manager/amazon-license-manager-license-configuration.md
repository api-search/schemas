---
description: An AWS License Manager license configuration.
layout: schema
name: LicenseConfiguration
properties_list:
- description: Unique ID of the license configuration.
  name: LicenseConfigurationId
  type: string
- description: Amazon Resource Name (ARN) of the license configuration.
  name: LicenseConfigurationArn
  type: string
- description: Name of the license configuration.
  name: Name
  type: string
- description: Dimension for which the licenses are counted.
  name: LicenseCountingType
  type: string
- description: Number of licenses managed by the license configuration.
  name: LicenseCount
  type: integer
- description: Number of available licenses as a hard limit.
  name: LicenseCountHardLimit
  type: boolean
- description: Number of licenses consumed by the license configuration.
  name: ConsumedLicenses
  type: integer
- description: Status of the license configuration.
  name: Status
  type: string
provider_name: Amazon License Manager
provider_slug: amazon-license-manager
schema_file: json-schema/amazon-license-manager-license-configuration-schema.json
slug: amazon-license-manager-license-configuration
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-license-manager/refs/heads/main/json-schema/amazon-license-manager-license-configuration-schema.json\",\n  \"title\": \"LicenseConfiguration\",\n  \"description\": \"An AWS License Manager license configuration.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"LicenseConfigurationId\": {\n      \"type\": \"string\",\n      \"description\": \"Unique ID of the license configuration.\",\n      \"example\": \"lic-0e6b56b16c0c11111\"\n    },\n    \"LicenseConfigurationArn\": {\n      \"type\": \"string\",\n      \"description\": \"Amazon Resource Name (ARN) of the license configuration.\"\n    },\n    \"Name\": {\n      \"type\": \"string\",\n      \"description\": \"Name of the license configuration.\",\n      \"example\": \"windows-server-2022\"\n    },\n    \"LicenseCountingType\": {\n      \"type\": \"string\",\n      \"description\"\
  : \"Dimension for which the licenses are counted.\",\n      \"example\": \"vCPU\",\n      \"enum\": [\n        \"vCPU\",\n        \"Instance\",\n        \"Core\",\n        \"Socket\"\n      ]\n    },\n    \"LicenseCount\": {\n      \"type\": \"integer\",\n      \"description\": \"Number of licenses managed by the license configuration.\",\n      \"example\": 100\n    },\n    \"LicenseCountHardLimit\": {\n      \"type\": \"boolean\",\n      \"description\": \"Number of available licenses as a hard limit.\",\n      \"example\": true\n    },\n    \"ConsumedLicenses\": {\n      \"type\": \"integer\",\n      \"description\": \"Number of licenses consumed by the license configuration.\",\n      \"example\": 45\n    },\n    \"Status\": {\n      \"type\": \"string\",\n      \"description\": \"Status of the license configuration.\",\n      \"example\": \"AVAILABLE\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-license-manager/refs/heads/main/json-schema/amazon-license-manager-license-configuration-schema.json
tags:
- AWS
- Compliance
- Cost Management
- License Management
- Software Licensing
title: LicenseConfiguration
---
