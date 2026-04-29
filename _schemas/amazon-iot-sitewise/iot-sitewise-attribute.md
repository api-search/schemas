---
description: Contains an asset attribute property. For more information, see <a href="https://docs.aws.amazon.com/iot-sitewise/latest/userguide/asset-properties.html#attributes">Attributes</a> in the <i>IoT SiteWise User Guide</i>.
layout: schema
name: Attribute
properties_list:
- description: ''
  name: defaultValue
  type: object
provider_name: Amazon IoT SiteWise
provider_slug: amazon-iot-sitewise
schema_file: json-schema/iot-sitewise-attribute-schema.json
slug: iot-sitewise-attribute
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iot-sitewise/refs/heads/main/json-schema/iot-sitewise-attribute-schema.json\",\n  \"title\": \"Attribute\",\n  \"description\": \"Contains an asset attribute property. For more information, see <a href=\\\"https://docs.aws.amazon.com/iot-sitewise/latest/userguide/asset-properties.html#attributes\\\">Attributes</a> in the <i>IoT SiteWise User Guide</i>.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"defaultValue\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DefaultValue\"\n        },\n        {\n          \"description\": \"The default value of the asset model property attribute. All assets that you create from the asset model contain this attribute value. You can update an attribute's value after you create an asset. For more information, see <a href=\\\"https://docs.aws.amazon.com/iot-sitewise/latest/userguide/update-attribute-values.html\\\
  \">Updating attribute values</a> in the <i>IoT SiteWise User Guide</i>.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iot-sitewise/refs/heads/main/json-schema/iot-sitewise-attribute-schema.json
tags:
- AWS
- Asset Management
- Industrial IoT
- IoT
- Time Series Data
title: Attribute
---
