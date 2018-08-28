---
swagger: "2.0"
x-collection-name: Kaltura
x-complete: 1
info:
  title: Kaltura VPaaS
  description: building-video-experiences-consists-of-ingesting-media-files-playing-back-videos-and-reviewing-usage-and-engagement-analytics--in-between-there-is-a-world-of-nuances-required-for-your-unique-usecase-and-application--kaltura-vpaas-is-built-on-the-principles-of-atomic-services-sdks-and-tools-that-allow-you-full-control-and-flexibility-over-every-element-and-process-in-your-medias-life-cycle-
  version: 3.3.0
host: www.kaltura.com
basePath: /api_v3
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /service/batch/action/addMediaInfo:
    get:
      summary: Get Service Batch Action Addmediainfo
      description: batch addMediaInfoAction action saves a media info object
      operationId: batch.addMediaInfo
      x-api-path-slug: servicebatchactionaddmediainfo-get
      parameters:
      - in: query
        name: mediaInfo[audioBitRateMode]
        description: 'Enum Type: `KalturaBitRateMode`The audio bit rate mode'
      - in: query
        name: mediaInfo[audioBitRate]
        description: The audio bit rate
      - in: query
        name: mediaInfo[audioChannels]
        description: The number of audio channels
      - in: query
        name: mediaInfo[audioCodecId]
        description: The audio codec id
      - in: query
        name: mediaInfo[audioDuration]
        description: The audio duration
      - in: query
        name: mediaInfo[audioFormat]
        description: The audio format
      - in: query
        name: mediaInfo[audioResolution]
        description: The audio resolution
      - in: query
        name: mediaInfo[audioSamplingRate]
        description: The audio sampling rate
      - in: query
        name: mediaInfo[complexityValue]
      - in: query
        name: mediaInfo[containerBitRate]
        description: The container bit rate
      - in: query
        name: mediaInfo[containerDuration]
        description: The container duration
      - in: query
        name: mediaInfo[containerFormat]
        description: The container format
      - in: query
        name: mediaInfo[containerId]
        description: The container id
      - in: query
        name: mediaInfo[containerProfile]
        description: The container profile
      - in: query
        name: mediaInfo[contentStreams]
      - in: query
        name: mediaInfo[fileSize]
        description: The file size
      - in: query
        name: mediaInfo[flavorAssetId]
        description: The id of the related flavor asset
      - in: query
        name: mediaInfo[isFastStart]
      - in: query
        name: mediaInfo[maxGOP]
      - in: query
        name: mediaInfo[multiStreamInfo]
      - in: query
        name: mediaInfo[multiStream]
      - in: query
        name: mediaInfo[rawData]
        description: The data as returned by the mediainfo command line
      - in: query
        name: mediaInfo[scanType]
      - in: query
        name: mediaInfo[videoBitRateMode]
        description: 'Enum Type: `KalturaBitRateMode`The video bit rate mode'
      - in: query
        name: mediaInfo[videoBitRate]
        description: The video bit rate
      - in: query
        name: mediaInfo[videoCodecId]
        description: The video codec id
      - in: query
        name: mediaInfo[videoDar]
        description: The video display aspect ratio (dar)
      - in: query
        name: mediaInfo[videoDuration]
        description: The video duration
      - in: query
        name: mediaInfo[videoFormat]
        description: The video format
      - in: query
        name: mediaInfo[videoFrameRate]
        description: The video frame rate
      - in: query
        name: mediaInfo[videoHeight]
        description: The video height
      - in: query
        name: mediaInfo[videoRotation]
      - in: query
        name: mediaInfo[videoWidth]
        description: The video width
      - in: query
        name: mediaInfo[writingLib]
        description: The writing library
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Service
      - Batch
      - Action
      - AddMediaInfo
---