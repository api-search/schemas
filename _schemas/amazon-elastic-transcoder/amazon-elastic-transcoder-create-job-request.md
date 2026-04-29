---
description: The <code>CreateJobRequest</code> structure.
layout: schema
name: CreateJobRequest
properties_list:
- description: ''
  name: PipelineId
  type: object
- description: ''
  name: Input
  type: object
- description: ''
  name: Inputs
  type: object
- description: ''
  name: Output
  type: object
- description: ''
  name: Outputs
  type: object
- description: ''
  name: OutputKeyPrefix
  type: object
- description: ''
  name: Playlists
  type: object
- description: ''
  name: UserMetadata
  type: object
provider_name: Amazon Elastic Transcoder
provider_slug: amazon-elastic-transcoder
schema_file: json-schema/amazon-elastic-transcoder-create-job-request-schema.json
slug: amazon-elastic-transcoder-create-job-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-elastic-transcoder/refs/heads/main/json-schema/amazon-elastic-transcoder-create-job-request-schema.json\",\n  \"title\": \"CreateJobRequest\",\n  \"description\": \"The <code>CreateJobRequest</code> structure.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"PipelineId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Id\"\n        },\n        {\n          \"description\": \"The <code>Id</code> of the pipeline that you want Elastic Transcoder to use for transcoding. The pipeline determines several settings, including the Amazon S3 bucket from which Elastic Transcoder gets the files to transcode and the bucket into which Elastic Transcoder puts the transcoded files.\"\n        }\n      ]\n    },\n    \"Input\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/JobInput\"\n   \
  \     },\n        {\n          \"description\": \"A section of the request body that provides information about the file that is being transcoded.\"\n        }\n      ]\n    },\n    \"Inputs\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/JobInputs\"\n        },\n        {\n          \"description\": \"A section of the request body that provides information about the files that are being transcoded.\"\n        }\n      ]\n    },\n    \"Output\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/CreateJobOutput\"\n        },\n        {\n          \"description\": \" A section of the request body that provides information about the transcoded (target) file. We strongly recommend that you use the <code>Outputs</code> syntax instead of the <code>Output</code> syntax. \"\n        }\n      ]\n    },\n    \"Outputs\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/CreateJobOutputs\"\n        },\n        {\n\
  \          \"description\": \" A section of the request body that provides information about the transcoded (target) files. We recommend that you use the <code>Outputs</code> syntax instead of the <code>Output</code> syntax. \"\n        }\n      ]\n    },\n    \"OutputKeyPrefix\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Key\"\n        },\n        {\n          \"description\": \"The value, if any, that you want Elastic Transcoder to prepend to the names of all files that this job creates, including output files, thumbnails, and playlists.\"\n        }\n      ]\n    },\n    \"Playlists\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/CreateJobPlaylists\"\n        },\n        {\n          \"description\": \"<p>If you specify a preset in <code>PresetId</code> for which the value of <code>Container</code> is fmp4 (Fragmented MP4) or ts (MPEG-TS), Playlists contains information about the master playlists that you want Elastic\
  \ Transcoder to create.</p> <p>The maximum number of master playlists in a job is 30.</p>\"\n        }\n      ]\n    },\n    \"UserMetadata\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/UserMetadata\"\n        },\n        {\n          \"description\": \"User-defined metadata that you want to associate with an Elastic Transcoder job. You specify metadata in <code>key/value</code> pairs, and you can add up to 10 <code>key/value</code> pairs per job. Elastic Transcoder does not guarantee that <code>key/value</code> pairs are returned in the same order in which you specify them.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"PipelineId\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-elastic-transcoder/refs/heads/main/json-schema/amazon-elastic-transcoder-create-job-request-schema.json
tags:
- Amazon Web Services
- AWS
- Media
- Transcoding
- Video
title: CreateJobRequest
---
