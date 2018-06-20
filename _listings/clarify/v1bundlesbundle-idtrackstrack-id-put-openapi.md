---
swagger: "2.0"
x-collection-name: Clarify
x-complete: 0
info:
  title: Clarify Add media to a track
  description: 'Add media to an existing track of a bundle. This can only be called
    on a track that currently has no media set or has parts pending.Once all media
    parts have been added to a track it is immutable, meaning it cannot be modified.
    If you wish to modify a track, simply add a new one and delete the existing one.media_url
    must be a publicly accessible url to a media file. It will be fetched asynchronously
    after the REST call returns. The audio can be mono or stereo.audio_channel is
    used to specify audio channels if the media is a stereo file. A value of left
    or right signifies that only the specified channel will be used. If no value or
    an empty string is specified for audio_channel, all channels will be used in a
    single track. If your stereo channels were recorded separately with each channel
    containing distinct content (for example if 2 legs of a phone call were recorded
    separately and combined into a single stereo file), for best speech recognition,
    create two tracks with audio_channel to be left and right. If your stereo file
    is simply a recording made with a stereo microphone, audio_channel should be set
    to an empty string (or not be specified.)audio_language can be used to specify
    the language of the audio media. This is an optional parameter and if not specified
    or an empty string, the language of the track will be automatically detected.
    If specified, it must be a language code as described in RFC5646 (see http://tools.ietf.org/html/rfc5646).
    Supported languages: en-US, en-UK, es, fr.start_time a time in seconds that the
    media starts, relative to start time of the bundle. This allows you to specify
    sequential parts of media. If not specified, the default is 0.parts_pending a
    boolean flag specifying if more media parts will subsequently be added to the
    track. If true, a subsequent API call must be made to signify that the track is
    complete. If not specified, the default is false.If version specified, the track
    will only be added if the current version matches this parameter value. If the
    version doesn''t match, a 409 Conflict error will be returned. If version not
    specified, the track will always be updated.'
  version: 1.3.4
host: api.clarify.io
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /v1/bundles/{bundle_id}/tracks/{track_id}:
    put:
      summary: Add media to a track
      description: 'Add media to an existing track of a bundle. This can only be called
        on a track that currently has no media set or has parts pending.Once all media
        parts have been added to a track it is immutable, meaning it cannot be modified.
        If you wish to modify a track, simply add a new one and delete the existing
        one.media_url must be a publicly accessible url to a media file. It will be
        fetched asynchronously after the REST call returns. The audio can be mono
        or stereo.audio_channel is used to specify audio channels if the media is
        a stereo file. A value of left or right signifies that only the specified
        channel will be used. If no value or an empty string is specified for audio_channel,
        all channels will be used in a single track. If your stereo channels were
        recorded separately with each channel containing distinct content (for example
        if 2 legs of a phone call were recorded separately and combined into a single
        stereo file), for best speech recognition, create two tracks with audio_channel
        to be left and right. If your stereo file is simply a recording made with
        a stereo microphone, audio_channel should be set to an empty string (or not
        be specified.)audio_language can be used to specify the language of the audio
        media. This is an optional parameter and if not specified or an empty string,
        the language of the track will be automatically detected. If specified, it
        must be a language code as described in RFC5646 (see http://tools.ietf.org/html/rfc5646).
        Supported languages: en-US, en-UK, es, fr.start_time a time in seconds that
        the media starts, relative to start time of the bundle. This allows you to
        specify sequential parts of media. If not specified, the default is 0.parts_pending
        a boolean flag specifying if more media parts will subsequently be added to
        the track. If true, a subsequent API call must be made to signify that the
        track is complete. If not specified, the default is false.If version specified,
        the track will only be added if the current version matches this parameter
        value. If the version doesn''t match, a 409 Conflict error will be returned.
        If version not specified, the track will always be updated.'
      operationId: putV1BundlesBundleTracksTrack
      x-api-path-slug: v1bundlesbundle-idtrackstrack-id-put
      parameters:
      - in: formData
        name: audio_channel
        description: The audio channel to use for the track (  | left | right )
      - in: formData
        name: audio_language
        description: Language of the audio in the track, specified with an RFC5646
          code
      - in: path
        name: bundle_id
        description: id of a bundle
      - in: formData
        name: media_url
        description: URL of a media file for this bundle
      - in: formData
        name: parts_pending
        description: Set to true if more media parts will be added to the track
      - in: formData
        name: start_time
        description: Time offset in seconds that the media starts relative to the
          bundle
      - in: path
        name: track_id
        description: id of a track
      - in: formData
        name: version
        description: Object version
      responses:
        200:
          description: OK
      tags:
      - Media
      - To
      - Track
x-streamrank:
  polling_total_time_average: 0
  polling_size_download_average: 0
  streaming_total_time_average: 0
  streaming_size_download_average: 0
  change_yes: 0
  change_no: 0
  time_percentage: 0
  size_percentage: 0
  change_percentage: 0
  last_run: ""
  days_run: 0
  minute_run: 0
---