---
description: A compute instance running in Oracle Cloud Infrastructure.
layout: schema
name: Instance
properties_list:
- description: The OCID of the instance.
  name: id
  type: string
- description: The OCID of the compartment.
  name: compartmentId
  type: string
- description: The availability domain the instance is running in.
  name: availabilityDomain
  type: string
- description: A user-friendly name.
  name: displayName
  type: string
- description: The shape of the instance.
  name: shape
  type: string
- description: The current state of the instance.
  name: lifecycleState
  type: string
- description: The region that contains the availability domain.
  name: region
  type: string
- description: The OCID of the image used to boot the instance.
  name: imageId
  type: string
- description: The date and time the instance was created.
  name: timeCreated
  type: string
- description: Free-form tags for the instance.
  name: freeformTags
  type: object
- description: Defined tags for the instance.
  name: definedTags
  type: object
provider_name: Oracle Cloud Infrastructure
provider_slug: oracle-cloud
schema_file: json-schema/compute-instance-schema.json
slug: compute-instance
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/oracle-cloud/refs/heads/main/json-schema/compute-instance-schema.json\",\n  \"title\": \"Instance\",\n  \"description\": \"A compute instance running in Oracle Cloud Infrastructure.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"The OCID of the instance.\",\n      \"example\": \"ocid1.instance.oc1.iad.abcdefg123456\"\n    },\n    \"compartmentId\": {\n      \"type\": \"string\",\n      \"description\": \"The OCID of the compartment.\",\n      \"example\": \"ocid1.compartment.oc1..abcdefg123456\"\n    },\n    \"availabilityDomain\": {\n      \"type\": \"string\",\n      \"description\": \"The availability domain the instance is running in.\",\n      \"example\": \"Uocm:US-ASHBURN-AD-1\"\n    },\n    \"displayName\": {\n      \"type\": \"string\",\n      \"description\": \"A user-friendly\
  \ name.\",\n      \"example\": \"my-instance-01\"\n    },\n    \"shape\": {\n      \"type\": \"string\",\n      \"description\": \"The shape of the instance.\",\n      \"example\": \"VM.Standard.E4.Flex\"\n    },\n    \"lifecycleState\": {\n      \"type\": \"string\",\n      \"description\": \"The current state of the instance.\",\n      \"enum\": \"['PROVISIONING', 'RUNNING', 'STARTING', 'STOPPING', 'STOPPED', 'CREATING_IMAGE', 'TERMINATING', 'TERMINATED']\",\n      \"example\": \"RUNNING\"\n    },\n    \"region\": {\n      \"type\": \"string\",\n      \"description\": \"The region that contains the availability domain.\",\n      \"example\": \"us-ashburn-1\"\n    },\n    \"imageId\": {\n      \"type\": \"string\",\n      \"description\": \"The OCID of the image used to boot the instance.\",\n      \"example\": \"ocid1.image.oc1.iad.abcdefg123456\"\n    },\n    \"timeCreated\": {\n      \"type\": \"string\",\n      \"description\": \"The date and time the instance was created.\",\n  \
  \    \"format\": \"date-time\",\n      \"example\": \"2026-01-15T10:30:00Z\"\n    },\n    \"freeformTags\": {\n      \"type\": \"object\",\n      \"description\": \"Free-form tags for the instance.\",\n      \"example\": {\n        \"key1\": \"value1\"\n      },\n      \"additionalProperties\": {\n        \"type\": \"string\"\n      }\n    },\n    \"definedTags\": {\n      \"type\": \"object\",\n      \"description\": \"Defined tags for the instance.\",\n      \"example\": {\n        \"key1\": \"value1\"\n      },\n      \"additionalProperties\": {\n        \"type\": \"object\"\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/oracle-cloud/refs/heads/main/json-schema/compute-instance-schema.json
tags:
- Cloud Computing
- Enterprise Cloud
- Infrastructure as a Service
- Oracle
- Platform as a Service
title: Instance
---
