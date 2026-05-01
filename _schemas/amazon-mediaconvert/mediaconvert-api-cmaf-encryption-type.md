---
description: Specify the encryption scheme that you want the service to use when encrypting your CMAF segments. Choose AES-CBC subsample (SAMPLE-AES) or AES_CTR (AES-CTR).
layout: schema
name: CmafEncryptionType
properties_list: []
provider_name: Amazon MediaConvert
provider_slug: amazon-mediaconvert
schema_file: json-schema/mediaconvert-api-cmaf-encryption-type-schema.json
slug: mediaconvert-api-cmaf-encryption-type
source_filename: mediaconvert-api-cmaf-encryption-type-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mediaconvert/refs/heads/main/json-schema/mediaconvert-api-cmaf-encryption-type-schema.json\",\n  \"title\": \"CmafEncryptionType\",\n  \"description\": \"Specify the encryption scheme that you want the service to use when encrypting your CMAF segments. Choose AES-CBC subsample (SAMPLE-AES) or AES_CTR (AES-CTR).\",\n  \"type\": \"string\",\n  \"enum\": [\n    \"SAMPLE_AES\",\n    \"AES_CTR\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mediaconvert/refs/heads/main/json-schema/mediaconvert-api-cmaf-encryption-type-schema.json
tags:
- Broadcasting
- Media Processing
- Media
title: CmafEncryptionType
---
