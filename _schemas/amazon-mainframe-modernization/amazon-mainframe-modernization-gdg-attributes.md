---
description: The required attributes for a generation data group data set. A generation data set is one of a collection of successive, historically related, catalogued data sets that together are known as a generation data group (GDG). Use this structure when you want to import a GDG. For more information on GDG, see <a href="https://www.ibm.com/docs/en/zos/2.3.0?topic=guide-generation-data-sets">Generation data sets</a>.
layout: schema
name: GdgAttributes
properties_list:
- description: ''
  name: limit
  type: object
- description: ''
  name: rollDisposition
  type: object
provider_name: Amazon Mainframe Modernization
provider_slug: amazon-mainframe-modernization
schema_file: json-schema/amazon-mainframe-modernization-gdg-attributes-schema.json
slug: amazon-mainframe-modernization-gdg-attributes
source_filename: amazon-mainframe-modernization-gdg-attributes-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mainframe-modernization/refs/heads/main/json-schema/amazon-mainframe-modernization-gdg-attributes-schema.json\",\n  \"title\": \"GdgAttributes\",\n  \"description\": \"The required attributes for a generation data group data set. A generation data set is one of a collection of successive, historically related, catalogued data sets that together are known as a generation data group (GDG). Use this structure when you want to import a GDG. For more information on GDG, see <a href=\\\"https://www.ibm.com/docs/en/zos/2.3.0?topic=guide-generation-data-sets\\\">Generation data sets</a>.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"limit\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Integer\"\n        },\n        {\n          \"description\": \"The maximum number of generation data sets, up to 255, in\
  \ a GDG.\"\n        }\n      ]\n    },\n    \"rollDisposition\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"The disposition of the data set in the catalog.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mainframe-modernization/refs/heads/main/json-schema/amazon-mainframe-modernization-gdg-attributes-schema.json
tags:
- AWS
- COBOL
- Mainframe
- Migration
- Modernization
- Batch Processing
title: GdgAttributes
---
