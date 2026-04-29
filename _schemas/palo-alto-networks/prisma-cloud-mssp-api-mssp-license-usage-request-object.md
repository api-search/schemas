---
description: 'MsspLicenseUsageRequestObject schema from Prisma Cloud: Managed Security Service Provider (MSSP)'
layout: schema
name: MsspLicenseUsageRequestObject
properties_list:
- description: ''
  name: tenantGroupId
  type: string
- description: ''
  name: licensePoolId
  type: string
- description: ''
  name: timeRange
  type: object
- description: ''
  name: nextPageToken
  type: string
provider_name: Palo Alto Networks
provider_slug: palo-alto-networks
schema_file: json-schema/prisma-cloud-mssp-api-mssp-license-usage-request-object-schema.json
slug: prisma-cloud-mssp-api-mssp-license-usage-request-object
source_filename: prisma-cloud-mssp-api-mssp-license-usage-request-object-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"MsspLicenseUsageRequestObject\",\n  \"description\": \"MsspLicenseUsageRequestObject schema from Prisma Cloud: Managed Security Service Provider (MSSP)\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/prisma-cloud-mssp-api-mssp-license-usage-request-object-schema.json\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"tenantGroupId\": {\n      \"type\": \"string\"\n    },\n    \"licensePoolId\": {\n      \"type\": \"string\"\n    },\n    \"timeRange\": {\n      \"oneOf\": [\n        {\n          \"type\": \"object\",\n          \"allOf\": [\n            {\n              \"type\": \"object\",\n              \"properties\": {\n                \"type\": {\n                  \"type\": \"string\"\n                },\n                \"timeUnit\": {\n                  \"type\": \"string\"\n                },\n                \"timeValue\"\
  : {\n                  \"type\": \"integer\",\n                  \"format\": \"int32\"\n                }\n              },\n              \"discriminator\": {\n                \"propertyName\": \"type\"\n              }\n            },\n            {\n              \"type\": \"object\",\n              \"properties\": {\n                \"value\": {\n                  \"type\": \"object\",\n                  \"properties\": {\n                    \"unit\": {\n                      \"type\": \"string\",\n                      \"enum\": [\n                        \"week\",\n                        \"month\",\n                        \"year\"\n                      ]\n                    },\n                    \"amount\": {\n                      \"type\": \"integer\",\n                      \"description\": \"Number of time units\",\n                      \"format\": \"int32\"\n                    }\n                  }\n                }\n              }\n            }\n          ]\n \
  \       },\n        {\n          \"type\": \"object\",\n          \"allOf\": [\n            {\n              \"type\": \"object\",\n              \"properties\": {\n                \"type\": {\n                  \"type\": \"string\"\n                },\n                \"timeUnit\": {\n                  \"type\": \"string\"\n                },\n                \"timeValue\": {\n                  \"type\": \"integer\",\n                  \"format\": \"int32\"\n                }\n              },\n              \"discriminator\": {\n                \"propertyName\": \"type\"\n              }\n            },\n            {\n              \"type\": \"object\",\n              \"properties\": {\n                \"value\": {\n                  \"type\": \"string\",\n                  \"enum\": [\n                    \"week\",\n                    \"month\",\n                    \"year\"\n                  ]\n                }\n              }\n            }\n          ]\n        }\n      ]\n\
  \    },\n    \"nextPageToken\": {\n      \"type\": \"string\"\n    }\n  },\n  \"required\": [\n    \"licensePoolId\"\n  ]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/prisma-cloud-mssp-api-mssp-license-usage-request-object-schema.json
tags:
- Cloud Security
- Cybersecurity
- Firewall
- Network Security
- SASE
- SOAR
- Threat Intelligence
- XDR
title: MsspLicenseUsageRequestObject
---
