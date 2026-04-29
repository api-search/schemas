---
description: A boot disk image for launching compute instances. Images can be platform images provided by Oracle, custom images, or Marketplace partner images.
layout: schema
name: Image
properties_list:
- description: The OCID of the image
  name: id
  type: string
- description: The OCID of the compartment containing the image
  name: compartmentId
  type: string
- description: A user-friendly name for the image. It does not have to be unique, and it is changeable.
  name: displayName
  type: string
- description: The image operating system (e.g., Oracle Linux)
  name: operatingSystem
  type: string
- description: The image operating system version (e.g., 8, 9)
  name: operatingSystemVersion
  type: string
- description: The date and time the image was created
  name: timeCreated
  type: string
- description: The OCID of the image originally used to create this custom image
  name: baseImageId
  type: string
- description: The boot volume size for an instance launched from this image, in MBs
  name: sizeInMBs
  type: integer
- description: The billable size of the image in GBs
  name: billableSizeInGBs
  type: integer
- description: Whether instances launched from this image can be used to create new images
  name: createImageAllowed
  type: boolean
- description: Oracle Cloud Agent features supported on the image
  name: agentFeatures
  type: object
- description: The launch mode of instances created from this image
  name: launchMode
  type: string
- description: The listing type of the image
  name: listingType
  type: string
provider_name: Oracle
provider_slug: oracle
schema_file: json-schema/oci-compute-image-schema.json
slug: oci-compute-image
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Image\",\n  \"type\": \"object\",\n  \"description\": \"A boot disk image for launching compute instances. Images can be platform images provided by Oracle, custom images, or Marketplace partner images.\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"The OCID of the image\"\n    },\n    \"compartmentId\": {\n      \"type\": \"string\",\n      \"description\": \"The OCID of the compartment containing the image\"\n    },\n    \"displayName\": {\n      \"type\": \"string\",\n      \"description\": \"A user-friendly name for the image. It does not have to be unique, and it is changeable.\"\n    },\n    \"operatingSystem\": {\n      \"type\": \"string\",\n      \"description\": \"The image operating system (e.g., Oracle Linux)\"\n    },\n    \"operatingSystemVersion\": {\n      \"type\": \"string\",\n      \"description\": \"The image operating system\
  \ version (e.g., 8, 9)\"\n    },\n    \"timeCreated\": {\n      \"type\": \"string\",\n      \"description\": \"The date and time the image was created\"\n    },\n    \"baseImageId\": {\n      \"type\": \"string\",\n      \"description\": \"The OCID of the image originally used to create this custom image\"\n    },\n    \"sizeInMBs\": {\n      \"type\": \"integer\",\n      \"description\": \"The boot volume size for an instance launched from this image, in MBs\"\n    },\n    \"billableSizeInGBs\": {\n      \"type\": \"integer\",\n      \"description\": \"The billable size of the image in GBs\"\n    },\n    \"createImageAllowed\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether instances launched from this image can be used to create new images\"\n    },\n    \"agentFeatures\": {\n      \"type\": \"object\",\n      \"description\": \"Oracle Cloud Agent features supported on the image\"\n    },\n    \"launchMode\": {\n      \"type\": \"string\",\n      \"description\":\
  \ \"The launch mode of instances created from this image\"\n    },\n    \"listingType\": {\n      \"type\": \"string\",\n      \"description\": \"The listing type of the image\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/oracle/refs/heads/main/json-schema/oci-compute-image-schema.json
tags:
- Cloud
- Database
- Enterprise
- Infrastructure
- SaaS
title: Image
---
