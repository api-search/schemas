---
description: The association of a datashare from a producer account with a data consumer.
layout: schema
name: DataShareAssociation
properties_list:
- description: ''
  name: ConsumerIdentifier
  type: object
- description: ''
  name: Status
  type: object
- description: ''
  name: ConsumerRegion
  type: object
- description: ''
  name: CreatedDate
  type: object
- description: ''
  name: StatusChangeDate
  type: object
provider_name: AWS Redshift
provider_slug: aws-redshift
schema_file: json-schema/redshift-data-share-association-schema.json
slug: redshift-data-share-association
source_filename: redshift-data-share-association-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"ConsumerIdentifier\": {},\n    \"Status\": {},\n    \"ConsumerRegion\": {},\n    \"CreatedDate\": {},\n    \"StatusChangeDate\": {}\n  },\n  \"description\": \"The association of a datashare from a producer account with a data consumer. \",\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/aws-redshift/refs/heads/main/json-schema/redshift-data-share-association-schema.json\",\n  \"title\": \"DataShareAssociation\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-redshift/refs/heads/main/json-schema/redshift-data-share-association-schema.json
tags:
- Analytics
- Big Data
- Cloud Database
- Data Warehouse
- SQL
title: DataShareAssociation
---
