---
description: Details for importing an image from Object Storage
layout: schema
name: ImageSourceDetails
properties_list:
- description: The source type for the image
  name: sourceType
  type: string
- description: The Object Storage bucket name (for objectStorageTuple)
  name: bucketName
  type: string
- description: The Object Storage namespace (for objectStorageTuple)
  name: namespaceName
  type: string
- description: The Object Storage object name (for objectStorageTuple)
  name: objectName
  type: string
- description: The Object Storage URL for the image (for objectStorageUri source type)
  name: sourceUri
  type: string
- description: The format of the image to import
  name: sourceImageType
  type: string
- description: The operating system of the image
  name: operatingSystem
  type: string
- description: The operating system version of the image
  name: operatingSystemVersion
  type: string
provider_name: Oracle
provider_slug: oracle
schema_file: json-schema/oci-compute-image-source-details-schema.json
slug: oci-compute-image-source-details
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ImageSourceDetails\",\n  \"type\": \"object\",\n  \"description\": \"Details for importing an image from Object Storage\",\n  \"properties\": {\n    \"sourceType\": {\n      \"type\": \"string\",\n      \"description\": \"The source type for the image\"\n    },\n    \"bucketName\": {\n      \"type\": \"string\",\n      \"description\": \"The Object Storage bucket name (for objectStorageTuple)\"\n    },\n    \"namespaceName\": {\n      \"type\": \"string\",\n      \"description\": \"The Object Storage namespace (for objectStorageTuple)\"\n    },\n    \"objectName\": {\n      \"type\": \"string\",\n      \"description\": \"The Object Storage object name (for objectStorageTuple)\"\n    },\n    \"sourceUri\": {\n      \"type\": \"string\",\n      \"description\": \"The Object Storage URL for the image (for objectStorageUri source type)\"\n    },\n    \"sourceImageType\": {\n      \"type\": \"string\"\
  ,\n      \"description\": \"The format of the image to import\"\n    },\n    \"operatingSystem\": {\n      \"type\": \"string\",\n      \"description\": \"The operating system of the image\"\n    },\n    \"operatingSystemVersion\": {\n      \"type\": \"string\",\n      \"description\": \"The operating system version of the image\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/oracle/refs/heads/main/json-schema/oci-compute-image-source-details-schema.json
tags:
- Cloud
- Database
- Enterprise
- Infrastructure
- SaaS
title: ImageSourceDetails
---
