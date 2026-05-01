---
description: Specifies a property-based filter condition that determines which Amazon Web Services resources are included or excluded from the query results.
layout: schema
name: SearchResourcesSimpleCriterion
properties_list:
- description: ''
  name: comparator
  type: object
- description: ''
  name: key
  type: object
- description: ''
  name: values
  type: object
provider_name: Amazon Macie
provider_slug: amazon-macie
schema_file: json-schema/amazon-macie-search-resources-simple-criterion-schema.json
slug: amazon-macie-search-resources-simple-criterion
source_filename: amazon-macie-search-resources-simple-criterion-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-macie/refs/heads/main/json-schema/amazon-macie-search-resources-simple-criterion-schema.json\",\n  \"title\": \"SearchResourcesSimpleCriterion\",\n  \"description\": \"Specifies a property-based filter condition that determines which Amazon Web Services resources are included or excluded from the query results.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"comparator\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SearchResourcesComparator\"\n        },\n        {\n          \"description\": \"The operator to use in the condition. Valid values are EQ (equals) and NE (not equals).\"\n        }\n      ]\n    },\n    \"key\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SearchResourcesSimpleCriterionKey\"\n        },\n        {\n          \"description\": \"The property\
  \ to use in the condition.\"\n        }\n      ]\n    },\n    \"values\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__listOf__string\"\n        },\n        {\n          \"description\": \"<p>An array that lists one or more values to use in the condition. If you specify multiple values, Amazon Macie uses OR logic to join the values. Valid values for each supported property (key) are:</p> <ul><li><p>ACCOUNT_ID - A string that represents the unique identifier for the Amazon Web Services account that owns the resource.</p></li> <li><p>S3_BUCKET_EFFECTIVE_PERMISSION - A string that represents an enumerated value that Macie defines for the <a href=\\\"https://docs.aws.amazon.com/macie/latest/APIReference/datasources-s3.html#datasources-s3-prop-bucketpublicaccess-effectivepermission\\\">BucketPublicAccess.effectivePermission</a> property of an S3 bucket.</p></li> <li><p>S3_BUCKET_NAME - A string that represents the name of an S3 bucket.</p></li> <li><p>S3_BUCKET_SHARED_ACCESS\
  \ - A string that represents an enumerated value that Macie defines for the <a href=\\\"https://docs.aws.amazon.com/macie/latest/APIReference/datasources-s3.html#datasources-s3-prop-bucketmetadata-sharedaccess\\\">BucketMetadata.sharedAccess</a> property of an S3 bucket.</p></li></ul> <p>Values are case sensitive. Also, Macie doesn't support use of partial values or wildcard characters in values.</p>\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-macie/refs/heads/main/json-schema/amazon-macie-search-resources-simple-criterion-schema.json
tags:
- Data Security
- Sensitive Data
- Privacy
- Compliance
- Machine Learning
- S3
title: SearchResourcesSimpleCriterion
---
