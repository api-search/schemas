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
