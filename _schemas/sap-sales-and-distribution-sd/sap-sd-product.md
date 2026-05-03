---
description: Schema for SAP S/4HANA Product entity (A_Product) from the API_PRODUCT_SRV OData service. Represents a material master record used across procurement, manufacturing, and sales processes.
layout: schema
name: SAP Product (Material Master)
properties_list:
- description: Material number
  name: Product
  type: string
- description: Material type (FERT=Finished Product, HALB=Semi-Finished, ROH=Raw Material, HAWA=Trading Goods)
  name: ProductType
  type: string
- description: Material group
  name: ProductGroup
  type: string
- description: Base unit of measure
  name: BaseUnit
  type: string
- description: Gross weight
  name: GrossWeight
  type: string
- description: Net weight
  name: NetWeight
  type: string
- description: Weight unit
  name: WeightUnit
  type: string
- description: Volume
  name: Volume
  type: string
- description: Volume unit
  name: VolumeUnit
  type: string
- description: Division
  name: Division
  type: string
- description: EAN/UPC code
  name: IndustryStandardName
  type: string
- description: Global Trade Item Number (GTIN)
  name: ProductStandardID
  type: string
- description: Creation date
  name: CreationDate
  type: string
- description: Date of last change
  name: LastChangeDate
  type: string
- description: Deletion flag
  name: IsMarkedForDeletion
  type: boolean
- description: Size/dimensions text
  name: SizeOrDimensionText
  type: string
provider_name: SAP Sales and Distribution (SD)
provider_slug: sap-sales-and-distribution-sd
schema_file: json-schema/sap-sd-product-schema.json
slug: sap-sd-product
source_filename: sap-sd-product-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://api.sap.com/schemas/sap-sd-product\",\n  \"title\": \"SAP Product (Material Master)\",\n  \"description\": \"Schema for SAP S/4HANA Product entity (A_Product) from the API_PRODUCT_SRV OData service. Represents a material master record used across procurement, manufacturing, and sales processes.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Product\": {\n      \"type\": \"string\",\n      \"maxLength\": 40,\n      \"description\": \"Material number\"\n    },\n    \"ProductType\": {\n      \"type\": \"string\",\n      \"maxLength\": 4,\n      \"description\": \"Material type (FERT=Finished Product, HALB=Semi-Finished, ROH=Raw Material, HAWA=Trading Goods)\"\n    },\n    \"ProductGroup\": {\n      \"type\": \"string\",\n      \"maxLength\": 9,\n      \"description\": \"Material group\"\n    },\n    \"BaseUnit\": {\n      \"type\": \"string\",\n      \"maxLength\": 3,\n      \"description\"\
  : \"Base unit of measure\"\n    },\n    \"GrossWeight\": {\n      \"type\": \"string\",\n      \"description\": \"Gross weight\"\n    },\n    \"NetWeight\": {\n      \"type\": \"string\",\n      \"description\": \"Net weight\"\n    },\n    \"WeightUnit\": {\n      \"type\": \"string\",\n      \"maxLength\": 3,\n      \"description\": \"Weight unit\"\n    },\n    \"Volume\": {\n      \"type\": \"string\",\n      \"description\": \"Volume\"\n    },\n    \"VolumeUnit\": {\n      \"type\": \"string\",\n      \"maxLength\": 3,\n      \"description\": \"Volume unit\"\n    },\n    \"Division\": {\n      \"type\": \"string\",\n      \"maxLength\": 2,\n      \"description\": \"Division\"\n    },\n    \"IndustryStandardName\": {\n      \"type\": \"string\",\n      \"maxLength\": 18,\n      \"description\": \"EAN/UPC code\"\n    },\n    \"ProductStandardID\": {\n      \"type\": \"string\",\n      \"maxLength\": 18,\n      \"description\": \"Global Trade Item Number (GTIN)\"\n    },\n    \"CreationDate\"\
  : {\n      \"type\": \"string\",\n      \"format\": \"date\",\n      \"description\": \"Creation date\"\n    },\n    \"LastChangeDate\": {\n      \"type\": \"string\",\n      \"format\": \"date\",\n      \"description\": \"Date of last change\"\n    },\n    \"IsMarkedForDeletion\": {\n      \"type\": \"boolean\",\n      \"description\": \"Deletion flag\"\n    },\n    \"SizeOrDimensionText\": {\n      \"type\": \"string\",\n      \"maxLength\": 32,\n      \"description\": \"Size/dimensions text\"\n    }\n  },\n  \"required\": [\"Product\"]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/sap-sales-and-distribution-sd/refs/heads/main/json-schema/sap-sd-product-schema.json
tags:
- Distribution
- ERP
- OData
- S/4HANA
- Sales
- SAP
title: SAP Product (Material Master)
---
