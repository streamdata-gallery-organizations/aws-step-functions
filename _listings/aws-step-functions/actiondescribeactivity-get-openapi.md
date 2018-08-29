---
swagger: "2.0"
x-collection-name: AWS Step Functions
x-complete: 0
info:
  title: AWS Step Functions API Describe Activity
  version: 1.0.0
  description: Describes an activity.
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=CreateActivity:
    get:
      summary: Create Activity
      description: Creates an activity.
      operationId: createActivity
      x-api-path-slug: actioncreateactivity-get
      parameters:
      - in: query
        name: name
        description: The name of the activity to create
        type: string
      responses:
        200:
          description: OK
      tags:
      - Activity
  /?Action=CreateStateMachine:
    get:
      summary: Create State Machine
      description: Creates a state machine.
      operationId: createStateMachine
      x-api-path-slug: actioncreatestatemachine-get
      parameters:
      - in: query
        name: definition
        description: The Amazon States Language definition of the state machine
        type: string
      - in: query
        name: name
        description: The name of the state machine
        type: string
      - in: query
        name: roleArn
        description: The Amazon Resource Name (ARN) of the IAM role to use for this
          state machine
        type: string
      responses:
        200:
          description: OK
      tags:
      - State Machine
  /?Action=DeleteActivity:
    get:
      summary: Delete Activity
      description: Deletes an activity.
      operationId: deleteActivity
      x-api-path-slug: actiondeleteactivity-get
      parameters:
      - in: query
        name: activityArn
        description: The Amazon Resource Name (ARN) of the activity to delete
        type: string
      responses:
        200:
          description: OK
      tags:
      - Activity
  /?Action=DeleteStateMachine:
    get:
      summary: Delete State Machine
      description: Deletes a state machine.
      operationId: deleteStateMachine
      x-api-path-slug: actiondeletestatemachine-get
      parameters:
      - in: query
        name: stateMachineArn
        description: The Amazon Resource Name (ARN) of the state machine to delete
        type: string
      responses:
        200:
          description: OK
      tags:
      - State Machine
  /?Action=DescribeActivity:
    get:
      summary: Describe Activity
      description: Describes an activity.
      operationId: describeActivity
      x-api-path-slug: actiondescribeactivity-get
      parameters:
      - in: query
        name: activityArn
        description: The Amazon Resource Name (ARN) of the activity to describe
        type: string
      responses:
        200:
          description: OK
      tags:
      - Activity
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