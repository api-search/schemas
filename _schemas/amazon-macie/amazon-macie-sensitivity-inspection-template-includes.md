---
description: Specifies the allow lists, custom data identifiers, and managed data identifiers to include (use) when performing automated sensitive data discovery for an Amazon Macie account. The configuration must specify at least one custom data identifier or managed data identifier. For information about the managed data identifiers that Amazon Macie currently provides, see <a href="https://docs.aws.amazon.com/macie/latest/user/managed-data-identifiers.html">Using managed data identifiers</a> in the <i>Amazon Macie User Guide</i>.
layout: schema
name: SensitivityInspectionTemplateIncludes
properties_list:
- description: ''
  name: allowListIds
  type: object
- description: ''
  name: customDataIdentifierIds
  type: object
- description: ''
  name: managedDataIdentifierIds
  type: object
provider_name: Amazon Macie
provider_slug: amazon-macie
schema_file: json-schema/amazon-macie-sensitivity-inspection-template-includes-schema.json
slug: amazon-macie-sensitivity-inspection-template-includes
source_filename: amazon-macie-sensitivity-inspection-template-includes-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-macie/refs/heads/main/json-schema/amazon-macie-sensitivity-inspection-template-includes-schema.json\",\n  \"title\": \"SensitivityInspectionTemplateIncludes\",\n  \"description\": \"Specifies the allow lists, custom data identifiers, and managed data identifiers to include (use) when performing automated sensitive data discovery for an Amazon Macie account. The configuration must specify at least one custom data identifier or managed data identifier. For information about the managed data identifiers that Amazon Macie currently provides, see <a href=\\\"https://docs.aws.amazon.com/macie/latest/user/managed-data-identifiers.html\\\">Using managed data identifiers</a> in the <i>Amazon Macie User Guide</i>.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"allowListIds\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__listOf__string\"\
  \n        },\n        {\n          \"description\": \"An array of unique identifiers, one for each allow list to include.\"\n        }\n      ]\n    },\n    \"customDataIdentifierIds\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__listOf__string\"\n        },\n        {\n          \"description\": \"An array of unique identifiers, one for each custom data identifier to include.\"\n        }\n      ]\n    },\n    \"managedDataIdentifierIds\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__listOf__string\"\n        },\n        {\n          \"description\": \"<p>An array of unique identifiers, one for each managed data identifier to include.</p> <p>Amazon Macie uses these managed data identifiers in addition to managed data identifiers that are subsequently released and recommended for automated sensitive data discovery. To retrieve a list of valid values for the managed data identifiers that are currently available, use the\
  \ ListManagedDataIdentifiers operation.</p> <para/>\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-macie/refs/heads/main/json-schema/amazon-macie-sensitivity-inspection-template-includes-schema.json
tags:
- AWS
- Data Security
- Sensitive Data
- Privacy
- Compliance
- Machine Learning
- S3
title: SensitivityInspectionTemplateIncludes
---
