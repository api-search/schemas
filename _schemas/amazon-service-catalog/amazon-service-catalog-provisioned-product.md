---
description: Information about a provisioned product.
layout: schema
name: ProvisionedProduct
properties_list:
- description: ''
  name: RecordDetail
  type: object
provider_name: Amazon Service Catalog
provider_slug: amazon-service-catalog
schema_file: json-schema/amazon-service-catalog-provisioned-product-schema.json
slug: amazon-service-catalog-provisioned-product
source_filename: amazon-service-catalog-provisioned-product-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-service-catalog/refs/heads/main/json-schema/amazon-service-catalog-provisioned-product-schema.json\",\n  \"title\": \"ProvisionedProduct\",\n  \"description\": \"Information about a provisioned product.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"RecordDetail\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"RecordId\": {\n          \"type\": \"string\",\n          \"description\": \"The identifier of the record.\",\n          \"example\": \"rec-a1b2c3d4\"\n        },\n        \"ProvisionedProductName\": {\n          \"type\": \"string\",\n          \"description\": \"The user-friendly name of the provisioned product.\",\n          \"example\": \"my-ec2-instance\"\n        },\n        \"Status\": {\n          \"type\": \"string\",\n          \"description\": \"The status of the provisioned product.\",\n   \
  \       \"enum\": [\n            \"CREATED\",\n            \"IN_PROGRESS\",\n            \"IN_PROGRESS_IN_ERROR\",\n            \"SUCCEEDED\",\n            \"FAILED\"\n          ]\n        },\n        \"ProvisionedProductId\": {\n          \"type\": \"string\",\n          \"description\": \"The identifier of the provisioned product.\"\n        }\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-service-catalog/refs/heads/main/json-schema/amazon-service-catalog-provisioned-product-schema.json
tags:
- Cloud Governance
- Compliance
- IT Governance
- Service Catalog
title: ProvisionedProduct
---
