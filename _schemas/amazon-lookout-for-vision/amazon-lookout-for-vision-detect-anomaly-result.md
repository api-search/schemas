---
description: The prediction results from a call to <a>DetectAnomalies</a>. <code>DetectAnomalyResult</code> includes classification information for the prediction (<code>IsAnomalous</code> and <code>Confidence</code>). If the model you use is an image segementation model, <code>DetectAnomalyResult</code> also includes segmentation information (<code>Anomalies</code> and <code>AnomalyMask</code>). Classification information is calculated separately from segmentation information and you shouldn't assume a relationship between them.
layout: schema
name: DetectAnomalyResult
properties_list:
- description: ''
  name: Source
  type: object
- description: ''
  name: IsAnomalous
  type: object
- description: ''
  name: Confidence
  type: object
- description: ''
  name: Anomalies
  type: object
- description: ''
  name: AnomalyMask
  type: object
provider_name: Amazon Lookout for Vision
provider_slug: amazon-lookout-for-vision
schema_file: json-schema/amazon-lookout-for-vision-detect-anomaly-result-schema.json
slug: amazon-lookout-for-vision-detect-anomaly-result
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-lookout-for-vision/refs/heads/main/json-schema/amazon-lookout-for-vision-detect-anomaly-result-schema.json\",\n  \"title\": \"DetectAnomalyResult\",\n  \"description\": \"The prediction results from a call to <a>DetectAnomalies</a>. <code>DetectAnomalyResult</code> includes classification information for the prediction (<code>IsAnomalous</code> and <code>Confidence</code>). If the model you use is an image segementation model, <code>DetectAnomalyResult</code> also includes segmentation information (<code>Anomalies</code> and <code>AnomalyMask</code>). Classification information is calculated separately from segmentation information and you shouldn't assume a relationship between them.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Source\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ImageSource\"\
  \n        },\n        {\n          \"description\": \"The source of the image that was analyzed. <code>direct</code> means that the images was supplied from the local computer. No other values are supported.\"\n        }\n      ]\n    },\n    \"IsAnomalous\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Boolean\"\n        },\n        {\n          \"description\": \"True if Amazon Lookout for Vision classifies the image as containing an anomaly, otherwise false.\"\n        }\n      ]\n    },\n    \"Confidence\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Float\"\n        },\n        {\n          \"description\": \"The confidence that Lookout for Vision has in the accuracy of the classification in <code>IsAnomalous</code>.\"\n        }\n      ]\n    },\n    \"Anomalies\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AnomalyList\"\n        },\n        {\n          \"description\": \"<p>If the\
  \ model is an image segmentation model, <code>Anomalies</code> contains a list of anomaly types found in the image. There is one entry for each type of anomaly found (even if multiple instances of an anomaly type exist on the image). The first element in the list is always an anomaly type representing the image background ('background') and shouldn't be considered an anomaly. Amazon Lookout for Vision automatically add the background anomaly type to the response, and you don't need to declare a background anomaly type in your dataset.</p> <p>If the list has one entry ('background'), no anomalies were found on the image.</p> <p/> <p>An image classification model doesn't return an <code>Anomalies</code> list. </p>\"\n        }\n      ]\n    },\n    \"AnomalyMask\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AnomalyMask\"\n        },\n        {\n          \"description\": \"<p>If the model is an image segmentation model, <code>AnomalyMask</code> contains\
  \ pixel masks that covers all anomaly types found on the image. Each anomaly type has a different mask color. To map a color to an anomaly type, see the <code>color</code> field of the <a>PixelAnomaly</a> object.</p> <p>An image classification model doesn't return an <code>Anomalies</code> list. </p>\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-lookout-for-vision/refs/heads/main/json-schema/amazon-lookout-for-vision-detect-anomaly-result-schema.json
tags:
- AWS
- Computer Vision
- Machine Learning
- Manufacturing
- Quality Inspection
- Anomaly Detection
title: DetectAnomalyResult
---
