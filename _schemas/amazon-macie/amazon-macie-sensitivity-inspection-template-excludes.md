---
description: Specifies managed data identifiers to exclude (not use) when performing automated sensitive data discovery for an Amazon Macie account. For information about the managed data identifiers that Amazon Macie currently provides, see <a href="https://docs.aws.amazon.com/macie/latest/user/managed-data-identifiers.html">Using managed data identifiers</a> in the <i>Amazon Macie User Guide</i>.
layout: schema
name: SensitivityInspectionTemplateExcludes
properties_list:
- description: ''
  name: managedDataIdentifierIds
  type: object
provider_name: Amazon Macie
provider_slug: amazon-macie
schema_file: json-schema/amazon-macie-sensitivity-inspection-template-excludes-schema.json
slug: amazon-macie-sensitivity-inspection-template-excludes
source_filename: amazon-macie-sensitivity-inspection-template-excludes-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-macie/refs/heads/main/json-schema/amazon-macie-sensitivity-inspection-template-excludes-schema.json\",\n  \"title\": \"SensitivityInspectionTemplateExcludes\",\n  \"description\": \"Specifies managed data identifiers to exclude (not use) when performing automated sensitive data discovery for an Amazon Macie account. For information about the managed data identifiers that Amazon Macie currently provides, see <a href=\\\"https://docs.aws.amazon.com/macie/latest/user/managed-data-identifiers.html\\\">Using managed data identifiers</a> in the <i>Amazon Macie User Guide</i>.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"managedDataIdentifierIds\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__listOf__string\"\n        },\n        {\n          \"description\": \"An array of unique identifiers, one for\
  \ each managed data identifier to exclude. To retrieve a list of valid values, use the ListManagedDataIdentifiers operation.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-macie/refs/heads/main/json-schema/amazon-macie-sensitivity-inspection-template-excludes-schema.json
tags:
- AWS
- Data Security
- Sensitive Data
- Privacy
- Compliance
- Machine Learning
- S3
title: SensitivityInspectionTemplateExcludes
---
