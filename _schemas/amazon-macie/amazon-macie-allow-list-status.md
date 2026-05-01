---
description: Provides information about the current status of an allow list, which indicates whether Amazon Macie can access and use the list's criteria.
layout: schema
name: AllowListStatus
properties_list:
- description: ''
  name: code
  type: object
- description: ''
  name: description
  type: object
provider_name: Amazon Macie
provider_slug: amazon-macie
schema_file: json-schema/amazon-macie-allow-list-status-schema.json
slug: amazon-macie-allow-list-status
source_filename: amazon-macie-allow-list-status-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-macie/refs/heads/main/json-schema/amazon-macie-allow-list-status-schema.json\",\n  \"title\": \"AllowListStatus\",\n  \"description\": \"Provides information about the current status of an allow list, which indicates whether Amazon Macie can access and use the list's criteria.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"code\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AllowListStatusCode\"\n        },\n        {\n          \"description\": \"<p>The current status of the allow list. If the list's criteria specify a regular expression (regex), this value is typically OK. Amazon Macie can compile the expression.</p> <p>If the list's criteria specify an S3 object, possible values are:</p> <ul><li><p>OK - Macie can retrieve and parse the contents of the object.</p></li> <li><p>S3_OBJECT_ACCESS_DENIED\
  \ - Macie isn't allowed to access the object or the object is encrypted with a customer managed KMS key that Macie isn't allowed to use. Check the bucket policy and other permissions settings for the bucket and the object. If the object is encrypted, also ensure that it's encrypted with a key that Macie is allowed to use.</p></li> <li><p>S3_OBJECT_EMPTY - Macie can retrieve the object but the object doesn't contain any content. Ensure that the object contains the correct entries. Also ensure that the list's criteria specify the correct bucket and object names.</p></li> <li><p>S3_OBJECT_NOT_FOUND - The object doesn't exist in Amazon S3. Ensure that the list's criteria specify the correct bucket and object names.</p></li> <li><p>S3_OBJECT_OVERSIZE - Macie can retrieve the object. However, the object contains too many entries or its storage size exceeds the quota for an allow list. Try breaking the list into multiple files and ensure that each file doesn't exceed any quotas. Then configure\
  \ list settings in Macie for each file.</p></li> <li><p>S3_THROTTLED - Amazon S3 throttled the request to retrieve the object. Wait a few minutes and then try again.</p></li> <li><p>S3_USER_ACCESS_DENIED - Amazon S3 denied the request to retrieve the object. If the specified object exists, you're not allowed to access it or it's encrypted with an KMS key that you're not allowed to use. Work with your Amazon Web Services administrator to ensure that the list's criteria specify the correct bucket and object names, and you have read access to the bucket and the object. If the object is encrypted, also ensure that it's encrypted with a key that you're allowed to use.</p></li> <li><p>UNKNOWN_ERROR - A transient or internal error occurred when Macie attempted to retrieve or parse the object. Wait a few minutes and then try again. A list can also have this status if it's encrypted with a key that Amazon S3 and Macie can't access or use.</p></li></ul>\"\n        }\n      ]\n    },\n    \"description\"\
  : {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__stringMin1Max1024PatternSS\"\n        },\n        {\n          \"description\": \"A brief description of the status of the allow list. Amazon Macie uses this value to provide additional information about an error that occurred when Macie tried to access and use the list's criteria.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"code\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-macie/refs/heads/main/json-schema/amazon-macie-allow-list-status-schema.json
tags:
- Data Security
- Sensitive Data
- Privacy
- Compliance
- Machine Learning
- S3
title: AllowListStatus
---
