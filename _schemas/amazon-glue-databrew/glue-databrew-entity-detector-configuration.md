---
description: Configuration of entity detection for a profile job. When undefined, entity detection is disabled.
layout: schema
name: EntityDetectorConfiguration
properties_list:
- description: ''
  name: EntityTypes
  type: object
- description: ''
  name: AllowedStatistics
  type: object
provider_name: Amazon Glue DataBrew
provider_slug: amazon-glue-databrew
schema_file: json-schema/glue-databrew-entity-detector-configuration-schema.json
slug: glue-databrew-entity-detector-configuration
source_filename: glue-databrew-entity-detector-configuration-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-glue-databrew/refs/heads/main/json-schema/glue-databrew-entity-detector-configuration-schema.json\",\n  \"title\": \"EntityDetectorConfiguration\",\n  \"description\": \"Configuration of entity detection for a profile job. When undefined, entity detection is disabled.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"EntityTypes\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/EntityTypeList\"\n        },\n        {\n          \"description\": \"<p>Entity types to detect. Can be any of the following:</p> <ul> <li> <p>USA_SSN</p> </li> <li> <p>EMAIL</p> </li> <li> <p>USA_ITIN</p> </li> <li> <p>USA_PASSPORT_NUMBER</p> </li> <li> <p>PHONE_NUMBER</p> </li> <li> <p>USA_DRIVING_LICENSE</p> </li> <li> <p>BANK_ACCOUNT</p> </li> <li> <p>CREDIT_CARD</p> </li> <li> <p>IP_ADDRESS</p> </li> <li> <p>MAC_ADDRESS</p>\
  \ </li> <li> <p>USA_DEA_NUMBER</p> </li> <li> <p>USA_HCPCS_CODE</p> </li> <li> <p>USA_NATIONAL_PROVIDER_IDENTIFIER</p> </li> <li> <p>USA_NATIONAL_DRUG_CODE</p> </li> <li> <p>USA_HEALTH_INSURANCE_CLAIM_NUMBER</p> </li> <li> <p>USA_MEDICARE_BENEFICIARY_IDENTIFIER</p> </li> <li> <p>USA_CPT_CODE</p> </li> <li> <p>PERSON_NAME</p> </li> <li> <p>DATE</p> </li> </ul> <p>The Entity type group USA_ALL is also supported, and includes all of the above entity types except PERSON_NAME and DATE.</p>\"\n        }\n      ]\n    },\n    \"AllowedStatistics\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AllowedStatisticList\"\n        },\n        {\n          \"description\": \"Configuration of statistics that are allowed to be run on columns that contain detected entities. When undefined, no statistics will be computed on columns that contain detected entities.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"EntityTypes\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-glue-databrew/refs/heads/main/json-schema/glue-databrew-entity-detector-configuration-schema.json
tags:
- Data Analytics
- Data Preparation
- ETL
- Machine Learning
title: EntityDetectorConfiguration
---
