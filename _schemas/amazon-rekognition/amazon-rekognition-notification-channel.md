---
description: Amazon SNS topic for completion status notifications.
layout: schema
name: NotificationChannel
properties_list:
- description: The Amazon SNS topic ARN to post completion status.
  name: SNSTopicArn
  type: string
- description: The ARN of an IAM role that gives Rekognition publishing permissions.
  name: RoleArn
  type: string
provider_name: Amazon Rekognition
provider_slug: amazon-rekognition
schema_file: json-schema/amazon-rekognition-notification-channel-schema.json
slug: amazon-rekognition-notification-channel
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-rekognition/refs/heads/main/json-schema/amazon-rekognition-notification-channel-schema.json\",\n  \"title\": \"NotificationChannel\",\n  \"description\": \"Amazon SNS topic for completion status notifications.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"SNSTopicArn\": {\n      \"type\": \"string\",\n      \"description\": \"The Amazon SNS topic ARN to post completion status.\",\n      \"example\": \"arn:aws:sns:us-east-1:123456789012:AmazonRekognitionTopic\"\n    },\n    \"RoleArn\": {\n      \"type\": \"string\",\n      \"description\": \"The ARN of an IAM role that gives Rekognition publishing permissions.\",\n      \"example\": \"arn:aws:iam::123456789012:role/RekognitionRole\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-rekognition/refs/heads/main/json-schema/amazon-rekognition-notification-channel-schema.json
tags:
- AWS
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
title: NotificationChannel
---
