---
swagger: "2.0"
x-collection-name: AWS Cognito
x-complete: 1
info:
  title: AWS Cognito Merged API
  version: 1.0.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=InitiateAuth:
    get:
      summary: Initiate Auth
      description: Initiates the authentication flow.
      operationId: initiateAuth
      x-api-path-slug: actioninitiateauth-get
      parameters:
      - in: query
        name: AuthFlow
        description: The authentication flow
        type: string
      - in: query
        name: AuthParameters
        description: The authentication parameters
        type: string
      - in: query
        name: ClientId
        description: The client ID
        type: string
      - in: query
        name: ClientMetadata
        description: The client apps metadata
        type: string
      responses:
        200:
          description: OK
      tags:
      - Authentication
  /?Action=AdminInitiateAuth:
    get:
      summary: Admin Initiate Auth
      description: Initiates the authentication flow, as an administrator.
      operationId: adminInitiateAuth
      x-api-path-slug: actionadmininitiateauth-get
      parameters:
      - in: query
        name: AuthFlow
        description: The authentication flow
        type: string
      - in: query
        name: AuthParameters
        description: The authentication parameters
        type: string
      - in: query
        name: ClientId
        description: The client app ID
        type: string
      - in: query
        name: ClientMetadata
        description: The client app metadata
        type: string
      - in: query
        name: UserPoolId
        description: The ID of the Amazon Cognito user pool
        type: string
      responses:
        200:
          description: OK
      tags:
      - Authnetication
---