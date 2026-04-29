---
description: Options for configuring the Apache Cordova Camera plugin getPicture call
layout: schema
name: CameraOptions
properties_list:
- description: Quality of the saved image, expressed as a range of 0-100, where 100 is typically full resolution with no file compression loss.
  name: quality
  type: integer
- description: Choose the format of the return value. 0 = DATA_URL (base64 encoded string), 1 = FILE_URI (image file URI).
  name: destinationType
  type: integer
- description: Set the source of the picture. 0 = PHOTOLIBRARY, 1 = CAMERA, 2 = SAVEDPHOTOALBUM.
  name: sourceType
  type: integer
- description: Allow simple editing of image before selection.
  name: allowEdit
  type: boolean
- description: Choose the returned image file encoding. 0 = JPEG, 1 = PNG.
  name: encodingType
  type: integer
- description: Width in pixels to scale image. Must be used with targetHeight. Aspect ratio remains constant.
  name: targetWidth
  type: integer
- description: Height in pixels to scale image. Must be used with targetWidth. Aspect ratio remains constant.
  name: targetHeight
  type: integer
- description: Set the type of media to select from. 0 = PICTURE, 1 = VIDEO, 2 = ALLMEDIA. Only works when sourceType is PHOTOLIBRARY or SAVEDPHOTOALBUM.
  name: mediaType
  type: integer
- description: Rotate the image to correct for the orientation of the device during capture.
  name: correctOrientation
  type: boolean
- description: Save the image to the photo album on the device after capture.
  name: saveToPhotoAlbum
  type: boolean
- description: Choose the camera to use. 0 = BACK, 1 = FRONT.
  name: cameraDirection
  type: integer
provider_name: Apache Cordova
provider_slug: apache-cordova
schema_file: json-schema/apache-cordova-camera-options-schema.json
slug: apache-cordova-camera-options
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-cordova/refs/heads/main/json-schema/apache-cordova-camera-options-schema.json\",\n  \"title\": \"CameraOptions\",\n  \"description\": \"Options for configuring the Apache Cordova Camera plugin getPicture call\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"quality\": {\n      \"type\": \"integer\",\n      \"description\": \"Quality of the saved image, expressed as a range of 0-100, where 100 is typically full resolution with no file compression loss.\",\n      \"minimum\": 0,\n      \"maximum\": 100,\n      \"default\": 50,\n      \"example\": 75\n    },\n    \"destinationType\": {\n      \"type\": \"integer\",\n      \"description\": \"Choose the format of the return value. 0 = DATA_URL (base64 encoded string), 1 = FILE_URI (image file URI).\",\n      \"enum\": [0, 1],\n      \"default\": 1,\n      \"example\": 1\n    },\n    \"\
  sourceType\": {\n      \"type\": \"integer\",\n      \"description\": \"Set the source of the picture. 0 = PHOTOLIBRARY, 1 = CAMERA, 2 = SAVEDPHOTOALBUM.\",\n      \"enum\": [0, 1, 2],\n      \"default\": 1,\n      \"example\": 1\n    },\n    \"allowEdit\": {\n      \"type\": \"boolean\",\n      \"description\": \"Allow simple editing of image before selection.\",\n      \"default\": false,\n      \"example\": false\n    },\n    \"encodingType\": {\n      \"type\": \"integer\",\n      \"description\": \"Choose the returned image file encoding. 0 = JPEG, 1 = PNG.\",\n      \"enum\": [0, 1],\n      \"default\": 0,\n      \"example\": 0\n    },\n    \"targetWidth\": {\n      \"type\": \"integer\",\n      \"description\": \"Width in pixels to scale image. Must be used with targetHeight. Aspect ratio remains constant.\",\n      \"minimum\": 1,\n      \"example\": 800\n    },\n    \"targetHeight\": {\n      \"type\": \"integer\",\n      \"description\": \"Height in pixels to scale image. Must\
  \ be used with targetWidth. Aspect ratio remains constant.\",\n      \"minimum\": 1,\n      \"example\": 600\n    },\n    \"mediaType\": {\n      \"type\": \"integer\",\n      \"description\": \"Set the type of media to select from. 0 = PICTURE, 1 = VIDEO, 2 = ALLMEDIA. Only works when sourceType is PHOTOLIBRARY or SAVEDPHOTOALBUM.\",\n      \"enum\": [0, 1, 2],\n      \"default\": 0,\n      \"example\": 0\n    },\n    \"correctOrientation\": {\n      \"type\": \"boolean\",\n      \"description\": \"Rotate the image to correct for the orientation of the device during capture.\",\n      \"example\": true\n    },\n    \"saveToPhotoAlbum\": {\n      \"type\": \"boolean\",\n      \"description\": \"Save the image to the photo album on the device after capture.\",\n      \"default\": false,\n      \"example\": false\n    },\n    \"cameraDirection\": {\n      \"type\": \"integer\",\n      \"description\": \"Choose the camera to use. 0 = BACK, 1 = FRONT.\",\n      \"enum\": [0, 1],\n      \"\
  default\": 0,\n      \"example\": 0\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-cordova/refs/heads/main/json-schema/apache-cordova-camera-options-schema.json
tags:
- Apache
- Cross-Platform
- Hybrid Apps
- JavaScript
- Mobile
- Open Source
- Plugins
title: CameraOptions
---
