---
swagger: "2.0"
info:
  title: AWS Step Functions API
  version: 1.0.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=DeleteActivity:
    get:
      summary: ' Delete Activity '
      description: Deletes an activity
      operationId: deleteActivity
      parameters:
      - in: query
        name: activityArn
        description: The Amazon Resource Name (ARN) of the activity to delete
        type: string
      responses:
        200:
          description: OK
      tags:
      - activity
definitions: []
x-collection-name: AWS Step Functions
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