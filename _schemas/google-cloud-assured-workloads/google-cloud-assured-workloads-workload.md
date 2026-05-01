---
description: Schema for an Assured Workloads workload, representing a compliance-controlled environment on Google Cloud.
layout: schema
name: Google Cloud Assured Workloads Workload
properties_list:
- description: The resource name of the workload
  name: name
  type: string
- description: User-assigned display name of the workload
  name: displayName
  type: string
- description: The compliance regime for the workload
  name: complianceRegime
  type: string
- description: The billing account associated with the workload
  name: billingAccount
  type: string
- description: Labels applied to the workload
  name: labels
  type: object
- description: The parent of the folder where resources are provisioned
  name: provisionedResourcesParent
  type: string
- description: Resources associated with the workload
  name: resources
  type: array
- description: The creation time of the workload
  name: createTime
  type: string
- description: Services that are compliant but not allowed for the workload
  name: compliantButDisallowedServices
  type: array
provider_name: Google Cloud Assured Workloads
provider_slug: google-cloud-assured-workloads
schema_file: json-schema/google-cloud-assured-workloads-workload-schema.json
slug: google-cloud-assured-workloads-workload
source_filename: google-cloud-assured-workloads-workload-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://cloud.google.com/schemas/assuredworkloads/workload.json\",\n  \"title\": \"Google Cloud Assured Workloads Workload\",\n  \"description\": \"Schema for an Assured Workloads workload, representing a compliance-controlled environment on Google Cloud.\",\n  \"type\": \"object\",\n  \"required\": [\"displayName\", \"complianceRegime\"],\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The resource name of the workload\"\n    },\n    \"displayName\": {\n      \"type\": \"string\",\n      \"description\": \"User-assigned display name of the workload\"\n    },\n    \"complianceRegime\": {\n      \"type\": \"string\",\n      \"description\": \"The compliance regime for the workload\",\n      \"enum\": [\n        \"FEDRAMP_HIGH\",\n        \"FEDRAMP_MODERATE\",\n        \"HIPAA\",\n        \"HITRUST\",\n        \"CJIS\",\n        \"IL4\",\n        \"IL5\"\
  ,\n        \"ITAR\",\n        \"EU_REGIONS_AND_SUPPORT\",\n        \"CA_REGIONS_AND_SUPPORT\",\n        \"AU_REGIONS_AND_US_SUPPORT\"\n      ]\n    },\n    \"billingAccount\": {\n      \"type\": \"string\",\n      \"description\": \"The billing account associated with the workload\"\n    },\n    \"labels\": {\n      \"type\": \"object\",\n      \"description\": \"Labels applied to the workload\",\n      \"additionalProperties\": {\n        \"type\": \"string\"\n      }\n    },\n    \"provisionedResourcesParent\": {\n      \"type\": \"string\",\n      \"description\": \"The parent of the folder where resources are provisioned\"\n    },\n    \"resources\": {\n      \"type\": \"array\",\n      \"description\": \"Resources associated with the workload\",\n      \"items\": {\n        \"$ref\": \"#/$defs/Resource\"\n      }\n    },\n    \"createTime\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"The creation time of the workload\"\n    },\n    \"\
  compliantButDisallowedServices\": {\n      \"type\": \"array\",\n      \"description\": \"Services that are compliant but not allowed for the workload\",\n      \"items\": {\n        \"type\": \"string\"\n      }\n    }\n  },\n  \"$defs\": {\n    \"Resource\": {\n      \"type\": \"object\",\n      \"description\": \"A resource associated with the workload\",\n      \"properties\": {\n        \"resourceId\": {\n          \"type\": \"integer\",\n          \"description\": \"The numeric identifier of the resource\"\n        },\n        \"resourceType\": {\n          \"type\": \"string\",\n          \"description\": \"The type of the resource\",\n          \"enum\": [\"CONSUMER_PROJECT\", \"CONSUMER_FOLDER\", \"ENCRYPTION_KEYS_PROJECT\", \"KEYRING\"]\n        }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/google-cloud-assured-workloads/refs/heads/main/json-schema/google-cloud-assured-workloads-workload-schema.json
tags:
- Compliance
- Data Residency
- FedRAMP
- Governance
- HIPAA
- Regulatory
title: Google Cloud Assured Workloads Workload
---
