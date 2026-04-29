---
description: <p>The container element for specifying the default Object Lock retention settings for new objects placed in the specified bucket.</p> <note> <ul> <li> <p>The <code>DefaultRetention</code> settings require both a mode and a period.</p> </li> <li> <p>The <code>DefaultRetention</code> period can be either <code>Days</code> or <code>Years</code> but you must select one. You cannot specify <code>Days</code> and <code>Years</code> at the same time.</p> </li> </ul> </note>
layout: schema
name: DefaultRetention
properties_list:
- description: ''
  name: Mode
  type: object
- description: ''
  name: Days
  type: object
- description: ''
  name: Years
  type: object
provider_name: Amazon S3 API
provider_slug: aws-s3
schema_file: json-schema/s3-defaultretention-schema.json
slug: s3-defaultretention
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"DefaultRetention\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Mode\": {},\n    \"Days\": {},\n    \"Years\": {}\n  },\n  \"description\": \"<p>The container element for specifying the default Object Lock retention settings for new objects placed in the specified bucket.</p> <note> <ul> <li> <p>The <code>DefaultRetention</code> settings require both a mode and a period.</p> </li> <li> <p>The <code>DefaultRetention</code> period can be either <code>Days</code> or <code>Years</code> but you must select one. You cannot specify <code>Days</code> and <code>Years</code> at the same time.</p> </li> </ul> </note>\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-s3/refs/heads/main/json-schema/s3-defaultretention-schema.json
tags:
- AWS
- Cloud Storage
- Object Storage
- Storage
title: DefaultRetention
---
