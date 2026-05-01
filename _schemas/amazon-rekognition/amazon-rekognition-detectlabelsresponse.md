---
description: Response object from the Amazon Rekognition DetectLabels operation containing detected labels with confidence scores and bounding box information.
layout: schema
name: DetectLabelsResponse
properties_list:
- description: An array of labels for the real-world objects detected in the image.
  name: Labels
  type: array
- description: Version number of the label detection model that was used to detect labels.
  name: LabelModelVersion
  type: string
- description: Information about the properties of the input image.
  name: ImageProperties
  type: object
provider_name: Amazon Rekognition
provider_slug: amazon-rekognition
schema_file: json-schema/amazon-rekognition-detectlabelsresponse-schema.json
slug: amazon-rekognition-detectlabelsresponse
source_filename: amazon-rekognition-detectlabelsresponse-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"http://json-schema.org/draft-07/schema#\",\n  \"$id\": \"https://aws.amazon.com/rekognition/schemas/detectlabelsresponse\",\n  \"title\": \"DetectLabelsResponse\",\n  \"description\": \"Response object from the Amazon Rekognition DetectLabels operation containing detected labels with confidence scores and bounding box information.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Labels\": {\n      \"type\": \"array\",\n      \"description\": \"An array of labels for the real-world objects detected in the image.\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"Name\": {\n            \"type\": \"string\",\n            \"description\": \"The name of the detected label.\"\n          },\n          \"Confidence\": {\n            \"type\": \"number\",\n            \"minimum\": 0,\n            \"maximum\": 100,\n            \"description\": \"Level of confidence in the label detection.\"\n          },\n       \
  \   \"Instances\": {\n            \"type\": \"array\",\n            \"description\": \"A list of instances of the label detected in the image, each with a bounding box.\",\n            \"items\": {\n              \"type\": \"object\",\n              \"properties\": {\n                \"BoundingBox\": {\n                  \"type\": \"object\",\n                  \"description\": \"The position of the detected instance in the image.\",\n                  \"properties\": {\n                    \"Width\": {\n                      \"type\": \"number\",\n                      \"description\": \"Width of the bounding box as a ratio of the overall image width.\"\n                    },\n                    \"Height\": {\n                      \"type\": \"number\",\n                      \"description\": \"Height of the bounding box as a ratio of the overall image height.\"\n                    },\n                    \"Left\": {\n                      \"type\": \"number\",\n                  \
  \    \"description\": \"Left coordinate of the bounding box as a ratio of overall image width.\"\n                    },\n                    \"Top\": {\n                      \"type\": \"number\",\n                      \"description\": \"Top coordinate of the bounding box as a ratio of overall image height.\"\n                    }\n                  },\n                  \"required\": [\"Width\", \"Height\", \"Left\", \"Top\"]\n                },\n                \"Confidence\": {\n                  \"type\": \"number\",\n                  \"minimum\": 0,\n                  \"maximum\": 100,\n                  \"description\": \"The confidence that Amazon Rekognition has in the accuracy of the bounding box.\"\n                }\n              }\n            }\n          },\n          \"Parents\": {\n            \"type\": \"array\",\n            \"description\": \"The parent labels for a label.\",\n            \"items\": {\n              \"type\": \"object\",\n              \"properties\"\
  : {\n                \"Name\": {\n                  \"type\": \"string\",\n                  \"description\": \"The name of the parent label.\"\n                }\n              }\n            }\n          },\n          \"Aliases\": {\n            \"type\": \"array\",\n            \"description\": \"A list of potential aliases for a given label.\",\n            \"items\": {\n              \"type\": \"object\",\n              \"properties\": {\n                \"Name\": {\n                  \"type\": \"string\",\n                  \"description\": \"The name of an alias.\"\n                }\n              }\n            }\n          },\n          \"Categories\": {\n            \"type\": \"array\",\n            \"description\": \"A list of the categories associated with a given label.\",\n            \"items\": {\n              \"type\": \"object\",\n              \"properties\": {\n                \"Name\": {\n                  \"type\": \"string\",\n                  \"description\":\
  \ \"The name of a category that applies to a given label.\"\n                }\n              }\n            }\n          }\n        },\n        \"required\": [\"Name\", \"Confidence\"]\n      }\n    },\n    \"LabelModelVersion\": {\n      \"type\": \"string\",\n      \"description\": \"Version number of the label detection model that was used to detect labels.\"\n    },\n    \"ImageProperties\": {\n      \"type\": \"object\",\n      \"description\": \"Information about the properties of the input image.\",\n      \"properties\": {\n        \"Quality\": {\n          \"type\": \"object\",\n          \"properties\": {\n            \"Brightness\": {\n              \"type\": \"number\",\n              \"description\": \"The brightness of the image.\"\n            },\n            \"Sharpness\": {\n              \"type\": \"number\",\n              \"description\": \"The sharpness of the image.\"\n            },\n            \"Contrast\": {\n              \"type\": \"number\",\n            \
  \  \"description\": \"The contrast of the image.\"\n            }\n          }\n        },\n        \"DominantColors\": {\n          \"type\": \"array\",\n          \"items\": {\n            \"type\": \"object\",\n            \"properties\": {\n              \"Red\": {\n                \"type\": \"integer\"\n              },\n              \"Green\": {\n                \"type\": \"integer\"\n              },\n              \"Blue\": {\n                \"type\": \"integer\"\n              },\n              \"HexCode\": {\n                \"type\": \"string\"\n              },\n              \"SimplifiedColor\": {\n                \"type\": \"string\"\n              },\n              \"CSSColor\": {\n                \"type\": \"string\"\n              },\n              \"PixelPercent\": {\n                \"type\": \"number\"\n              }\n            }\n          }\n        }\n      }\n    }\n  },\n  \"required\": [\"Labels\"]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-rekognition/refs/heads/main/json-schema/amazon-rekognition-detectlabelsresponse-schema.json
tags:
- Celebrity Recognition
- Computer Vision
- Content Moderation
- Custom Labels
- Deep Learning
- Face Liveness
- Facial Recognition
- Image Analysis
- Machine Learning
- Object Detection
- Text Detection
- Video Analysis
title: DetectLabelsResponse
---
