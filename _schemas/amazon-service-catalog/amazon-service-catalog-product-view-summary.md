---
description: Summary information about a product view.
layout: schema
name: ProductViewSummary
properties_list:
- description: The product view identifier.
  name: Id
  type: string
- description: The product identifier.
  name: ProductId
  type: string
- description: The name of the product.
  name: Name
  type: string
- description: The owner of the product.
  name: Owner
  type: string
- description: Short description of the product.
  name: ShortDescription
  type: string
- description: The product type.
  name: Type
  type: string
provider_name: Amazon Service Catalog
provider_slug: amazon-service-catalog
schema_file: json-schema/amazon-service-catalog-product-view-summary-schema.json
slug: amazon-service-catalog-product-view-summary
source_filename: amazon-service-catalog-product-view-summary-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-service-catalog/refs/heads/main/json-schema/amazon-service-catalog-product-view-summary-schema.json\",\n  \"title\": \"ProductViewSummary\",\n  \"description\": \"Summary information about a product view.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Id\": {\n      \"type\": \"string\",\n      \"description\": \"The product view identifier.\",\n      \"example\": \"prodview-a1b2c3\"\n    },\n    \"ProductId\": {\n      \"type\": \"string\",\n      \"description\": \"The product identifier.\",\n      \"example\": \"prod-a1b2c3\"\n    },\n    \"Name\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the product.\",\n      \"example\": \"EC2 Instance\"\n    },\n    \"Owner\": {\n      \"type\": \"string\",\n      \"description\": \"The owner of the product.\",\n      \"example\": \"IT Team\"\n    },\n    \"ShortDescription\"\
  : {\n      \"type\": \"string\",\n      \"description\": \"Short description of the product.\"\n    },\n    \"Type\": {\n      \"type\": \"string\",\n      \"description\": \"The product type.\",\n      \"enum\": [\n        \"CLOUD_FORMATION_TEMPLATE\",\n        \"MARKETPLACE\",\n        \"TERRAFORM_OPEN_SOURCE\",\n        \"TERRAFORM_CLOUD\",\n        \"EXTERNAL\"\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-service-catalog/refs/heads/main/json-schema/amazon-service-catalog-product-view-summary-schema.json
tags:
- AWS
- Cloud Governance
- Compliance
- IT Governance
- Service Catalog
title: ProductViewSummary
---
