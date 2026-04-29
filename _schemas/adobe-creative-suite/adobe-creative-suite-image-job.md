---
description: Schema for asynchronous image processing jobs submitted to Adobe Photoshop and related Creative Suite image APIs. Covers the full lifecycle of a job from submission through completion or failure, including input references, output references, and error details.
layout: schema
name: Adobe Creative Suite Image Job
properties_list:
- description: Unique identifier assigned to the image processing job upon submission
  name: jobId
  type: string
- description: Current lifecycle status of the image processing job
  name: status
  type: string
- description: ISO 8601 timestamp indicating when the job was submitted for processing
  name: created
  type: string
- description: ISO 8601 timestamp indicating when the job record was last updated
  name: modified
  type: string
- description: Reference to the input file used for this image processing job
  name: input
  type: object
- description: Reference to the output file location for this image processing job
  name: output
  type: object
- description: List of output files produced when the job succeeds (for multi-output operations)
  name: outputs
  type: array
- description: List of errors encountered during job processing (populated when status is failed)
  name: errors
  type: array
provider_name: Adobe Creative Suite
provider_slug: adobe-creative-suite
schema_file: json-schema/adobe-creative-suite-image-job-schema.json
slug: adobe-creative-suite-image-job
source_filename: adobe-creative-suite-image-job-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://developer.adobe.com/ns/creative-suite/schemas/image-job\",\n  \"title\": \"Adobe Creative Suite Image Job\",\n  \"description\": \"Schema for asynchronous image processing jobs submitted to Adobe Photoshop and related Creative Suite image APIs. Covers the full lifecycle of a job from submission through completion or failure, including input references, output references, and error details.\",\n  \"type\": \"object\",\n  \"required\": [\"jobId\", \"status\"],\n  \"properties\": {\n    \"jobId\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier assigned to the image processing job upon submission\",\n      \"examples\": [\"f54e0fcb-260b-47c3-b520-de0d17dc2b67\"]\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"description\": \"Current lifecycle status of the image processing job\",\n      \"enum\": [\"pending\", \"running\", \"succeeded\", \"failed\"\
  ],\n      \"examples\": [\"succeeded\"]\n    },\n    \"created\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"ISO 8601 timestamp indicating when the job was submitted for processing\",\n      \"examples\": [\"2026-03-02T12:00:00.000Z\"]\n    },\n    \"modified\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"ISO 8601 timestamp indicating when the job record was last updated\",\n      \"examples\": [\"2026-03-02T12:00:45.000Z\"]\n    },\n    \"input\": {\n      \"type\": \"object\",\n      \"description\": \"Reference to the input file used for this image processing job\",\n      \"required\": [\"href\", \"storage\"],\n      \"properties\": {\n        \"href\": {\n          \"type\": \"string\",\n          \"description\": \"URL or path to the input file in the specified cloud storage provider\",\n          \"examples\": [\"https://my-storage.blob.core.windows.net/images/input.psd\"]\n        },\n\
  \        \"storage\": {\n          \"type\": \"string\",\n          \"description\": \"Cloud storage provider where the input file resides\",\n          \"enum\": [\"adobe\", \"external\", \"azure\", \"dropbox\"],\n          \"examples\": [\"external\"]\n        },\n        \"type\": {\n          \"type\": \"string\",\n          \"description\": \"MIME type of the input file\",\n          \"examples\": [\"image/vnd.adobe.photoshop\", \"image/jpeg\", \"image/png\"]\n        }\n      },\n      \"additionalProperties\": false\n    },\n    \"output\": {\n      \"type\": \"object\",\n      \"description\": \"Reference to the output file location for this image processing job\",\n      \"required\": [\"href\", \"storage\", \"type\"],\n      \"properties\": {\n        \"href\": {\n          \"type\": \"string\",\n          \"description\": \"URL or path where the processed output file will be stored\",\n          \"examples\": [\"https://my-storage.blob.core.windows.net/images/output.png\"]\n\
  \        },\n        \"storage\": {\n          \"type\": \"string\",\n          \"description\": \"Cloud storage provider where the output file will be written\",\n          \"enum\": [\"adobe\", \"external\", \"azure\", \"dropbox\"],\n          \"examples\": [\"external\"]\n        },\n        \"type\": {\n          \"type\": \"string\",\n          \"description\": \"MIME type of the output file to produce\",\n          \"examples\": [\"image/png\", \"image/jpeg\", \"image/vnd.adobe.photoshop\"]\n        },\n        \"width\": {\n          \"type\": \"integer\",\n          \"description\": \"Width of the output image in pixels\",\n          \"minimum\": 1,\n          \"examples\": [1920]\n        },\n        \"height\": {\n          \"type\": \"integer\",\n          \"description\": \"Height of the output image in pixels\",\n          \"minimum\": 1,\n          \"examples\": [1080]\n        },\n        \"overwrite\": {\n          \"type\": \"boolean\",\n          \"description\": \"Whether\
  \ to overwrite an existing file at the output location\",\n          \"default\": true\n        }\n      },\n      \"additionalProperties\": false\n    },\n    \"outputs\": {\n      \"type\": \"array\",\n      \"description\": \"List of output files produced when the job succeeds (for multi-output operations)\",\n      \"items\": {\n        \"type\": \"object\",\n        \"description\": \"An individual output produced by this image processing job\",\n        \"properties\": {\n          \"input\": {\n            \"type\": \"string\",\n            \"description\": \"Reference to the input file that generated this output\"\n          },\n          \"status\": {\n            \"type\": \"string\",\n            \"description\": \"Status of this specific output\",\n            \"enum\": [\"pending\", \"running\", \"succeeded\", \"failed\"]\n          },\n          \"details\": {\n            \"type\": \"string\",\n            \"description\": \"Additional human-readable detail about this output's\
  \ status\"\n          },\n          \"href\": {\n            \"type\": \"string\",\n            \"description\": \"URL to download the completed output file\",\n            \"examples\": [\"https://my-storage.blob.core.windows.net/images/output.png\"]\n          },\n          \"storage\": {\n            \"type\": \"string\",\n            \"description\": \"Cloud storage provider where the output file was written\",\n            \"enum\": [\"adobe\", \"external\", \"azure\", \"dropbox\"]\n          },\n          \"type\": {\n            \"type\": \"string\",\n            \"description\": \"MIME type of the output file\",\n            \"examples\": [\"image/png\"]\n          },\n          \"width\": {\n            \"type\": \"integer\",\n            \"description\": \"Actual width of the output image in pixels\",\n            \"minimum\": 1\n          },\n          \"height\": {\n            \"type\": \"integer\",\n            \"description\": \"Actual height of the output image in pixels\"\
  ,\n            \"minimum\": 1\n          }\n        }\n      }\n    },\n    \"errors\": {\n      \"type\": \"array\",\n      \"description\": \"List of errors encountered during job processing (populated when status is failed)\",\n      \"items\": {\n        \"type\": \"object\",\n        \"description\": \"An individual error encountered during image processing\",\n        \"properties\": {\n          \"code\": {\n            \"type\": \"string\",\n            \"description\": \"Machine-readable error code identifying the type of failure\",\n            \"examples\": [\"InputValidationError\", \"StorageAccessError\"]\n          },\n          \"title\": {\n            \"type\": \"string\",\n            \"description\": \"Short human-readable title for the error\",\n            \"examples\": [\"Invalid input file format\"]\n          },\n          \"description\": {\n            \"type\": \"string\",\n            \"description\": \"Detailed human-readable explanation of what went wrong\"\
  ,\n            \"examples\": [\"The provided file is not a valid PSD document\"]\n          }\n        },\n        \"required\": [\"code\"]\n      }\n    }\n  },\n  \"additionalProperties\": false,\n  \"examples\": [\n    {\n      \"jobId\": \"f54e0fcb-260b-47c3-b520-de0d17dc2b67\",\n      \"status\": \"succeeded\",\n      \"created\": \"2026-03-02T12:00:00.000Z\",\n      \"modified\": \"2026-03-02T12:00:45.000Z\",\n      \"input\": {\n        \"href\": \"https://my-storage.blob.core.windows.net/images/product.jpg\",\n        \"storage\": \"external\",\n        \"type\": \"image/jpeg\"\n      },\n      \"output\": {\n        \"href\": \"https://my-storage.blob.core.windows.net/images/product-cutout.png\",\n        \"storage\": \"external\",\n        \"type\": \"image/png\",\n        \"width\": 2000,\n        \"height\": 3000\n      },\n      \"errors\": []\n    }\n  ]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adobe-creative-suite/refs/heads/main/json-schema/adobe-creative-suite-image-job-schema.json
tags:
- Creative
- Design
- Graphics
- Photography
- Video
title: Adobe Creative Suite Image Job
---
