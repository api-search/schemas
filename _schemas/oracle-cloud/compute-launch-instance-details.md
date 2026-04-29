---
description: Details for launching a new compute instance.
layout: schema
name: LaunchInstanceDetails
properties_list:
- description: The OCID of the compartment.
  name: compartmentId
  type: string
- description: The availability domain.
  name: availabilityDomain
  type: string
- description: The shape of the instance.
  name: shape
  type: string
- description: A user-friendly name.
  name: displayName
  type: string
- description: The OCID of the image to use.
  name: imageId
  type: string
- description: The OCID of the subnet.
  name: subnetId
  type: string
- description: Configuration for flexible shapes.
  name: shapeConfig
  type: object
- description: ''
  name: freeformTags
  type: object
provider_name: Oracle Cloud Infrastructure
provider_slug: oracle-cloud
schema_file: json-schema/compute-launch-instance-details-schema.json
slug: compute-launch-instance-details
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/oracle-cloud/refs/heads/main/json-schema/compute-launch-instance-details-schema.json\",\n  \"title\": \"LaunchInstanceDetails\",\n  \"description\": \"Details for launching a new compute instance.\",\n  \"type\": \"object\",\n  \"required\": [\n    \"compartmentId\",\n    \"shape\",\n    \"availabilityDomain\"\n  ],\n  \"properties\": {\n    \"compartmentId\": {\n      \"type\": \"string\",\n      \"description\": \"The OCID of the compartment.\",\n      \"example\": \"ocid1.compartment.oc1..abcdefg123456\"\n    },\n    \"availabilityDomain\": {\n      \"type\": \"string\",\n      \"description\": \"The availability domain.\",\n      \"example\": \"Uocm:US-ASHBURN-AD-1\"\n    },\n    \"shape\": {\n      \"type\": \"string\",\n      \"description\": \"The shape of the instance.\",\n      \"example\": \"VM.Standard.E4.Flex\"\n    },\n    \"displayName\"\
  : {\n      \"type\": \"string\",\n      \"description\": \"A user-friendly name.\",\n      \"example\": \"my-new-instance\"\n    },\n    \"imageId\": {\n      \"type\": \"string\",\n      \"description\": \"The OCID of the image to use.\",\n      \"example\": \"ocid1.image.oc1.iad.abcdefg123456\"\n    },\n    \"subnetId\": {\n      \"type\": \"string\",\n      \"description\": \"The OCID of the subnet.\",\n      \"example\": \"ocid1.subnet.oc1.iad.abcdefg123456\"\n    },\n    \"shapeConfig\": {\n      \"type\": \"object\",\n      \"description\": \"Configuration for flexible shapes.\",\n      \"example\": {\n        \"ocpus\": 2.0,\n        \"memoryInGBs\": 16.0\n      }\n    },\n    \"freeformTags\": {\n      \"type\": \"object\",\n      \"example\": {\n        \"key1\": \"value1\"\n      },\n      \"additionalProperties\": {\n        \"type\": \"string\"\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/oracle-cloud/refs/heads/main/json-schema/compute-launch-instance-details-schema.json
tags:
- Cloud Computing
- Enterprise Cloud
- Infrastructure as a Service
- Oracle
- Platform as a Service
title: LaunchInstanceDetails
---
