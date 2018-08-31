---
swagger: "2.0"
x-collection-name: Predix
x-complete: 0
info:
  title: Predix Nurego Post Registrations
  description: |-
    The following parameters can be used to validate the user's request.
    The parameters are optional, but the sample code includes email as part of the requestParams.post method.
  contact:
    name: support@nurego.com
  version: 1.0.0
host: api.nurego.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /monitoring/heartbeat:
    get:
      summary: Monitoring API that allows to check the ACS heartbeat
      description: Monitoring api that allows to check the acs heartbeat.
      operationId: getHeartBeatUsingGET
      x-api-path-slug: monitoringheartbeat-get
      responses:
        200:
          description: Successful response
      tags:
      - Monitoring
      - That
      - Ows
      - To
      - Check
      - ACS
      - Heartbeat
  /v1/connector/resource:
    get:
      summary: Retrieves connector configuration for external resource attributes
        for the given zone.
      description: Retrieves connector configuration for external resource attributes
        for the given zone..
      operationId: getResourceConnectorUsingGET_1
      x-api-path-slug: v1connectorresource-get
      responses:
        200:
          description: Successful response
      tags:
      - Retrieves
      - Connector
      - Configurationexternal
      - Resource
      - Attributesthe
      - Given
      - Zone
    put:
      summary: Creates or updates connector configuration for external resource attributes
        for the given zone.
      description: Creates or updates connector configuration for external resource
        attributes for the given zone..
      operationId: putResourceConnectorUsingPUT_1
      x-api-path-slug: v1connectorresource-put
      parameters:
      - in: body
        name: connector
        description: New or updated connector configuration for external resource
          attributes
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: Successful response
      tags:
      - Creates
      - Updates
      - Connector
      - Configurationexternal
      - Resource
      - Attributesthe
      - Given
      - Zone
    delete:
      summary: Deletes connector configuration for external resource attributes for
        the given zone.
      description: Deletes connector configuration for external resource attributes
        for the given zone..
      operationId: deleteResourceConnectorUsingDELETE
      x-api-path-slug: v1connectorresource-delete
      responses:
        200:
          description: Successful response
      tags:
      - S
      - Connector
      - Configurationexternal
      - Resource
      - Attributesthe
      - Given
      - Zone
  /v1/connector/subject:
    get:
      summary: Retrieves connector configuration for external subject attributes for
        the given zone.
      description: Retrieves connector configuration for external subject attributes
        for the given zone..
      operationId: getSubjectConnectorUsingGET
      x-api-path-slug: v1connectorsubject-get
      responses:
        200:
          description: Successful response
      tags:
      - Retrieves
      - Connector
      - Configurationexternal
      - Subject
      - Attributesthe
      - Given
      - Zone
    put:
      summary: Creates or updates connector configuration for external subject attributes
        for the given zone.
      description: Creates or updates connector configuration for external subject
        attributes for the given zone..
      operationId: putSubjectConnectorUsingPUT_1
      x-api-path-slug: v1connectorsubject-put
      parameters:
      - in: body
        name: connector
        description: New or updated connector configuration for external subject attributes
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: Successful response
      tags:
      - Creates
      - Updates
      - Connector
      - Configurationexternal
      - Subject
      - Attributesthe
      - Given
      - Zone
    delete:
      summary: Deletes connector configuration for external subject attributes for
        the given zone.
      description: Deletes connector configuration for external subject attributes
        for the given zone..
      operationId: deleteSubjectConnectorUsingDELETE
      x-api-path-slug: v1connectorsubject-delete
      responses:
        200:
          description: Successful response
      tags:
      - S
      - Connector
      - Configurationexternal
      - Subject
      - Attributesthe
      - Given
      - Zone
  /v1/policy-evaluation:
    post:
      summary: Evaluates all applicable policies and returns decision result
      description: Evaluates all applicable policies and returns decision result.
      operationId: evalPolicyV1UsingPOST
      x-api-path-slug: v1policyevaluation-post
      parameters:
      - in: body
        name: request
        description: request
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: Successful response
      tags:
      - Evaluates
      - ""
      - Applicable
      - Policies
      - Returns
      - Decision
      - Result
  /v1/policy-set:
    get:
      summary: Returns all the policy sets for the given zone.
      description: Returns all the policy sets for the given zone..
      operationId: getAllPolicySetsUsingGET_1
      x-api-path-slug: v1policyset-get
      responses:
        200:
          description: Successful response
      tags:
      - Returns
      - ""
      - Policy
      - Setsthe
      - Given
      - Zone
  /v1/policy-set/{policySetId}:
    get:
      summary: Retrieves a policy set for the given zone.
      description: Retrieves a policy set for the given zone..
      operationId: getPolicySetUsingGET
      x-api-path-slug: v1policysetpolicysetid-get
      parameters:
      - in: path
        name: policySetId
        description: policySetId
      responses:
        200:
          description: Successful response
      tags:
      - Retrieves
      - Policy
      - Setthe
      - Given
      - Zone
    put:
      summary: Creates/Updates a policy set for the given zone.
      description: Creates/updates a policy set for the given zone..
      operationId: createPolicySetUsingPUT_1
      x-api-path-slug: v1policysetpolicysetid-put
      parameters:
      - in: body
        name: policySet
        description: policySet
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: policySetId
        description: policySetId
      responses:
        200:
          description: Successful response
      tags:
      - Creates
      - S
      - Policy
      - Setthe
      - Given
      - Zone
    delete:
      summary: Deletes a policy set for the given zone.
      description: Deletes a policy set for the given zone..
      operationId: deletePolicySetUsingDELETE
      x-api-path-slug: v1policysetpolicysetid-delete
      parameters:
      - in: path
        name: policySetId
        description: policySetId
      responses:
        200:
          description: Successful response
      tags:
      - S
      - Policy
      - Setthe
      - Given
      - Zone
  /v1/resource:
    get:
      summary: Retrieves the list of all resources for the given zone.
      description: Retrieves the list of all resources for the given zone..
      operationId: getResourcesUsingGET
      x-api-path-slug: v1resource-get
      responses:
        200:
          description: Successful response
      tags:
      - Retrieves
      - List
      - Of
      - ""
      - Resourcesthe
      - Given
      - Zone
    post:
      summary: Creates a list of resources for the given zone. Existing resources
        will be updated with the provided values.
      description: Creates a list of resources for the given zone. existing resources
        will be updated with the provided values..
      operationId: appendResourcesUsingPOST
      x-api-path-slug: v1resource-post
      parameters:
      - in: body
        name: resources
        description: resources
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: Successful response
      tags:
      - Creates
      - List
      - Of
      - Resourcesthe
      - Given
      - Zone
      - ""
      - Existing
      - Resources
      - Will
      - Be
      - Updated
      - Provided
      - Values
  /v1/resource/{resourceIdentifier}:
    get:
      summary: Retrieves the resource for the given zone. The resourceIdentifier must
        be URL encoded in application/x-www-form-urlencoded format with UTF-8.
      description: Retrieves the resource for the given zone. the resourceidentifier
        must be url encoded in application/x-www-form-urlencoded format with utf-8..
      operationId: getResourceV1UsingGET
      x-api-path-slug: v1resourceresourceidentifier-get
      parameters:
      - in: query
        name: includeInheritedAttributes
        description: includeInheritedAttributes
      - in: path
        name: resourceIdentifier
        description: resourceIdentifier
      responses:
        200:
          description: Successful response
      tags:
      - Retrieves
      - Resourcethe
      - Given
      - Zone
      - ""
      - ResourceIdentifier
      - Must
      - Be
      - URL
      - Encoded
      - In
      - Application
      - X-www-form-urlencoded
      - Format
      - UTF-8
    put:
      summary: Creates/Updates a given resource for a given zone. The resourceIdentifier
        must be URL encoded in application/x-www-form-urlencoded format with UTF-8.
      description: Creates/updates a given resource for a given zone. the resourceidentifier
        must be url encoded in application/x-www-form-urlencoded format with utf-8..
      operationId: putResourceV1UsingPUT_1
      x-api-path-slug: v1resourceresourceidentifier-put
      parameters:
      - in: body
        name: resource
        description: resource
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: resourceIdentifier
        description: resourceIdentifier
      responses:
        200:
          description: Successful response
      tags:
      - Creates
      - S
      - Given
      - Resourcea
      - Given
      - Zone
      - ""
      - ResourceIdentifier
      - Must
      - Be
      - URL
      - Encoded
      - In
      - Application
      - X-www-form-urlencoded
      - Format
      - UTF-8
    delete:
      summary: Deletes the resource for a given zone. The resourceIdentifier must
        be URL encoded in application/x-www-form-urlencoded format with UTF-8.
      description: Deletes the resource for a given zone. the resourceidentifier must
        be url encoded in application/x-www-form-urlencoded format with utf-8..
      operationId: deleteResourceV1UsingDELETE
      x-api-path-slug: v1resourceresourceidentifier-delete
      parameters:
      - in: path
        name: resourceIdentifier
        description: resourceIdentifier
      responses:
        200:
          description: Successful response
      tags:
      - S
      - Resourcea
      - Given
      - Zone
      - ""
      - ResourceIdentifier
      - Must
      - Be
      - URL
      - Encoded
      - In
      - Application
      - X-www-form-urlencoded
      - Format
      - UTF-8
  /v1/subject:
    get:
      summary: Retrieves the list of subjects for the given zone.
      description: Retrieves the list of subjects for the given zone..
      operationId: getSubjectsUsingGET_1
      x-api-path-slug: v1subject-get
      responses:
        200:
          description: Successful response
      tags:
      - Retrieves
      - List
      - Of
      - Subjectsthe
      - Given
      - Zone
    post:
      summary: Creates a list of subjects. Existing subjects will be updated with
        the provided values.
      description: Creates a list of subjects. existing subjects will be updated with
        the provided values..
      operationId: appendsubjectsUsingPOST_1
      x-api-path-slug: v1subject-post
      parameters:
      - in: body
        name: subjects
        description: subjects
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: Successful response
      tags:
      - Creates
      - List
      - Of
      - Subjects
      - ""
      - Existing
      - Subjects
      - Will
      - Be
      - Updated
      - Provided
      - Values
  /v1/subject/{subjectIdentifier}:
    get:
      summary: Retrieves the subject for the given zone. The subjectIdentifier must
        be URL encoded in application/x-www-form-urlencoded format with UTF-8.
      description: Retrieves the subject for the given zone. the subjectidentifier
        must be url encoded in application/x-www-form-urlencoded format with utf-8..
      operationId: getSubjectUsingGET
      x-api-path-slug: v1subjectsubjectidentifier-get
      parameters:
      - in: query
        name: includeInheritedAttributes
        description: includeInheritedAttributes
      - in: path
        name: subjectIdentifier
        description: subjectIdentifier
      responses:
        200:
          description: Successful response
      tags:
      - Retrieves
      - Subjectthe
      - Given
      - Zone
      - ""
      - SubjectIdentifier
      - Must
      - Be
      - URL
      - Encoded
      - In
      - Application
      - X-www-form-urlencoded
      - Format
      - UTF-8
    put:
      summary: Creates/Updates a given Subject.
      description: Creates/updates a given subject..
      operationId: putSubjectUsingPUT_1
      x-api-path-slug: v1subjectsubjectidentifier-put
      parameters:
      - in: body
        name: subject
        description: subject
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: subjectIdentifier
        description: subjectIdentifier
      responses:
        200:
          description: Successful response
      tags:
      - Creates
      - S
      - Given
      - Subject
    delete:
      summary: Deletes the subject for a given zone. The subjectIdentifier must be
        URL encoded in application/x-www-form-urlencoded format with UTF-8.
      description: Deletes the subject for a given zone. the subjectidentifier must
        be url encoded in application/x-www-form-urlencoded format with utf-8..
      operationId: deleteSubjectUsingDELETE_1
      x-api-path-slug: v1subjectsubjectidentifier-delete
      parameters:
      - in: path
        name: subjectIdentifier
        description: subjectIdentifier
      responses:
        200:
          description: Successful response
      tags:
      - S
      - Subjecta
      - Given
      - Zone
      - ""
      - SubjectIdentifier
      - Must
      - Be
      - URL
      - Encoded
      - In
      - Application
      - X-www-form-urlencoded
      - Format
      - UTF-8
  /api/v1/analytic/execution:
    post:
      summary: Execute the analytic synchronously.
      description: Execute the analytic synchronously with the given execution payload.
      operationId: synchronousExecution
      x-api-path-slug: apiv1analyticexecution-post
      parameters:
      - in: header
        name: Authorization
        description: Authorization
      - in: body
        name: body
        description: request payload containing analytic input data
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Predix-Zone-Id
        description: Predix-Zone-Id
      responses:
        2:
          description: Successful response
      tags:
      - Execute
      - Analytic
      - Synchronously
  /api/v1/analytic/execution/async:
    post:
      summary: Execute the analytic asynchronously using input data.
      description: Execute the analytic asynchronously with the given input data payload.
      operationId: asynchronousExecution
      x-api-path-slug: apiv1analyticexecutionasync-post
      parameters:
      - in: header
        name: Authorization
        description: Authorization
      - in: body
        name: body
        description: request payload containing analytic input data
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Predix-Zone-Id
        description: Predix-Zone-Id
      responses:
        2:
          description: Successful response
      tags:
      - Execute
      - Analytic
      - Asynchronously
      - Using
      - Input
      - Data
  /api/v1/analytic/execution/async/{requestId}:
    delete:
      summary: Cleanup analytic execution result by request id.
      description: Removes the analytic execution result from the cache. It is highly
        recommended to clean your old result data to have room for future result data.
      operationId: clearAnalyticExecutionResult
      x-api-path-slug: apiv1analyticexecutionasyncrequestid-delete
      parameters:
      - in: header
        name: Authorization
      - in: header
        name: Predix-Zone-Id
      - in: path
        name: requestId
      responses:
        2:
          description: Successful response
      tags:
      - Cleanup
      - Analytic
      - Execution
      - Result
      - By
      - Request
      - Id
  /api/v1/analytic/execution/async/{requestId}/result:
    get:
      summary: Get the analytic execution result by request id.
      description: Returns the analytic execution result.
      operationId: retrieveAnalyticExecutionResult
      x-api-path-slug: apiv1analyticexecutionasyncrequestidresult-get
      parameters:
      - in: header
        name: Authorization
        description: Authorization
      - in: header
        name: Predix-Zone-Id
        description: Predix-Zone-Id
      - in: path
        name: requestId
        description: analytic execution request id
      responses:
        2:
          description: Successful response
      tags:
      - Analytic
      - Execution
      - Result
      - By
      - Request
      - Id
  /api/v1/analytic/execution/async/{requestId}/status:
    get:
      summary: Get the analytic execution status by request id.
      description: Returns the analytic execution status (one of QUEUED, PROCESSING,
        COMPLETED, or FAILED).
      operationId: retrieveAnalyticExecutionStatus
      x-api-path-slug: apiv1analyticexecutionasyncrequestidstatus-get
      parameters:
      - in: header
        name: Authorization
        description: Authorization
      - in: header
        name: Predix-Zone-Id
        description: Predix-Zone-Id
      - in: path
        name: requestId
        description: analytic execution request id
      responses:
        2:
          description: Successful response
      tags:
      - Analytic
      - Execution
      - Status
      - By
      - Request
      - Id
  /api/v1/catalog/analytics:
    get:
      summary: Get all analytic catalog entries.
      description: Returns all analytic catalog entries as specified by page and sort
        criteria.
      operationId: retrieveAll
      x-api-path-slug: apiv1cataloganalytics-get
      parameters:
      - in: query
        name: page
        description: 'page index : zero-based page index'
      - in: query
        name: size
        description: 'page size : between 1 and 1000 inclusive'
      - in: query
        name: sortableFields
        description: 'sortable fields : name'
      - in: query
        name: sortOrder
        description: 'sort order : asc | desc'
      - in: query
        name: taxonomyPath
        description: 'taxonomy path : taxonomyPath'
      responses:
        2:
          description: Successful response
      tags:
      - Analytic
      - Catalog
      - Entries
    post:
      summary: Create an analytic catalog entry.
      description: Creates the analytic catalog entry with a generated id.
      operationId: createAnalyticCatalogEntry
      x-api-path-slug: apiv1cataloganalytics-post
      parameters:
      - in: body
        name: body
        description: analytic catalog entry
        schema:
          $ref: '#/definitions/holder'
      responses:
        2:
          description: Successful response
      tags:
      - Analytic
      - Catalog
      - Entry
  /api/v1/catalog/analytics/versions:
    get:
      summary: Get all versions of the analytic catalog entry with the given name.
      description: Returns all versions of the analytic catalog entry with the given
        name.
      operationId: retrieveByName
      x-api-path-slug: apiv1cataloganalyticsversions-get
      parameters:
      - in: query
        name: name
        description: analytic name
      responses:
        2:
          description: Successful response
      tags:
      - Versions
      - Of
      - Analytic
      - Catalog
      - Entry
      - Given
      - Name
  /api/v1/catalog/analytics/{id}:
    get:
      summary: Get an analytic catalog entry by id.
      description: Returns the analytic catalog entry with the given id.
      operationId: retrieveAnalyticCatalogEntryById
      x-api-path-slug: apiv1cataloganalyticsid-get
      parameters:
      - in: path
        name: id
        description: analytic catalog entry id
      responses:
        2:
          description: Successful response
      tags:
      - Analytic
      - Catalog
      - Entry
      - By
      - Id
    put:
      summary: Update an analytic catalog entry by id.
      description: The analytic catalog entry with the given id will be updated.
      operationId: updateAnalyticCatalogEntry
      x-api-path-slug: apiv1cataloganalyticsid-put
      parameters:
      - in: body
        name: body
        description: analytic catalog entry
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: id
        description: analytic catalog entry id
      responses:
        2:
          description: Successful response
      tags:
      - Analytic
      - Catalog
      - Entry
      - By
      - Id
    delete:
      summary: Delete an analytic catalog entry by id.
      description: Deletes the analytic catalog entry with the given id.
      operationId: deleteAnalyticCatalogEntryById
      x-api-path-slug: apiv1cataloganalyticsid-delete
      parameters:
      - in: path
        name: id
        description: analytic catalog entry id
      responses:
        2:
          description: Successful response
      tags:
      - Analytic
      - Catalog
      - Entry
      - By
      - Id
  /api/v1/catalog/analytics/{id}/artifacts:
    get:
      summary: Get the descriptive information of the artifacts corresponding to an
        analytic catalog entry.
      description: 'Returns the description information (type, description, etc.)
        for all artifacts associated with the given analytic catalog entry id. Note:
        it does not return the artifact file contents; use the download APIs to obtain
        an artifact file. An error is returned if the supplied analytic catalog entry
        id does not exist.'
      operationId: retrieveArtifactsByCatalogEntryId
      x-api-path-slug: apiv1cataloganalyticsidartifacts-get
      parameters:
      - in: path
        name: id
        description: analytic catalog entry id
      responses:
        2:
          description: Successful response
      tags:
      - Descriptive
      - Information
      - Of
      - Artifacts
      - Corresponding
      - To
      - Analytic
      - Catalog
      - Entry
  /api/v1/catalog/analytics/{id}/deployment:
    post:
      summary: Deploy an analytic with an optional deployment configuration by analytic
        catalog entry id.
      description: This operation FORCE deploys the specified analytic into the Cloud
        Foundry environment with an optional deployment configuration, responds with
        the request id (generated for the request), and the current request status.  The
        force deploy usually takes longer than the standard timeout, so the calling
        process should use the returned request id to monitor the request status and
        to retrieve the deployment results.
      operationId: deployAnalytic
      x-api-path-slug: apiv1cataloganalyticsiddeployment-post
      parameters:
      - in: body
        name: body
        description: deployment configuration
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: id
        description: analytic catalog entry id
      responses:
        2:
          description: Successful response
      tags:
      - Deploy
      - Analytic
      - Optional
      - Deployment
      - Configuration
      - By
      - Analytic
      - Catalog
      - Entry
      - Id
  /api/v1/catalog/analytics/{id}/deployment/{requestId}:
    get:
      summary: Get the analytic deployment status by request id.
      description: Returns the analytic deployment status (one of 'queued,' 'processing,'
        or 'completed').
      operationId: retrieveAnalyticDeploymentResult
      x-api-path-slug: apiv1cataloganalyticsiddeploymentrequestid-get
      parameters:
      - in: path
        name: id
        description: analytic id
      - in: path
        name: requestId
        description: analytic deployment request id
      responses:
        2:
          description: Successful response
      tags:
      - Analytic
      - Deployment
      - Status
      - By
      - Request
      - Id
  /api/v1/catalog/analytics/{id}/execution:
    post:
      summary: Execute an analytic by analytic catalog entry id.
      description: This operation executes the specified analytic and responds with
        the result produced by analytic.
      operationId: executeAnalytic
      x-api-path-slug: apiv1cataloganalyticsidexecution-post
      parameters:
      - in: body
        name: body
        description: request payload containing analytic input data
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: id
        description: analytic catalog entry id
      - in: query
        name: inputId
        description: test artifact id
      responses:
        2:
          description: Successful response
      tags:
      - Execute
      - Analytic
      - By
      - Analytic
      - Catalog
      - Entry
      - Id
  /api/v1/catalog/analytics/{id}/logs:
    get:
      summary: Get the analytic recent logs
      description: Return the recent analytic logs
      operationId: retrieveAnalyticLog
      x-api-path-slug: apiv1cataloganalyticsidlogs-get
      parameters:
      - in: path
        name: id
        description: analytic id
      responses:
        2:
          description: Successful response
      tags:
      - Analytic
      - Recent
      - Logs
  /api/v1/catalog/analytics/{id}/validation:
    post:
      summary: Validate an analytic by analytic catalog entry id.
      description: This operation FORCE deploys the specified analytic into the Cloud
        Foundry environment, runs the analytic and responds with the validation request
        id (generated for the request), and the current request status.  The force
        deploy usually takes longer than the standard timeout, so the calling process
        should use the returned validation request id to monitor the request status
        and to retrieve the validation results.
      operationId: validateAnalytic
      x-api-path-slug: apiv1cataloganalyticsidvalidation-post
      parameters:
      - in: body
        name: body
        description: request payload containing analytic input data
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: id
        description: analytic catalog entry id
      - in: query
        name: inputId
        description: test artifact id
      responses:
        2:
          description: Successful response
      tags:
      - Validate
      - Analytic
      - By
      - Analytic
      - Catalog
      - Entry
      - Id
    delete:
      summary: Undeploy test analytics.
      description: This operation un-deploys the analytic app from the Cloud Foundry
        environment only if the analytic has been validated for testing purposes.
        This api will not un-deploy production analytics.
      operationId: invalidateAnalytic
      x-api-path-slug: apiv1cataloganalyticsidvalidation-delete
      parameters:
      - in: path
        name: id
        description: analytic catalog entry id
      responses:
        2:
          description: Successful response
      tags:
      - Undeploy
      - Test
      - Analytics
  /api/v1/catalog/analytics/{id}/validation/{validationRequestId}:
    get:
      summary: Get the analytic validation status by validation request id.
      description: Returns the analytic validation status (one of 'queued,' 'processing,'
        or 'completed' and the result from running the analytic (when status is 'completed').
      operationId: retrieveAnalyticValidationResult
      x-api-path-slug: apiv1cataloganalyticsidvalidationvalidationrequestid-get
      parameters:
      - in: path
        name: id
        description: analytic id
      - in: path
        name: validationRequestId
        description: analytic validation request id
      responses:
        2:
          description: Successful response
      tags:
      - Analytic
      - Validation
      - Status
      - By
      - Validation
      - Request
      - Id
  /api/v1/catalog/analytics/{name}/versions:
    delete:
      summary: Delete all versions of the named analytic.
      description: Given the name of an analytic, this API deletes all its versions.
      operationId: deleteAllVersions
      x-api-path-slug: apiv1cataloganalyticsnameversions-delete
      parameters:
      - in: path
        name: name
        description: analytic name
      responses:
        2:
          description: Successful response
      tags:
      - Versions
      - Of
      - Named
      - Analytic
  /api/v1/catalog/artifacts:
    post:
      summary: Upload an artifact and attach it to an analytic catalog entry.
      description: Upload a single artifact file in a multipart MIME structure and
        attach it to an analytic catalog entry. The multipart MIME structure must
        have the catalog entry id tagged as 'catalogEntryId',  the file contents tagged
        as 'file',  the artifact type tagged as 'type', and  a description (under
        1024 characters) tagged as 'description'. Artifact types can be any string.  Artifacts
        with the type 'executable' must contain the executable for the analytic.   An
        analytic can only have 1 artifact labelled as 'executable'(See the documentation
        for more information regarding these files.)
      operationId: uploadAnalyticArtifact
      x-api-path-slug: apiv1catalogartifacts-post
      parameters:
      - in: formData
        name: catalogEntryId
        description: (Required) analytic catalog entry id
      - in: formData
        name: description
        description: artifact description
      - in: formData
        name: file
        description: (Required) artifact file
      - in: formData
        name: type
        description: (Required) artifact type
      responses:
        2:
          description: Successful response
      tags:
      - Upload
      - Artifact
      - Attach
      - It
      - To
      - Analytic
      - Catalog
      - Entry
  /api/v1/catalog/artifacts/{id}:
    put:
      summary: Update an artifact by id.
      description: 'Update an artifact in the catalog with the contents of the supplied
        multipart MIME structure. The multipart MIME structure may have any of the
        following: new file contents tagged as ''file'',  a new artifact type tagged
        as ''type'', and  a new description (under 1024 characters) tagged as ''description''.
        Artifact types can be any string.  Artifacts with the type ''executable''
        must contain the executable for the analytic.   An analytic can only have
        1 artifact labelled as ''executable'' (See the documentation for more information
        regarding these files.)'
      operationId: updateAnalyticArtifact
      x-api-path-slug: apiv1catalogartifactsid-put
      parameters:
      - in: formData
        name: description
        description: artifact description
      - in: formData
        name: file
        description: artifact file
      - in: path
        name: id
        description: artifact id
      - in: formData
        name: type
        description: artifact type
      responses:
        2:
          description: Successful response
      tags:
      - Artifact
      - By
      - Id
    delete:
      summary: Delete an artifact by id.
      description: Deletes the artifact by artifact id.
      operationId: deleteAnalyticArtifact
      x-api-path-slug: apiv1catalogartifactsid-delete
      parameters:
      - in: path
        name: id
        description: artifact id
      responses:
        2:
          description: Successful response
      tags:
      - Artifact
      - By
      - Id
  /api/v1/catalog/artifacts/{id}/file:
    get:
      summary: Download an artifact file by id.
      description: The file is downloaded as an octet-stream.
      operationId: downloadAnalyticArtifact
      x-api-path-slug: apiv1catalogartifactsidfile-get
      parameters:
      - in: path
        name: id
        description: artifact id
      responses:
        2:
          description: Successful response
      tags:
      - Download
      - Artifact
      - File
      - By
      - Id
  /api/v1/catalog/taxonomy:
    get:
      summary: Retrieve the full taxonomy.
      description: This operation retrieves the full taxonomy structure from the catalog.
      operationId: retrieveFullTaxonomy
      x-api-path-slug: apiv1catalogtaxonomy-get
      responses:
        2:
          description: Successful response
      tags:
      - Retrieve
      - Full
      - Taxonomy
    post:
      summary: Load a taxonomy.
      description: This operation loads the supplied taxonomy structure into catalog.
        If a taxonomy already exists in the catalog, new paths in the supplied structure
        will be added. It will not delete existing paths.
      operationId: loadTaxonomy
      x-api-path-slug: apiv1catalogtaxonomy-post
      parameters:
      - in: body
        name: body
        description: taxonomy JSON request
        schema:
          $ref: '#/definitions/holder'
      responses:
        2:
          description: Successful response
      tags:
      - Load
      - Taxonomy
  /api/v1/analytics/customdata/healthcheck:
    get:
      summary: Healthcheck for custom datasource.
      description: Indicates whether custom data connector is up and running.
      operationId: healthcheck
      x-api-path-slug: apiv1analyticscustomdatahealthcheck-get
      responses:
        2:
          description: Successful response
        200:
          description: Successful response
      tags:
      - Healthcheckcustom
      - Datasource
  /api/v1/analytics/customdata/read:
    post:
      summary: Retrieve analytic input data from custom datasource.
      description: Returns the analytic input data used during runtime execution.
      operationId: readCustomProviderData
      x-api-path-slug: apiv1analyticscustomdataread-post
      parameters:
      - in: body
        name: body
        description: Analytic Input Data Read request
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: Successful response
      tags:
      - Retrieve
      - Analytic
      - Input
      - Data
      - From
      - Custom
      - Datasource
  /api/v1/analytics/customdata/write:
    post:
      summary: Write analytic output data to custom datasource.
      description: Writes analytic output data generated during runtime execution.
      operationId: writeCustomProviderData
      x-api-path-slug: apiv1analyticscustomdatawrite-post
      parameters:
      - in: body
        name: body
        description: Analytic Output Data Write Request
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: Successful response
      tags:
      - Write
      - Analytic
      - Output
      - Data
      - To
      - Custom
      - Datasource
  /api/v1/execution:
    post:
      summary: Execute the specified orchestration.
      description: To successfully execute the orchestration, the OrchestrationRequest
        must contain valid orchestration id, bpmn workflow xml and optionally input
        data for each analytic step defined in the workflow.
      operationId: run
      x-api-path-slug: apiv1execution-post
      parameters:
      - in: body
        name: body
        description: orchestration execution request
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: Successful response
      tags:
      - Execute
      - Specified
      - Orchestration
  /api/v1/monitoring/orchestrations/{orchestrationRequestId}:
    get:
      summary: Retrieve orchestration execution result
      description: Returns orchestration execution result for the given orchestration
        request id.
      operationId: retrieveOrchestrationResult
      x-api-path-slug: apiv1monitoringorchestrationsorchestrationrequestid-get
      parameters:
      - in: header
        name: Authorization
        description: Authorization
      - in: path
        name: orchestrationRequestId
      - in: header
        name: Predix-Zone-Id
        description: Predix-Zone-Id
      responses:
        200:
          description: Successful response
      tags:
      - Retrieve
      - Orchestration
      - Execution
      - Result
  /api/v1/scheduler/jobs:
    get:
      summary: Get all job definition entries.
      description: Returns all job definition entries as specified by page and sort
        criteria.
      operationId: retrieveAllJobs
      x-api-path-slug: apiv1schedulerjobs-get
      parameters:
      - in: header
        name: Authorization
        description: Authorization
      - in: query
        name: page
        description: 'page index : zero-based page index'
      - in: header
        name: Predix-Zone-Id
        description: Predix-Zone-Id
      - in: query
        name: size
        description: 'page size : between 1 and 1000 inclusive'
      - in: query
        name: sortOrder
        description: 'sort order : asc | desc'
      responses:
        200:
          description: Successful response
      tags:
      - Job
      - Definition
      - Entries
    post:
      summary: Create a scheduler job.
      description: Creates the scheduler job with a generated id. Set the state value
        to 'Active' to start the job. Set the state value to 'Inactive' to avoid starting
        the job.
      operationId: createJob
      x-api-path-slug: apiv1schedulerjobs-post
      parameters:
      - in: header
        name: Authorization
        description: Authorization
      - in: header
        name: Predix-Zone-Id
        description: Predix-Zone-Id
      - in: header
        name: Refresh-Token-For-Job-Execution
        description: Refresh-Token-For-Job-Execution
      responses:
        200:
          description: Successful response
      tags:
      - Scheduler
      - Job
  /api/v1/scheduler/jobs/{id}:
    get:
      summary: Get a scheduler job by id.
      description: Returns the scheduler job with the given id.
      operationId: retrieveJob
      x-api-path-slug: apiv1schedulerjobsid-get
      parameters:
      - in: header
        name: Authorization
        description: Authorization
      - in: path
        name: id
        description: Job id
      - in: header
        name: Predix-Zone-Id
        description: Predix-Zone-Id
      responses:
        200:
          description: Successful response
      tags:
      - Scheduler
      - Job
      - By
      - Id
    put:
      summary: Update an existing scheduler job.
      description: Updates the scheduled job. The updated changes will be effective
        from the next scheduling of this job. To suspend a job, update the job with
        state value 'Inactive'. To resume a job, update the job with state value 'Active'.
      operationId: updateJob
      x-api-path-slug: apiv1schedulerjobsid-put
      parameters:
      - in: header
        name: Authorization
        description: Authorization
      - in: path
        name: id
      - in: header
        name: Predix-Zone-Id
        description: Predix-Zone-Id
      - in: header
        name: Refresh-Token-For-Job-Execution
        description: Refresh-Token-For-Job-Execution
      responses:
        200:
          description: Successful response
      tags:
      - Existing
      - Scheduler
      - Job
    delete:
      summary: Delete job definition.
      description: Delete job definition for the given job id.
      operationId: deleteJob
      x-api-path-slug: apiv1schedulerjobsid-delete
      parameters:
      - in: header
        name: Authorization
        description: Authorization
      - in: path
        name: id
        description: Job id
      - in: header
        name: Predix-Zone-Id
        description: Predix-Zone-Id
      responses:
        200:
          description: Successful response
      tags:
      - Job
      - Definition
  /api/v1/scheduler/jobs/{id}/history:
    get:
      summary: Retrieve job execution history of the given job.
      description: Retrieve job execution history
      operationId: retrieveJobHistory
      x-api-path-slug: apiv1schedulerjobsidhistory-get
      parameters:
      - in: header
        name: Authorization
        description: Authorization
      - in: query
        name: endTime
        description: End time in millis
      - in: path
        name: id
        description: Job id
      - in: header
        name: Predix-Zone-Id
        description: Predix-Zone-Id
      - in: query
        name: startTime
        description: Start time in millis
      responses:
        200:
          description: Successful response
      tags:
      - Retrieve
      - Job
      - Execution
      - History
      - Of
      - Given
      - Job
  /api/v2/config/orchestrations:
    get:
      summary: Get all orchestration configuration entries.
      description: Returns all orchestration configuration entries as specified by
        page and sort criteria.
      operationId: retrieveAllOrchConfigs
      x-api-path-slug: apiv2configorchestrations-get
      parameters:
      - in: header
        name: Authorization
        description: Authorization
      - in: query
        name: page
        description: 'page index : zero-based page index'
      - in: header
        name: Predix-Zone-Id
        description: Predix-Zone-Id
      - in: query
        name: size
        description: 'page size : between 1 and 1000 inclusive'
      - in: query
        name: sortableFields
        description: 'sortable fields : name'
      - in: query
        name: sortOrder
        description: 'sort order : asc | desc'
      responses:
        200:
          description: Successful response
      tags:
      - Orchestration
      - Configuration
      - Entries
    post:
      summary: Create an orchestration configuration entry.
      description: Creates the orchestration configuration entry with a generated
        id.
      operationId: createOrchestrationEntry
      x-api-path-slug: apiv2configorchestrations-post
      parameters:
      - in: header
        name: Authorization
        description: Authorization
      - in: body
        name: body
        description: orchestration configuration entry
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Predix-Zone-Id
        description: Predix-Zone-Id
      responses:
        200:
          description: Successful response
      tags:
      - Orchestration
      - Configuration
      - Entry
  /api/v2/config/orchestrations/artifacts:
    post:
      summary: Upload an artifact and attach it to an orchestration configuration
        entry.
      description: Upload a single artifact file in a multipart MIME structure and
        attach it to an orchestration configuration entry. The multipart MIME structure
        must have the orchestration entry id tagged as 'orchestrationEntryId',  the
        file contents tagged as 'file',  the artifact type tagged as 'type', and  the
        name of artifact tagged as 'name'.  A description (under 1024 characters)
        tagged as 'description' can be optionally specified. Artifact types can be
        either 'portToFieldMap', 'bpmn' or any.   If the artifact type is 'portToFieldMap',
        specify the orchestration step ID tagged as 'stepId'.   Otherwise, 'name'
        will be used as 'stepId'.  (See the documentation for more information regarding
        these files.)
      operationId: uploadOrchConfigArtifact
      x-api-path-slug: apiv2configorchestrationsartifacts-post
      parameters:
      - in: header
        name: Authorization
        description: Authorization
      - in: formData
        name: description
        description: Artifact description
      - in: formData
        name: file
        description: (Required) Artifact file
      - in: formData
        name: name
        description: (Required) Artifact name
      - in: formData
        name: orchestrationEntryId
        description: (Required) orchestration configuration entry id
      - in: header
        name: Predix-Zone-Id
        description: Predix-Zone-Id
      - in: formData
        name: stepId
        description: Orchestration Step ID
      - in: formData
        name: type
        description: (Required) Artifact type
      responses:
        200:
          description: Successful response
      tags:
      - Upload
      - Artifact
      - Attach
      - It
      - To
      - Orchestration
      - Configuration
      - Entry
  /api/v2/config/orchestrations/artifacts/{id}:
    put:
      summary: Update an artifact by id.
      description: Update the artifact of the orchestration configuration with the
        contents of the supplied multipart MIME structure. The multipart MIME structure
        may have new file contents tagged as 'file',  new artifact type tagged as
        'type',  new name of artifact tagged as 'name',  new description (under 1024
        characters) tagged as 'description', and  new value of the orchestration step
        id tagged as 'stepId.   Artifact types can be either 'portToFieldMap', 'bpmn'
        or any.  (See the documentation for more information regarding these files.)
      operationId: updateOrchConfigArtifact
      x-api-path-slug: apiv2configorchestrationsartifactsid-put
      parameters:
      - in: header
        name: Authorization
        description: Authorization
      - in: formData
        name: description
        description: Artifact description
      - in: formData
        name: file
        description: Artifact file
      - in: path
        name: id
        description: Artifact id
      - in: formData
        name: name
        description: Artifact name
      - in: header
        name: Predix-Zone-Id
        description: Predix-Zone-Id
      - in: formData
        name: stepId
        description: Orchestration Step ID
      - in: formData
        name: type
        description: Artifact type
      responses:
        200:
          description: Successful response
      tags:
      - Artifact
      - By
      - Id
    delete:
      summary: Delete an orchestration artifact by id.
      description: Delete the orchestration artifact by artifact id.
      operationId: deleteOrchConfigArtifact
      x-api-path-slug: apiv2configorchestrationsartifactsid-delete
      parameters:
      - in: header
        name: Authorization
        description: Authorization
      - in: path
        name: id
        description: Artifact id
      - in: header
        name: Predix-Zone-Id
        description: Predix-Zone-Id
      responses:
        200:
          description: Successful response
      tags:
      - Orchestration
      - Artifact
      - By
      - Id
  /api/v2/config/orchestrations/artifacts/{id}/file:
    get:
      summary: Download an orchestration artifact file by id.
      description: The file is downloaded as an octet-stream.
      operationId: downloadOrchConfigArtifact
      x-api-path-slug: apiv2configorchestrationsartifactsidfile-get
      parameters:
      - in: header
        name: Authorization
        description: Authorization
      - in: path
        name: id
        description: Artifact id
      - in: header
        name: Predix-Zone-Id
        description: Predix-Zone-Id
      responses:
        200:
          description: Successful response
      tags:
      - Download
      - Orchestration
      - Artifact
      - File
      - By
      - Id
  /api/v2/config/orchestrations/defaulttagquery:
    get:
      summary: Get the default tag query corresponding for the tenant.
      description: Returns all information (query string, fieldnamespecifier, tagnamespecifer,
        description etc.) associated with the default tag query. An error is returned
        if tag query does not exist for the tenant.
      operationId: retrieveDefaultTagQuery
      x-api-path-slug: apiv2configorchestrationsdefaulttagquery-get
      parameters:
      - in: header
        name: Authorization
        description: Authorization
      - in: header
        name: Predix-Zone-Id
        description: Predix-Zone-Id
      responses:
        200:
          description: Successful response
      tags:
      - Default
      - Tag
      - Query
      - Correspondingthe
      - Tenant
    post:
      summary: Create the default tag query corresponding for the tenant.
      description: Creates the default tag query including all information (query
        string, fieldnamespecifier, tagnamespecifer, description etc.) associated
        with the query.
      operationId: createDefaultTagQuery
      x-api-path-slug: apiv2configorchestrationsdefaulttagquery-post
      parameters:
      - in: header
        name: Authorization
        description: Authorization
      - in: body
        name: body
        description: tag names default query
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Predix-Zone-Id
        description: Predix-Zone-Id
      responses:
        200:
          description: Successful response
      tags:
      - Default
      - Tag
      - Query
      - Correspondingthe
      - Tenant
    put:
      summary: Update the default tag query for the tenant.
      description: Updates the default tag query including all information (query
        string, fieldnamespecifier, tagnamespecifer, description etc.) associated
        with the query.
      operationId: updateDefaultTagQuery
      x-api-path-slug: apiv2configorchestrationsdefaulttagquery-put
      parameters:
      - in: header
        name: Authorization
        description: Authorization
      - in: body
        name: body
        description: tag names default query
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Predix-Zone-Id
        description: Predix-Zone-Id
      responses:
        200:
          description: Successful response
      tags:
      - Default
      - Tag
      - Querythe
      - Tenant
    delete:
      summary: Delete the default tag query for the tenant.
      description: Deletes the default tag query.
      operationId: deleteDefaultTagQuery
      x-api-path-slug: apiv2configorchestrationsdefaulttagquery-delete
      parameters:
      - in: header
        name: Authorization
        description: Authorization
      - in: header
        name: Predix-Zone-Id
        description: Predix-Zone-Id
      responses:
        200:
          description: Successful response
      tags:
      - Default
      - Tag
      - Querythe
      - Tenant
  /api/v2/config/orchestrations/models:
    get:
      summary: Get all model entries.
      description: Returns all model entries as specified by page and sort criteria.
        By default, retrieves all models for tenant. If additional query params specified,
        then results will be filtered
      operationId: retrieveAllModels
      x-api-path-slug: apiv2configorchestrationsmodels-get
      parameters:
      - in: header
        name: Authorization
        description: Authorization
      - in: query
        name: modelKey
        description: Model Key
      - in: query
        name: modelName
        description: Model Name
      - in: query
        name: modelVersion
        description: Model Version
      - in: query
        name: page
        description: 'page index : zero-based page index'
      - in: header
        name: Predix-Zone-Id
        description: Predix-Zone-Id
      - in: query
        name: size
        description: 'page size : between 1 and 1000 inclusive'
      responses:
        200:
          description: Successful response
      tags:
      - Model
      - Entries
    post:
      summary: Upload a model.
      description: Upload a model in a multipart MIME structure. The multipart MIME
        structure must have the modelKey  tagged as 'modelKey',  the modelName  tagged
        as 'modelName',  the modelVersion  tagged as 'modelVersion',  the file contents
        tagged as 'file',  a description (under 1024 characters) tagged as 'description'.
        (See the documentation for more information regarding these files.)
      operationId: uploadModel
      x-api-path-slug: apiv2configorchestrationsmodels-post
      parameters:
      - in: header
        name: Authorization
        description: Authorization
      - in: formData
        name: description
        description: Artifact description
      - in: formData
        name: file
        description: (Required) Model file
      - in: formData
        name: modelKey
        description: (Required) Model Key
      - in: formData
        name: modelName
        description: (Required) Model Name
      - in: formData
        name: modelVersion
        description: (Required) Model Version
      - in: header
        name: Predix-Zone-Id
        description: Predix-Zone-Id
      responses:
        200:
          description: Successful response
      tags:
      - Upload
      - Model
  /api/v2/config/orchestrations/models/{id}:
    put:
      summary: Update model by id.
      description: Update a model with attributes of the supplied multipart MIME structure.
        The multipart MIME structure must have the modelKey  tagged as 'modelKey',  the
        modelName  tagged as 'modelName',  the modelVersion  tagged as 'modelVersion',  the
        file contents tagged as 'file',  a description (under 1024 characters) tagged
        as 'description'. (See the documentation for more information regarding these
        files.)
      operationId: updateModel
      x-api-path-slug: apiv2configorchestrationsmodelsid-put
      parameters:
      - in: header
        name: Authorization
        description: Authorization
      - in: formData
        name: description
        description: Artifact description
      - in: formData
        name: file
        description: (Required) Model file
      - in: path
        name: id
        description: artifact id
      - in: formData
        name: modelKey
        description: (Required) Model Key
      - in: formData
        name: modelName
        description: (Required) Model Name
      - in: formData
        name: modelVersion
        description: (Required) Model Version
      - in: header
        name: Predix-Zone-Id
        description: Predix-Zone-Id
      responses:
        200:
          description: Successful response
      tags:
      - Model
      - By
      - Id
    delete:
      summary: Delete a model by id.
      description: Delete a model by model id.
      operationId: deleteModel
      x-api-path-slug: apiv2configorchestrationsmodelsid-delete
      parameters:
      - in: header
        name: Authorization
        description: Authorization
      - in: path
        name: id
        description: Model id
      - in: header
        name: Predix-Zone-Id
        description: Predix-Zone-Id
      responses:
        200:
          description: Successful response
      tags:
      - Model
      - By
      - Id
  /api/v2/config/orchestrations/models/{id}/file:
    get:
      summary: Download a model file by id.
      description: The file is downloaded as an octet-stream.
      operationId: downloadModel
      x-api-path-slug: apiv2configorchestrationsmodelsidfile-get
      parameters:
      - in: header
        name: Authorization
        description: Authorization
      - in: path
        name: id
        description: Model id
      - in: header
        name: Predix-Zone-Id
        description: Predix-Zone-Id
      responses:
        200:
          description: Successful response
      tags:
      - Download
      - Model
      - File
      - By
      - Id
  /api/v2/config/orchestrations/{id}:
    get:
      summary: Get an orchestration configuration entry by id.
      description: Returns the orchestration configuration entry with the given id.
      operationId: retrieveOrchestrationEntryById
      x-api-path-slug: apiv2configorchestrationsid-get
      parameters:
      - in: header
        name: Authorization
        description: Authorization
      - in: path
        name: id
        description: orchestration configuration entry id
      - in: header
        name: Predix-Zone-Id
        description: Predix-Zone-Id
      responses:
        200:
          description: Successful response
      tags:
      - Orchestration
      - Configuration
      - Entry
      - By
      - Id
    put:
      summary: Update an existing orchestration configuration entry.
      description: Updates the orchestration configuration entry with given orchestration
        configuration.
      operationId: updateOrchestrationEntry
      x-api-path-slug: apiv2configorchestrationsid-put
      parameters:
      - in: header
        name: Authorization
        description: Authorization
      - in: body
        name: body
        description: orchestration configuration entry
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: id
        description: orchestration configuration id
      - in: header
        name: Predix-Zone-Id
        description: Predix-Zone-Id
      responses:
        200:
          description: Successful response
      tags:
      - Existing
      - Orchestration
      - Configuration
      - Entry
    delete:
      summary: Delete an orchestration configuration entry by id.
      description: Deletes the orchestration configuration entry with the given id.
      operationId: deleteOrchestrationEntryById
      x-api-path-slug: apiv2configorchestrationsid-delete
      parameters:
      - in: header
        name: Authorization
        description: Authorization
      - in: path
        name: id
        description: orchestration configuration entry id
      - in: header
        name: Predix-Zone-Id
        description: Predix-Zone-Id
      responses:
        200:
          description: Successful response
      tags:
      - Orchestration
      - Configuration
      - Entry
      - By
      - Id
  /api/v2/config/orchestrations/{id}/artifacts:
    get:
      summary: Get the descriptive information of the orchestration artifacts corresponding
        to an orchestration configuration entry.
      description: 'Returns the description information (type, description, etc.)
        for all orchestration artifacts associated with the given configuration entry
        id. Note: it does not return the orchestration artifact file contents; use
        the download APIs to obtain an artifact file. An error is returned if the
        supplied orchestration configuration entry id does not exist.'
      operationId: retrieveArtifactsByOrchestrationEntryId
      x-api-path-slug: apiv2configorchestrationsidartifacts-get
      parameters:
      - in: header
        name: Authorization
        description: Authorization
      - in: path
        name: id
        description: orchestration configuration entry id
      - in: header
        name: Predix-Zone-Id
        description: Predix-Zone-Id
      responses:
        200:
          description: Successful response
      tags:
      - Descriptive
      - Information
      - Of
      - Orchestration
      - Artifacts
      - Corresponding
      - To
      - Orchestration
      - Configuration
      - Entry
  /api/v2/config/orchestrations/{id}/file:
    get:
      summary: Download an orchestration artifact file by orchestration id and artifact
        type.
      description: The file is downloaded as an octet-stream. If the type is bpmn,
        then then bpmn xml is downloaded. If the type is portToFieldMap, then the
        system expects analyticStepId to download the portToFieldMap for the given
        step
      operationId: downloadArtifactByType
      x-api-path-slug: apiv2configorchestrationsidfile-get
      parameters:
      - in: header
        name: Authorization
        description: Authorization
      - in: path
        name: id
        description: orchestration configuration entry id
      - in: query
        name: name
        description: artifact name (analytic step id)
      - in: header
        name: Predix-Zone-Id
        description: Predix-Zone-Id
      - in: query
        name: type
        description: artifact type (Ex
      responses:
        200:
          description: Successful response
      tags:
      - Download
      - Orchestration
      - Artifact
      - File
      - By
      - Orchestration
      - Id
      - Artifact
      - Type
  /api/v2/execution:
    post:
      summary: Execute the specified orchestration.
      description: To successfully execute the orchestration, the OrchestrationExecutionRequest
        must contain valid orchestration id, asset id, asset data field mapping details.
        This API will execute the orchestration in synchronous mode and if the execution
        is not completed  in 1 minute then the request will fail. After successful
        completion, the response will contain each orchestration steps output data.
      operationId: runSyncV2
      x-api-path-slug: apiv2execution-post
      parameters:
      - in: body
        name: body
        description: orchestration execution request
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: Successful response
      tags:
      - Execute
      - Specified
      - Orchestration
  /api/v2/execution/async:
    post:
      summary: Execute the specified orchestration in asynchronous mode.
      description: To successfully execute the orchestration, the OrchestrationExecutionRequest
        must contain valid orchestration id, asset id, asset data field mapping details.
      operationId: runAsync
      x-api-path-slug: apiv2executionasync-post
      parameters:
      - in: body
        name: body
        description: orchestration execution request
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: Successful response
      tags:
      - Execute
      - Specified
      - Orchestration
      - In
      - Asynchronous
      - Mode
  /api/v2/execution/orchestrations/{orchConfigId}/deployment:
    post:
      summary: Deploy the specified orchestration workflow file to the Orchestration
        Engine.
      description: This API will deploy the BPMN file associated with the specified
        orchestration configuration to the Orchestration Engine in preparation for
        orchestration execution.
      operationId: retrieveAndDeployBpmn
      x-api-path-slug: apiv2executionorchestrationsorchconfigiddeployment-post
      parameters:
      - in: path
        name: orchConfigId
        description: orchestration configuration id
      responses:
        200:
          description: Successful response
      tags:
      - Deploy
      - Specified
      - Orchestration
      - Workflow
      - File
      - To
      - Orchestration
      - Engine
  /api/v2/execution/testrun:
    post:
      summary: Execute the orchestration with given bpmn and input data.
      description: To successfully execute the orchestration, the request must contain
        valid bpmn20.xml, input data for each step in the bpmn.
      operationId: testRun
      x-api-path-slug: apiv2executiontestrun-post
      parameters:
      - in: formData
        name: bpmn
        description: BPMN file
      - in: formData
        name: input
        description: Input data file
      responses:
        200:
          description: Successful response
      tags:
      - Execute
      - Orchestration
      - Given
      - Bpmn
      - Input
      - Data
  /api/v2/execution/validation:
    post:
      summary: Validate the specified orchestration and the health of all the analytics
        used in the orchestration.
      description: To successfully validate the orchestration, the BPMN XML file must
        reference analytics that are running. The validation will call a 'healthCheck'
        entry on each analytic.  Analytics in the platform automatically have this
        entry, analytics outside the platform must implement this APIfor their validation
        to pass.  The results contain the http status for each for the healthCheck
        call to each analytic.
      operationId: validate
      x-api-path-slug: apiv2executionvalidation-post
      parameters:
      - in: body
        name: file
        description: (Required) artifact file
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: Successful response
      tags:
      - Validate
      - Specified
      - Orchestration
      - Health
      - Of
      - ""
      - Analytics
      - Used
      - In
      - Orchestration
  /apps:
    get:
      summary: Get all the registered microapps
      description: Get the registered microapps for the given tenant
      operationId: getAllRegisteredAppsUsingGET
      x-api-path-slug: apps-get
      responses:
        200:
          description: OK
      tags:
      - Apps
    post:
      summary: Register the microapp
      description: Register the microapps
      operationId: registerAppUsingPOST
      x-api-path-slug: apps-post
      parameters:
      - in: body
        name: request
        description: request
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Apps
    put:
      summary: Update the microapp
      description: Update the microapps
      operationId: updateAppUsingPUT
      x-api-path-slug: apps-put
      parameters:
      - in: body
        name: request
        description: request
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Apps
  /apps/{uuid}:
    get:
      summary: Get the registered microapp
      description: Get the registered microapp for the given uri
      operationId: getRegisterAppUsingGET
      x-api-path-slug: appsuuid-get
      parameters:
      - in: path
        name: uuid
        description: uuid
      responses:
        200:
          description: OK
      tags:
      - Apps
      - Uuid
    delete:
      summary: Unregister the microapp
      description: Unregister the microapp
      operationId: unRegisterAppUsingDELETE
      x-api-path-slug: appsuuid-delete
      parameters:
      - in: path
        name: uuid
        description: uuid
      responses:
        200:
          description: OK
      tags:
      - Apps
      - Uuid
  /globalconfig:
    get:
      summary: Get global config information
      description: Get global config information
      operationId: getGlobalConfigUsingGET
      x-api-path-slug: globalconfig-get
      responses:
        200:
          description: OK
      tags:
      - Globalconfig
    post:
      summary: Save global config information
      description: Save global config information
      operationId: saveGlobalConfigUsingPOST
      x-api-path-slug: globalconfig-post
      parameters:
      - in: body
        name: config
        description: config
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Globalconfig
  /globalconfig/{uuid}:
    put:
      summary: Update global config information
      description: Update global config information
      operationId: updateGlobalConfigUsingPUT
      x-api-path-slug: globalconfiguuid-put
      parameters:
      - in: body
        name: config
        description: config
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: uuid
        description: uuid
      responses:
        200:
          description: OK
      tags:
      - Globalconfig
      - Uuid
    delete:
      summary: Delete global config information
      description: Delete global config information
      operationId: deleteGlobalConfigUsingDELETE
      x-api-path-slug: globalconfiguuid-delete
      parameters:
      - in: path
        name: uuid
        description: uuid
      responses:
        200:
          description: OK
      tags:
      - Globalconfig
      - Uuid
  /preferences:
    get:
      summary: Get the preferences information
      description: Get the preferences information
      operationId: getPreferenceUsingGET
      x-api-path-slug: preferences-get
      responses:
        200:
          description: OK
      tags:
      - Preferences
    post:
      summary: Save the preferences information
      description: save the preferences information
      operationId: savePreferenceUsingPOST
      x-api-path-slug: preferences-post
      parameters:
      - in: body
        name: request
        description: request
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Preferences
  /preferences/{uuid}:
    put:
      summary: Update the preferences information
      description: Update the preferences information
      operationId: updatePreferenceUsingPUT
      x-api-path-slug: preferencesuuid-put
      parameters:
      - in: body
        name: request
        description: request
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: uuid
        description: uuid
      responses:
        200:
          description: OK
      tags:
      - Preferences
      - Uuid
    delete:
      summary: Delete the preferences information
      description: Delete the preferences information
      operationId: deletePreferenceUsingDELETE
      x-api-path-slug: preferencesuuid-delete
      parameters:
      - in: path
        name: uuid
        description: uuid
      responses:
        200:
          description: OK
      tags:
      - Preferences
      - Uuid
  /privileges:
    get:
      summary: Get the privileges information
      description: Get the privileges information
      operationId: getPrivilegeUsingGET
      x-api-path-slug: privileges-get
      responses:
        200:
          description: OK
      tags:
      - Privileges
    post:
      summary: Save the privileges information
      description: Save the privileges information
      operationId: savePrivilegeUsingPOST
      x-api-path-slug: privileges-post
      parameters:
      - in: body
        name: request
        description: request
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Privileges
  /privileges/{uuid}:
    put:
      summary: Update the privileges information
      description: Update the privileges information
      operationId: updatePrivilegeUsingPUT
      x-api-path-slug: privilegesuuid-put
      parameters:
      - in: body
        name: request
        description: request
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: uuid
        description: uuid
      responses:
        200:
          description: OK
      tags:
      - Privileges
      - Uuid
    delete:
      summary: Delete the privileges information
      description: Delete the privileges information
      operationId: deletePrivilegeUsingDELETE
      x-api-path-slug: privilegesuuid-delete
      parameters:
      - in: path
        name: uuid
        description: uuid
      responses:
        200:
          description: OK
      tags:
      - Privileges
      - Uuid
  /provision:
    post:
      summary: postTenantConfig
      description: ""
      operationId: postTenantConfigUsingPOST
      x-api-path-slug: provision-post
      parameters:
      - in: body
        name: tenantConfigReq
        description: tenantConfigReq
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Provision
  /provision/{tenantId}:
    delete:
      summary: deleteTenantConfig
      description: ""
      operationId: deleteTenantConfigUsingDELETE
      x-api-path-slug: provisiontenantid-delete
      parameters:
      - in: path
        name: tenantId
        description: tenantId
      responses:
        200:
          description: OK
      tags:
      - Provision
      - TenantId
  /themes:
    get:
      summary: Get theme information for a tenant
      description: Get theme information
      operationId: getThemeUsingGET
      x-api-path-slug: themes-get
      responses:
        200:
          description: OK
      tags:
      - Themes
    post:
      summary: Save theme config information
      description: Save theme config information
      operationId: saveThemeUsingPOST
      x-api-path-slug: themes-post
      parameters:
      - in: body
        name: theme
        description: theme
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Themes
    put:
      summary: Update theme
      description: Update theme
      operationId: updateThemeUsingPUT
      x-api-path-slug: themes-put
      parameters:
      - in: body
        name: theme
        description: theme
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Themes
  /themes/{uuid}:
    get:
      summary: Get the registered theme by uri
      description: Get the registered theme infromation for the given uri
      operationId: getThemeInfoByIdUsingGET
      x-api-path-slug: themesuuid-get
      parameters:
      - in: path
        name: uuid
        description: uuid
      responses:
        200:
          description: OK
      tags:
      - Themes
      - Uuid
    delete:
      summary: Delete theme
      description: Delete theme
      operationId: deleteThemeUsingDELETE
      x-api-path-slug: themesuuid-delete
      parameters:
      - in: path
        name: uuid
        description: uuid
      responses:
        200:
          description: OK
      tags:
      - Themes
      - Uuid
  /user:
    get:
      summary: Get the current user information
      description: Get the current user information
      operationId: getUserUsingGET
      x-api-path-slug: user-get
      responses:
        200:
          description: OK
      tags:
      - User
    post:
      summary: Save the current user information
      description: Save the current user information
      operationId: saveUserUsingPOST
      x-api-path-slug: user-post
      parameters:
      - in: body
        name: request
        description: request
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - User
  /user/{uuid}:
    put:
      summary: Update the current user information
      description: Update the current user information
      operationId: updateUserUsingPUT
      x-api-path-slug: useruuid-put
      parameters:
      - in: body
        name: request
        description: request
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: uuid
        description: uuid
      responses:
        200:
          description: OK
      tags:
      - User
      - Uuid
    delete:
      summary: Delete the current user information
      description: Delete the current user information
      operationId: deleteUserUsingDELETE
      x-api-path-slug: useruuid-delete
      parameters:
      - in: path
        name: uuid
        description: uuid
      responses:
        200:
          description: OK
      tags:
      - User
      - Uuid
  /v1/:
    get:
      summary: Get a listing of user-defined domain object collections
      description: Returns the names of all user-defined domain object collections
        with counts of domain objects contained.
      operationId: getV1
      x-api-path-slug: v1-get
      responses:
        200:
          description: Successful response
      tags:
      - Listing
      - Of
      - User-defined
      - Domain
      - Object
      - Collections
  /v1/{collection}:
    get:
      summary: Gets all user-defined domain objects.
      description: |-
        This is a user-defined domain object collection.

        You can create your own custom domain objects, add properties to them, define relationships, and so on.
      operationId: getV1Collection
      x-api-path-slug: v1collection-get
      parameters:
      - in: path
        name: collection
        description: Name of the user-defined domain object collection
      - in: query
        name: fields
        description: Fields to be returned from each entity (comma separated)
      - in: query
        name: filter
        description: GEL query filter
      - in: query
        name: pageSize
        description: Limits the number of entities returned
      responses:
        200:
          description: Successful response
      tags:
      - S
      - ""
      - User-defined
      - Domain
      - Objects
    post:
      summary: Create one or more user-defined domain objects
      description: |-
        This is a user-defined domain object collection.

        You can create your own custom domain objects, add properties to them, define relationships, and so on.

        The following characters are not allowed in any attribute names: $ < > : | ( ) , = ! ? &
      operationId: postV1Collection
      x-api-path-slug: v1collection-post
      parameters:
      - in: body
        name: body
        description: Array of entities to create
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: collection
        description: Name of the user-defined domain object collection
      responses:
        200:
          description: Successful response
      tags:
      - More
      - User-defined
      - Domain
      - Objects
  /v1/{collection}/{id}:
    get:
      summary: Get entity based on  uri
      description: |-
        This is a user-defined domain object collection.

        You can create your own custom domain objects, add properties to them, define relationships, and so on.
      operationId: getV1Collection
      x-api-path-slug: v1collectionid-get
      parameters:
      - in: path
        name: collection
        description: Name of the user-defined domain object collection
      - in: query
        name: fields
        description: Fields to be returned from the entity (comma separated)
      - in: path
        name: id
        description: ID of the domain object to retrieve
      responses:
        200:
          description: Successful response
      tags:
      - Entity
      - Based
      - "On"
      - ""
      - Uri
    put:
      summary: Update a user-defined domain object
      description: |-
        This is a user-defined domain object collection.

        You can create your own custom domain objects, add properties to them, define relationships, and so on.

        The following characters are not allowed in any attribute names: $ < > : | ( ) , = ! ? &
      operationId: putV1Collection
      x-api-path-slug: v1collectionid-put
      parameters:
      - in: body
        name: body
        description: Array of one entity to create/update
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: collection
        description: Name of the user-defined domain object collection
      - in: path
        name: id
        description: ID of the domain object to update
      responses:
        200:
          description: Successful response
      tags:
      - User-defined
      - Domain
      - Object
    patch:
      summary: Patch a user-defined domain object
      description: |-
        This is a user-defined domain object collection.

        You can create your own custom domain objects, add properties to them, define relationships, and so on.

        Update specific model using http PATCH requests. Request format should follow JSON PATCH format. Supported operations on each attribute are add, remove, replace, move, copy, test. Refer RFC link for more details on request format. https://tools.ietf.org/html/rfc6902
      operationId: patchV1Collection
      x-api-path-slug: v1collectionid-patch
      parameters:
      - in: body
        name: body
        description: 'Array of patch operations to apply to the domain object (see:
          https://tools'
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: collection
        description: Name of the user-defined domain object collection
      - in: path
        name: id
        description: ID of the domain object to patch
      responses:
        200:
          description: Successful response
      tags:
      - User-defined
      - Domain
      - Object
    delete:
      summary: Delete a user-defined domain object
      description: |-
        This is a user-defined domain object collection.

        You can create your own custom domain objects, add properties to them, define relationships, and so on.
      operationId: deleteV1Collection
      x-api-path-slug: v1collectionid-delete
      parameters:
      - in: path
        name: collection
        description: Name of the user-defined domain object collection
      - in: path
        name: id
        description: ID of the domain object to delete
      responses:
        200:
          description: Successful response
      tags:
      - User-defined
      - Domain
      - Object
  /v1/system/audit:
    get:
      summary: Get domain object audit records.
      description: For detailed documentation of all available query options please
        refer to Predix Asset Documentation.
      operationId: getV1SystemAudit
      x-api-path-slug: v1systemaudit-get
      parameters:
      - in: query
        name: fields
        description: Fields to be returned from the entity (comma separated)
      responses:
        200:
          description: Successful response
      tags:
      - Domain
      - Object
      - Audit
      - Records
  /v1/system/audit/changes:
    get:
      summary: Get property-level audit records.
      description: For detailed documentation of all available query options please
        refer to Predix Asset Documentation.
      operationId: getV1SystemAuditChanges
      x-api-path-slug: v1systemauditchanges-get
      parameters:
      - in: query
        name: fields
        description: Fields to be returned from the entity (comma separated)
      responses:
        200:
          description: Successful response
      tags:
      - Property-level
      - Audit
      - Records
  /v1/system/audit/snapshots:
    get:
      summary: Get a snapshot of an entity at or before a specified datetime (ISO-8601).
      description: For detailed documentation of all available query options please
        refer to Predix Asset Documentation.
      operationId: getV1SystemAuditSnapshots
      x-api-path-slug: v1systemauditsnapshots-get
      parameters:
      - in: query
        name: filter
        description: identifier={entity uri}:{before|eBefore}={ISO-8601 datetime}
      responses:
        200:
          description: Successful response
      tags:
      - Snapshot
      - Of
      - Entity
      - At
      - Before
      - Specified
      - Datetime
      - (ISO-8601)
  /v1/system/configs:
    get:
      summary: Get tenant-specific configuration settings
      description: This can be used to verify whether the audit feature is enabled.
      operationId: getV1SystemConfigs
      x-api-path-slug: v1systemconfigs-get
      responses:
        200:
          description: Successful response
      tags:
      - Tenant-specific
      - Configuration
      - Settings
    post:
      summary: Update tenant-specific configuration settings
      description: This can be used to enable or disable the audit feature.
      operationId: postV1SystemConfigs
      x-api-path-slug: v1systemconfigs-post
      parameters:
      - in: body
        name: body
        description: Array of configs to create
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: Successful response
      tags:
      - Tenant-specific
      - Configuration
      - Settings
  /v1/system/schema/entities/{type}:
    get:
      summary: Get the JSON Schema of the specified entity type
      description: Get the json schema of the specified entity type.
      operationId: getV1SystemSchemaEntitiesType
      x-api-path-slug: v1systemschemaentitiestype-get
      parameters:
      - in: path
        name: type
        description: Entity type (e
      responses:
        200:
          description: Successful response
      tags:
      - JSON
      - Schema
      - Of
      - Specified
      - Entity
      - Type
    put:
      summary: Create or update the JSON Schema of the specified entity type
      description: Create or update the json schema of the specified entity type.
      operationId: putV1SystemSchemaEntitiesType
      x-api-path-slug: v1systemschemaentitiestype-put
      parameters:
      - in: body
        name: body
        description: JSON Schema for the specified entity type
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: type
        description: Entity type (e
      responses:
        200:
          description: Successful response
      tags:
      - Update
      - JSON
      - Schema
      - Of
      - Specified
      - Entity
      - Type
    delete:
      summary: Delete the JSON Schema of the specified entity type
      description: Delete the json schema of the specified entity type.
      operationId: deleteV1SystemSchemaEntitiesType
      x-api-path-slug: v1systemschemaentitiestype-delete
      parameters:
      - in: path
        name: type
        description: Entity type (e
      responses:
        200:
          description: Successful response
      tags:
      - JSON
      - Schema
      - Of
      - Specified
      - Entity
      - Type
  /v1/chaincodes/{chaincodeName}:
    put:
      summary: Put Chaincodes
      description: Deploy chaincode (smart contract) to Blockchain
      operationId: deploy-chaincode-smart-contract-to-blockchain
      x-api-path-slug: v1chaincodeschaincodename-put
      parameters:
      - in: formData
        name: args
        description: args for uploaded script, e
      - in: header
        name: Authorization
        description: access token
      - in: formData
        name: chaincode
        description: upload compressed file (tar
      - in: path
        name: chaincodeName
        description: name of chain code
      - in: header
        name: predix-zone-id
        description: tenantId
      responses:
        200:
          description: OK
      tags:
      - Chaincodes
    get:
      summary: Get Chaincodes
      description: Get a single chaincode
      operationId: get-a-single-chaincode
      x-api-path-slug: v1chaincodeschaincodename-get
      parameters:
      - in: header
        name: Authorization
        description: access token
      - in: path
        name: chaincodeName
        description: name of deployed chain code
      - in: header
        name: predix-zone-id
        description: tenantId
      responses:
        200:
          description: OK
      tags:
      - Chaincodes
  /v1/chaincodes:
    get:
      summary: Get Chaincodes
      description: Get all chaincodes
      operationId: get-all-chaincodes
      x-api-path-slug: v1chaincodes-get
      parameters:
      - in: header
        name: Authorization
        description: access token
      - in: header
        name: predix-zone-id
        description: tenantId
      responses:
        200:
          description: OK
      tags:
      - Chaincodes
  /v1/chaincodes/{chaincodeName}/query:
    post:
      summary: Post Chaincodes Query
      description: Performs query operation on the chaincode and returns the result
      operationId: performs-query-operation-on-the-chaincode-and-returns-the-result
      x-api-path-slug: v1chaincodeschaincodenamequery-post
      parameters:
      - in: header
        name: Authorization
        description: access token
      - in: path
        name: chaincodeName
        description: chain code name
      - in: body
        name: payload
        description: payload of function and args
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: predix-zone-id
        description: tenantId
      responses:
        200:
          description: OK
      tags:
      - Chaincodes
      - Query
  /v1/users/{userId}/enroll:
    post:
      summary: Post Users Userid Enroll
      description: Enrolls the blockchain user by downloading its certificates and
        storing it in Vault. It also maps the oauth user with the blockchain user.
        This is the very first operation that must be performed.
      operationId: enrolls-the-blockchain-user-by-downloading-its-certificates-and-storing-it-in-vault-it-also-maps-the
      x-api-path-slug: v1usersuseridenroll-post
      parameters:
      - in: header
        name: Authorization
        description: access token
      - in: header
        name: predix-zone-id
        description: tenantId
      - in: body
        name: secret
        description: one time password
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: userId
        description: user id
      responses:
        200:
          description: OK
      tags:
      - Users
      - Userid
      - Enroll
  /v1/users/{userId}:
    put:
      summary: Put User
      description: Registers a new user with blockchain. It sets the attribute 'zone'
        for the user to 'tenantId' as specified in predix-zone-id header
      operationId: registers-a-new-user-with-blockchain-it-sets-the-attribute-zone-for-the-user-to-tenantid-as-specifie
      x-api-path-slug: v1usersuserid-put
      parameters:
      - in: body
        name: attributes
        description: Attributes for this user
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Authorization
        description: access token
      - in: header
        name: predix-zone-id
        description: tenantId
      - in: path
        name: userId
        description: user id
      responses:
        200:
          description: OK
      tags:
      - User
    delete:
      summary: Delete Users
      description: Deletes the user and the user mapping with oauth user. User can
        be deleted only after user has been enrolled.
      operationId: deletes-the-user-and-the-user-mapping-with-oauth-user-user-can-be-deleted-only-after-user-has-been-e
      x-api-path-slug: v1usersuserid-delete
      parameters:
      - in: header
        name: Authorization
        description: access token
      - in: header
        name: predix-zone-id
        description: tenantId
      - in: path
        name: userId
        description: user id
      responses:
        200:
          description: OK
      tags:
      - Users
  /v1/chaincodes/{chaincodeName}/invoke:
    post:
      summary: Post Chaincodes Invoke
      description: Performs the invoke or state change operation on chaincode. It
        invokes the function as specified in the body with given arguments. It returns
        the transaction id to the user.
      operationId: performs-the-invoke-or-state-change-operation-on-chaincode-it-invokes-the-function-as-specified-in-t
      x-api-path-slug: v1chaincodeschaincodenameinvoke-post
      parameters:
      - in: header
        name: Authorization
        description: access token
      - in: path
        name: chaincodeName
        description: chain code name
      - in: body
        name: payload
        description: payload of function and args
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: predix-zone-id
        description: tenantId
      responses:
        200:
          description: OK
      tags:
      - Chaincodes
      - Invoke
  /v1/blocks:
    get:
      summary: Get Blocks
      description: Get current blockchain root info
      operationId: get-current-blockchain-root-info
      x-api-path-slug: v1blocks-get
      parameters:
      - in: header
        name: Authorization
        description: access token
      - in: header
        name: predix-zone-id
        description: tenantId
      responses:
        200:
          description: OK
      tags:
      - Blocks
  /v1/blocks/{blockNumber}:
    get:
      summary: Get Blocks Blocknumber
      description: Get a single blockchain info
      operationId: get-a-single-blockchain-info
      x-api-path-slug: v1blocksblocknumber-get
      parameters:
      - in: header
        name: Authorization
        description: access token
      - in: path
        name: blockNumber
        description: block node number
      - in: header
        name: predix-zone-id
        description: tenantId
      responses:
        200:
          description: OK
      tags:
      - Blocks
      - Blocknumber
  /v1/transactions/{transactionId}:
    get:
      summary: Get Transactions
      description: Get a transaction info
      operationId: get-a-transaction-info
      x-api-path-slug: v1transactionstransactionid-get
      parameters:
      - in: header
        name: Authorization
        description: access token
      - in: header
        name: predix-zone-id
        description: tenantId
      - in: path
        name: transactionId
        description: transaction Id
      responses:
        200:
          description: OK
      tags:
      - Transactions
  /v1/proxy/signature:
    post:
      summary: Post Proxy Signature
      description: Post proxy signature.
      operationId: postV1ProxySignature
      x-api-path-slug: v1proxysignature-post
      parameters:
      - in: header
        name: Authorization
        description: token
      - in: header
        name: Predix-Zone-Id
        description: serviceInstanceId
      - in: body
        name: request
        description: request
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Proxy
      - Signature
  /v1/proxy/signature/details:
    post:
      summary: Post Proxy Signature Details
      description: Post proxy signature details.
      operationId: postV1ProxySignatureDetails
      x-api-path-slug: v1proxysignaturedetails-post
      parameters:
      - in: header
        name: Authorization
        description: token
      - in: header
        name: Predix-Zone-Id
        description: serviceInstanceId
      - in: body
        name: request
        description: request
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Proxy
      - Signature
      - Details
  /v1/proxy/signature/extension:
    post:
      summary: Post Proxy Signature Extension
      description: Post proxy signature extension.
      operationId: postV1ProxySignatureExtension
      x-api-path-slug: v1proxysignatureextension-post
      parameters:
      - in: header
        name: Authorization
        description: token
      - in: header
        name: Predix-Zone-Id
        description: serviceInstanceId
      - in: body
        name: request
        description: request
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Proxy
      - Signature
      - Extension
  /v1/aggregations:
    get:
      summary: Get all available aggregations
      description: |-
        Return all supported aggregations.Response JSON (Status 200){
          "results": [
            {
              "name": "max",
              "type": "Maximum",
              "description": "Returns the maximum value data point for the time range"
            },
            {
              "name": "trendmode",
              "type": "Trend Mode",
              "description": "Returns the maximum and minimum value data point for the time range"
            },
            {
              "name": "count",
              "type": "Count",
              "description": "Returns the number of data points"
            },
            {
              "name": "scale",
              "type": "Scale",
              "description": "Scales each data point by a factor"
            },
            {
              "name": "interpolate",
              "type": "Interpolate",
              "description": "Does linear interpolation for the chosen window"
            },
            {
              "name": "sum",
              "type": "Sum",
              "description": "Adds the data points together"
            },
            {
              "name": "diff",
              "type": "Difference",
              "description": "Returns the difference between successive data points"
            },
            {
              "name": "gaps",
              "type": "Gaps",
              "description": "Marks gaps in data according to sampling rate with a null data point"
            },
            {
              "name": "sampler",
              "type": "Sampler",
              "description": "Returns the sampling rate of change for the data points"
            },
            {
              "name": "div",
              "type": "Divide",
              "description": "Divides each data point by a divisor"
            },
            {
              "name": "min",
              "type": "Minimum",
              "description": "Returns the minimum value data point for the time range"
            },
            {
              "name": "avg",
              "type": "Average",
              "description": "Returns the average of the data point set"
            },
            {
              "name": "least_squares",
              "type": "Least Squares",
              "description": "Returns a best fit line through the data points using the least squares algorithm"
            },
            {
              "name": "percentile",
              "type": "Percentile",
              "description": "Returns the percentile of the data range"
            },
            {
              "name": "dev",
              "type": "Standard Deviation",
              "description": "Returns the standard deviation of the time series"
            },
            {
              "name": "rate",
              "type": "Rate",
              "description": "Returns the rate of change for the data points"
            }
          ]
        }
      operationId: getAggregationNames
      x-api-path-slug: v1aggregations-get
      parameters:
      - in: header
        name: Authorization
      - in: header
        name: Content-Type
      - in: header
        name: Predix-Zone-Id
      responses:
        200:
          description: Successful response
      tags:
      - Available
      - Aggregations
  /v1/datapoints:
    get:
      summary: Query Datapoints
      description: "Both the GET and POST methods can be used to query time series
        data. Use the query API with the GET HTTP method by passing the query JSON
        as a URL query parameter. The advantage of using the GET method is that requests
        and responses can be cached in proxy servers and browsers.  In cases where
        the query JSON is very long and exceeds query parameter length (for some browsers),
        use POST as a convenience method to query the time series API. POST requests
        have no restrictions on data length, however, requests are never cached. The
        Time Series service API is designed this way to support complex, nested time
        series queries on one or more tags and their attributes, with start and end
        times, along with aggregations and filters.Response JSON (Status 200)\n{\n\t\"tags\":
        [{\n\t\t\"name\": \"ALT_SENSOR\",\n\t\t\"results\": [{\n\t\t\t\"filters\":
        {\n\t\t\t\t\"attributes\": {\n\t\t\t\t\t\"host\": [\n\t\t\t\t\t\t\"test\"\n\t\t\t\t\t]\n\t\t\t\t},\n\t\t\t\t\"measurements\":
        {\n\t\t\t\t\t\"condition\": \"le\",\n\t\t\t\t\t\"values\": [\n\t\t\t\t\t\t36\n\t\t\t\t\t]\n\t\t\t\t},\n\t\t\t\t\"qualities\":
        {\n\t\t\t\t\t\"values\": [\n\t\t\t\t\t\t\"3\"\n\t\t\t\t\t]\n\t\t\t\t}\n\t\t\t},\n\t\t\t\"attributes\":
        {\n\t\t\t\t\"host\": [\"test\"]\n\t\t\t},\n\t\t\t\"values\": [\n\t\t\t\t[1449709894000,
        5, 3],\n\t\t\t\t[1449709895000, 7, 3]\n\t\t\t]\n\t\t}],\n\t\t\"stats\": {\n\t\t\t\"rawCount\":
        2\n\t\t}\n\t}]\n}"
      operationId: query
      x-api-path-slug: v1datapoints-get
      parameters:
      - in: header
        name: Authorization
      - in: header
        name: Content-Type
      - in: header
        name: Predix-Zone-Id
      - in: query
        name: query
        description: Valid JSON string
      responses:
        200:
          description: Successful response
      tags:
      - Query
      - Datapoints
    post:
      summary: Query Datapoints
      description: "Both the GET and POST methods can be used to query time series
        data. Use the query API with the GET HTTP method by passing the query JSON
        as a URL query parameter. The advantage of using the GET method is that requests
        and responses can be cached in proxy servers and browsers.  In cases where
        the query JSON is very long and exceeds query parameter length (for some browsers),
        use POST as a convenience method to query the time series API. POST requests
        have no restrictions on data length, however, requests are never cached. The
        Time Series service API is designed this way to support complex, nested time
        series queries on one or more tags and their attributes, with start and end
        times, along with aggregations and filters.  Following is a sample request
        message: Request JSON{\n\t\"start\": \"24h-ago\",\n\t\"end\": \"12h-ago\",\n\t\"tags\":
        [{\n\t\t\"name\": \"ALT_SENSOR\",\n\t\t\"limit\": 1000,\n\t\t\"order\": \"desc\",\n\t\t\"suppressGroupByType\":
        true|false,\n\t\t\"aggregations\": [{\n\t\t\t\"type\": \"avg\",\n\t\t\t\"interval\":
        \"1h\"\n\t\t}],\n\t\t\"filters\": {\n\t\t\t\"attributes\": {\n\t\t\t\t\"host\":
        [\n\t\t\t\t\t\"test\"\n\t\t\t\t]\n\t\t\t},\n\t\t\t\"measurements\": {\n\t\t\t\t\"condition\":
        \"le\",\n\t\t\t\t\"values\": [\n\t\t\t\t\t\"36\"\n\t\t\t\t]\n\t\t\t},\n\t\t\t\"qualities\":
        {\n\t\t\t\t\"values\": [\n\t\t\t\t\t\"3\"\n\t\t\t\t]\n\t\t\t}\n\t\t},\n\t\t\"groups\":
        [{\n\t\t\t\"name\": \"attribute\",\n\t\t\t\"attributes\": [\n\t\t\t\t\"host\",
        \"subtenant\"\n\t\t\t]\n\t\t}]\n\t}]\n}\nResponse JSON (Status 200){\n\t\"tags\":
        [{\n\t\t\"name\": \"ALT_SENSOR\",\n\t\t\"results\": [{\n\t\t\t\"filters\":
        {\n\t\t\t\t\"attributes\": {\n\t\t\t\t\t\"host\": [\n\t\t\t\t\t\t\"test\"\n\t\t\t\t\t]\n\t\t\t\t},\n\t\t\t\t\"measurements\":
        {\n\t\t\t\t\t\"condition\": \"le\",\n\t\t\t\t\t\"values\": [\n\t\t\t\t\t\t36\n\t\t\t\t\t]\n\t\t\t\t},\n\t\t\t\t\"qualities\":
        {\n\t\t\t\t\t\"values\": [\n\t\t\t\t\t\t\"3\"\n\t\t\t\t\t]\n\t\t\t\t}\n\t\t\t},\n\t\t\t\"attributes\":
        {\n\t\t\t\t\"host\": [\"test\"]\n\t\t\t},\n\t\t\t\"values\": [\n\t\t\t\t[1449709894000,
        5, 3],\n\t\t\t\t[1449709895000, 7, 3]\n\t\t\t]\n\t\t}],\n\t\t\"stats\": {\n\t\t\t\"rawCount\":
        2\n\t\t}\n\t}]\n}"
      operationId: get
      x-api-path-slug: v1datapoints-post
      parameters:
      - in: header
        name: Authorization
      - in: header
        name: Content-Type
      - in: header
        name: Predix-Zone-Id
      - in: body
        name: Query Request JSON
        description: Query Request (JSON)
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: Successful response
      tags:
      - Query
      - Datapoints
  /v1/datapoints/latest:
    get:
      summary: Query for Current Value
      description: "This API helps to query time series data for the latest values.Response
        JSON (Status 200){\n\t\"tags\": [{\n\t\t\"name\": \"tagName1\",\n\t\t\"results\":
        [{\n\t\t\t\"values\": [\n\t\t\t\t[1449709895000, 7, 3]\n\t\t\t]\n\t\t}],\n\t\t\"stats\":
        {\n\t\t\t\"rawCount\": 1\n\t\t}\n\t}, {\n\t\t\"name\": \"tagName2\",\n\t\t\"results\":
        [{\n\t\t\t\"values\": [\n\t\t\t\t[1449709896000, 8, 3]\n\t\t\t]\n\t\t}],\n\t\t\"stats\":
        {\n\t\t\t\"rawCount\": 1\n\t\t}\n\t}]\n}"
      operationId: queryCurrent
      x-api-path-slug: v1datapointslatest-get
      parameters:
      - in: header
        name: Authorization
      - in: header
        name: Content-Type
      - in: header
        name: Predix-Zone-Id
      - in: query
        name: suppressGroupByType
        description: Flag to suppress the grouping of results by type
      - in: query
        name: tags
        description: 'List of tags Eg: tag1,tag2'
      responses:
        200:
          description: Successful response
      tags:
      - QueryCurrent
      - Value
    post:
      summary: Query for Current Value
      description: "This API helps to query for timeseries for the latest values for
        the given tags. The POST API also provides a way to specify a time window
        or filter options and retrieves the latest value that satisfies it.Request
        JSON{\n\t\"tags\": [{\n\t\t\"name\": \"ALT_SENSOR\",\n\t\t\"suppressGroupByType\":
        true|false,\n\t\t\"filters\": {\n\t\t\t\"attributes\": {\n\t\t\t\t\"host\":
        [\n\t\t\t\t\t\"test\"\n\t\t\t\t]\n\t\t\t},\n\t\t\t\"measurements\": {\n\t\t\t\t\"condition\":
        \"le\",\n\t\t\t\t\"values\": [\n\t\t\t\t\t\"36\"\n\t\t\t\t]\n\t\t\t},\n\t\t\t\"qualities\":
        {\n\t\t\t\t\"values\": [\n\t\t\t\t\t\"3\"\n\t\t\t\t]\n\t\t\t}\n\t\t}\n\t}]\n}Response
        JSON (Status 200){\n\t\"tags\": [{\n\t\t\"name\": \"ALT_SENSOR\",\n\t\t\"results\":
        [{\n\t\t\t\"filters\": {\n\t\t\t\t\"attributes\": {\n\t\t\t\t\t\"host\": [\n\t\t\t\t\t\t\"test\"\n\t\t\t\t\t]\n\t\t\t\t},\n\t\t\t\t\"measurements\":
        {\n\t\t\t\t\t\"condition\": \"le\",\n\t\t\t\t\t\"values\": [\n\t\t\t\t\t\t36\n\t\t\t\t\t]\n\t\t\t\t},\n\t\t\t\t\"qualities\":
        {\n\t\t\t\t\t\"values\": [\n\t\t\t\t\t\t\"3\"\n\t\t\t\t\t]\n\t\t\t\t}\n\t\t\t},\n\t\t\t\"attributes\":
        {\n\t\t\t\t\"host\": [\"test\"]\n\t\t\t},\n\t\t\t\"values\": [\n\t\t\t\t[1449709895000,
        7, 3]\n\t\t\t]\n\t\t}],\n\t\t\"stats\": {\n\t\t\t\"rawCount\": 1\n\t\t}\n\t}]\n}"
      operationId: queryCurrentPost
      x-api-path-slug: v1datapointslatest-post
      parameters:
      - in: header
        name: Authorization
      - in: header
        name: Content-Type
      - in: header
        name: Predix-Zone-Id
      - in: body
        name: Query Request JSON
        description: Query Request (JSON)
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: Successful response
      tags:
      - QueryCurrent
      - Value
  /v1/tags:
    get:
      summary: Get all tags
      description: "Return all the ingested tag names.Response JSON (Status 200){\n\t\"results\":
        [\n\t\t\"ALT_SENSOR\",\n\t\t\"tagName1\",\n\t\t\"tagName2\"\n\t]\n}"
      operationId: getMetricNames
      x-api-path-slug: v1tags-get
      parameters:
      - in: header
        name: Authorization
      - in: header
        name: Content-Type
      - in: header
        name: Predix-Zone-Id
      responses:
        200:
          description: Successful response
      tags:
      - Tags
  /v1/collections:
    get:
      summary: List all data collections for a customer
      description: |-
        Returns an array containing the names of all data collections for the
        specified customer.
      operationId: returns-an-array-containing-the-names-of-all-data-collections-for-thespecified-customer
      x-api-path-slug: v1collections-get
      parameters:
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - List
      - ""
      - Data
      - Collectionsa
      - Customer
  /v1/collections/{collectionName}:
    get:
      summary: Return all data for a collection
      description: |-
        Returns the full GeoJSON FeatureCollection uploaded for this collection.
        All GeoJSON Features will be as originally uploaded with the addition of
        a featureId attribute that uniquely identifies the feature across all
        your collections.
      operationId: returns-the-full-geojson-featurecollection-uploaded-for-this-collectionall-geojson-features-will-be-
      x-api-path-slug: v1collectionscollectionname-get
      parameters:
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Return
      - ""
      - Dataa
      - Collection
    delete:
      summary: Delete a collection
      description: Delete the collection of data specified by the collection name.
      operationId: delete-the-collection-of-data-specified-by-the-collection-name
      x-api-path-slug: v1collectionscollectionname-delete
      parameters:
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Collection
    post:
      summary: Add a new collection
      description: |-
        Add a new collection of data in the form of a GeoJSON FeatureCollection.
        All coordinates must be in EPSG:4326 (WGS84) (for further details see
        http://epsg.io/4326). Any feature that is not compliant with the GeoJSON
        specification will not be stored. If the specified collection already
        exists, the geospatial data will be appended to the existing data.
      operationId: add-a-new-collection-of-data-in-the-form-of-a-geojson-featurecollectionall-coordinates-must-be-in-ep
      x-api-path-slug: v1collectionscollectionname-post
      parameters:
      - in: body
        name: body
        description: Geospatial data for the collection
        schema:
          $ref: '#/definitions/holder'
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - New
      - Collection
    put:
      summary: Add a new collection
      description: |-
        Add a new collection of data in the form of a GeoJSON FeatureCollection.
        All coordinates must be in EPSG:4326 (WGS84) (for further details see
        http://epsg.io/4326). Any feature that is not compliant with the GeoJSON
        specification will not be stored. Any feature that doesn't contain an id
        will not be stored. If the specified collection already exists, the
        geospatial data will be appended to the existing data. Features with matching
        id's are overwritten.
      operationId: add-a-new-collection-of-data-in-the-form-of-a-geojson-featurecollectionall-coordinates-must-be-in-ep
      x-api-path-slug: v1collectionscollectionname-put
      parameters:
      - in: body
        name: body
        description: Geospatial data for the collection
        schema:
          $ref: '#/definitions/holder'
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - New
      - Collection
  /v1/collections/{collectionName}/spatial-query/bbox-interacts:
    get:
      summary: Return collection features in specified bounding box
      description: |-
        Returns all features in the specified collection that exist fully or
        partially within the specified bounding box. The bounding box is defined
        by two coordinates in the EPSG:4326 (WGS84) (for further details see
        http://epsg.io/4326):

        * left (longitude), bottom (latitude)

        * right (longitude), top (latitude)
      operationId: returns-all-features-in-the-specified-collection-that-exist-fully-orpartially-within-the-specified-b
      x-api-path-slug: v1collectionscollectionnamespatialquerybboxinteracts-get
      parameters:
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Return
      - Collection
      - Features
      - In
      - Specified
      - Bounding
      - Box
  /v1/collections/{collectionName}/cluster:
    get:
      summary: Returns clustering data for collection features in specified bounding
        box
      description: |-
        Returns Clustering data for the specified collection that exist fully
         or partially within the specified bounding box. The bounding box is
         defined by two coordinates in the EPSG:4326 (WGS84)
         (for further details see http://epsg.io/4326):
         * left (longitude), bottom (latitude)
         * right (longitude), top (latitude)
      operationId: returns-clustering-data-for-the-specified-collection-that-exist-fully-or-partially-within-the-specif
      x-api-path-slug: v1collectionscollectionnamecluster-get
      parameters:
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Returns
      - Clustering
      - Datacollection
      - Features
      - In
      - Specified
      - Bounding
      - Box
  /v1/collections/{collectionName}/assets/{assetId}:
    put:
      summary: Add an asset location into a collection.
      description: |-
        Insert a location entry into the named collection for the given asset identifier and timestamp. In addition to
        adding the new asset location, the request also controls the retention of the location history that is
        stored for the given asset in the given collection.

          - If the mandatory property retain_history is set to false then all existing location history for the
          given asset is removed before the new location is added.

          - If the retain_history property is set to true and the optional property purge_history_before is not set
          then the new location is added to the existing set of locations for the given asset.

          - If retain_history is set to true and the optional property purge_history_before is set then any existing
          locations for the given asset that have a timestamp that is older than the supplied purge_history_before
          timestamp are first deleted. Next the new location is added to the set of locations that remain.

          - If the set of location entries for the given asset (after any possible removals) contains a location entry
           with the same timestamp as the new location then the location of that entry is updated rather than a new
           location entry being added.

          - Note the new entry is always added or used to update an existing entry.
      operationId: insert-a-location-entry-into-the-named-collection-for-the-given-asset-identifier-and-timestamp-in-ad
      x-api-path-slug: v1collectionscollectionnameassetsassetid-put
      parameters:
      - in: body
        name: body
        description: An object containing the location of the asset at a given timestamp,
          together with additional properties to controlthe retention of any existing
          asset location history
        schema:
          $ref: '#/definitions/holder'
      - in: query
        name: No Name
      responses:
        200:
          description: Successful response
      tags:
      - Asset
      - Location
      - Into
      - Collection
    delete:
      summary: Delete an asset and its location data
      description: Delete the asset specified by the collection name. Any location
        data associated with the asset are also deleted.
      operationId: delete-the-asset-specified-by-the-collection-name-any-location-data-associated-with-the-asset-are-al
      x-api-path-slug: v1collectionscollectionnameassetsassetid-delete
      parameters:
      - in: query
        name: No Name
      responses:
        200:
          description: Successful response
      tags:
      - Asset
      - Its
      - Location
      - Data
    get:
      summary: Return the latest location data for an asset
      description: |-
        Returns the latest location entry for the given asset. The timestamp and location data for the
        given entry is included in the response.
      operationId: returns-the-latest-location-entry-for-the-given-asset-the-timestamp-and-location-data-for-thegiven-e
      x-api-path-slug: v1collectionscollectionnameassetsassetid-get
      parameters:
      - in: query
        name: No Name
      responses:
        200:
          description: Successful response
      tags:
      - Return
      - Latest
      - Location
      - Dataan
      - Asset
  /v1/collections/{collectionName}/assets/{assetId}/query:
    post:
      summary: Return locations for an asset by query condition for given customer
        id and collection name.
      description: |-
        Returns the locations for an asset by three types of query for a given customer id and collection name.
        The returned locations are in descending order of time.
        Three types of query:
        1. type=latest: The latest n locations will be returned.
        2. type=timeperiod: Locations within a time period will be returned.
        3. type=bbox: Locations within a time period and a spatial bounding box will be returned.
      operationId: returns-the-locations-for-an-asset-by-three-types-of-query-for-a-given-customer-id-and-collection-na
      x-api-path-slug: v1collectionscollectionnameassetsassetidquery-post
      parameters:
      - in: body
        name: body
        description: The parameters for the query for asset locations
        schema:
          $ref: '#/definitions/holder'
      - in: query
        name: No Name
      responses:
        200:
          description: Successful response
      tags:
      - Return
      - Locationsan
      - Asset
      - By
      - Query
      - Conditiongiven
      - Customer
      - Id
      - Collection
      - Name
  /warp:
    post:
      summary: Warp subject and reference arrays
      description: Warp subject and reference arrays.
      operationId: postWarp
      x-api-path-slug: warp-post
      parameters:
      - in: body
        name: body
        description: Subject and Reference arrays to be processed
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: Successful response
      tags:
      - Warp
      - Subject
      - Reference
      - Arrays
  /api/settings:
    get:
      summary: Get EC Gateway settings
      description: Get your EC Gateway settings details
      operationId: get-your-ec-gateway-settings-details
      x-api-path-slug: apisettings-get
      parameters:
      - in: header
        name: Authorization
        description: Bearer *your_token
      - in: header
        name: Predix-Zone-Id
      responses:
        200:
          description: Successful response
      tags:
      - EC
      - Gateway
      - Settings
  /api/token/validate:
    post:
      summary: Validate the oauth2 token
      description: Validate the oauth2 token for the gateway usage
      operationId: validate-the-oauth2-token-for-the-gateway-usage
      x-api-path-slug: apitokenvalidate-post
      parameters:
      - in: header
        name: Authorization
        description: Bearer *your_token
      - in: header
        name: Predix-Zone-Id
      responses:
        200:
          description: Successful response
      tags:
      - Validate
      - Oauth2
      - Token
  /health/check:
    get:
      summary: Validate the EC service status
      description: Validate the EC API status
      operationId: validate-the-ec-api-status
      x-api-path-slug: healthcheck-get
      responses:
        200:
          description: Successful response
      tags:
      - Validate
      - EC
      - Service
      - Status
  /health/memory:
    get:
      summary: Validate the EC service memory usage
      description: Validate the EC gateway memory usage
      operationId: validate-the-ec-gateway-memory-usage
      x-api-path-slug: healthmemory-get
      responses:
        200:
          description: Successful response
      tags:
      - Validate
      - EC
      - Service
      - Memory
      - Usage
  /reports/usage:
    post:
      summary: Report usage
      description: Report usage by zoneid
      operationId: report-usage-by-zoneid
      x-api-path-slug: reportsusage-post
      parameters:
      - in: header
        name: Authorization
        description: Basic *token
      - in: body
        name: content
        description: The content for reporting the usage
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: predix-zone-id
        description: Cloud Foundry service instance id
      responses:
        200:
          description: Successful response
      tags:
      - Report
      - Usage
    get:
      summary: Get last usage
      description: get last usage by zoneid
      operationId: get-last-usage-by-zoneid
      x-api-path-slug: reportsusage-get
      parameters:
      - in: header
        name: Authorization
        description: Basic *token
      - in: header
        name: predix-zone-id
        description: Cloud Foundry service instance id
      responses:
        200:
          description: Successful response
      tags:
      - Last
      - Usage
  /certs:
    post:
      summary: Request a digital certificate
      description: Submit a CSR for a certificate for the EC usage
      operationId: submit-a-csr-for-a-certificate-for-the-ec-usage
      x-api-path-slug: certs-post
      parameters:
      - in: header
        name: Authorization
        description: Basic *token
      - in: body
        name: content
        description: The CSR content in pem format
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: predix-zone-id
        description: Cloud Foundry service instance id
      responses:
        200:
          description: Successful response
      tags:
      - Request
      - Digital
      - Certificate
    get:
      summary: Retrieve current certificate
      description: Retrieve the current certificate issued by the GE Digital CA.
      operationId: retrieve-the-current-certificate-issued-by-the-ge-digital-ca
      x-api-path-slug: certs-get
      parameters:
      - in: header
        name: Authorization
        description: Basic *token
      - in: header
        name: predix-zone-id
        description: Cloud Foundry service instance id
      responses:
        200:
          description: Successful response
      tags:
      - Retrieve
      - Current
      - Certificate
  /admin/accounts/{predix-zone-id}:
    post:
      summary: Create an EC system account
      description: Create a EC system account with the CF details
      operationId: create-a-ec-system-account-with-the-cf-details
      x-api-path-slug: adminaccountspredixzoneid-post
      parameters:
      - in: header
        name: Authorization
        description: Basic *token
      - in: path
        name: predix-zone-id
        description: Cloud Foundry service instance details
      - in: body
        name: settings
        description: Cloud Foundry setting details
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: Successful response
      tags:
      - EC
      - System
      - Account
    get:
      summary: Get the EC system account
      description: Get an existing EC system account by predix zone id
      operationId: get-an-existing-ec-system-account-by-predix-zone-id
      x-api-path-slug: adminaccountspredixzoneid-get
      parameters:
      - in: header
        name: Authorization
        description: Basic *token
      - in: path
        name: predix-zone-id
        description: pass the predix zone id
      responses:
        200:
          description: Successful response
      tags:
      - EC
      - System
      - Account
    delete:
      summary: Delete the EC system account
      description: Delete an existing EC system account by predix zone id
      operationId: delete-an-existing-ec-system-account-by-predix-zone-id
      x-api-path-slug: adminaccountspredixzoneid-delete
      parameters:
      - in: header
        name: Authorization
        description: Basic *token
      - in: path
        name: predix-zone-id
        description: pass the predix zone id
      responses:
        200:
          description: Successful response
      tags:
      - EC
      - System
      - Account
    put:
      summary: Update the EC gateway setting in the account
      description: Update the EC gateway setting in the account with the CF details
      operationId: update-the-ec-gateway-setting-in-the-account-with-the-cf-details
      x-api-path-slug: adminaccountspredixzoneid-put
      parameters:
      - in: header
        name: Authorization
        description: Basic *token
      - in: path
        name: predix-zone-id
        description: Predix Zone Id
      - in: body
        name: settings
        description: Cloud Foundry setting destails
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: Successful response
      tags:
      - EC
      - Gateway
      - Setting
      - In
      - Account
  /v1/plugins/archive/tenants/{tenant_uuid}/archives:
    get:
      summary: Get Plugins Archive Tenants Archives
      description: Get plugins archive tenants archives.
      operationId: getV1PluginsArchiveTenantsTenantUuArchives
      x-api-path-slug: v1pluginsarchivetenantstenant-uuidarchives-get
      parameters:
      - in: path
        name: tenant_uuid
        description: tenant_uuid
      responses:
        200:
          description: Successful response
      tags:
      - Plugins
      - Archive
      - Tenants
      - Archives
  /v1/plugins/archive/tenants/{tenant_uuid}/archives/{uuid}:
    get:
      summary: Get Plugins Archive Tenants Archives
      description: Get plugins archive tenants archives.
      operationId: getV1PluginsArchiveTenantsTenantUuArchivesUu
      x-api-path-slug: v1pluginsarchivetenantstenant-uuidarchivesuuid-get
      parameters:
      - in: path
        name: tenant_uuid
        description: tenant_uuid
      - in: path
        name: uuid
        description: uuid
      responses:
        200:
          description: Successful response
      tags:
      - Plugins
      - Archive
      - Tenants
      - Archives
    delete:
      summary: Delete Plugins Archive Tenants Archives
      description: Delete plugins archive tenants archives.
      operationId: deleteV1PluginsArchiveTenantsTenantUuArchivesUu
      x-api-path-slug: v1pluginsarchivetenantstenant-uuidarchivesuuid-delete
      parameters:
      - in: path
        name: tenant_uuid
        description: tenant_uuid
      - in: path
        name: uuid
        description: uuid
      responses:
        200:
          description: Successful response
      tags:
      - Plugins
      - Archive
      - Tenants
      - Archives
  /v1/plugins/archive/tenants/{tenant_uuid}/configuration:
    get:
      summary: Get Plugins Archive Tenants Configuration
      description: Get plugins archive tenants configuration.
      operationId: getV1PluginsArchiveTenantsTenantUuConfiguration
      x-api-path-slug: v1pluginsarchivetenantstenant-uuidconfiguration-get
      parameters:
      - in: path
        name: tenant_uuid
        description: tenant_uuid
      responses:
        200:
          description: Successful response
      tags:
      - Plugins
      - Archive
      - Tenants
      - Configuration
    post:
      summary: Post Plugins Archive Tenants Configuration
      description: Post plugins archive tenants configuration.
      operationId: postV1PluginsArchiveTenantsTenantUuConfiguration
      x-api-path-slug: v1pluginsarchivetenantstenant-uuidconfiguration-post
      parameters:
      - in: body
        name: archivePluginConfiguration
        description: archivePluginConfiguration
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: tenant_uuid
        description: tenant_uuid
      responses:
        200:
          description: Successful response
      tags:
      - Plugins
      - Archive
      - Tenants
      - Configuration
  /v1/plugins/archive/tenants/{tenant_uuid}/staged-events:
    get:
      summary: Get Plugins Archive Tenants Staged Events
      description: Get plugins archive tenants staged events.
      operationId: getV1PluginsArchiveTenantsTenantUuStagedEvents
      x-api-path-slug: v1pluginsarchivetenantstenant-uuidstagedevents-get
      parameters:
      - in: path
        name: tenant_uuid
        description: tenant_uuid
      responses:
        200:
          description: Successful response
      tags:
      - Plugins
      - Archive
      - Tenants
      - Staged
      - Events
  /v1/tenants/{tenant_uuid}:
    get:
      summary: Get Tenants
      description: Get tenants.
      operationId: getV1TenantsTenantUu
      x-api-path-slug: v1tenantstenant-uuid-get
      parameters:
      - in: path
        name: tenant_uuid
        description: tenant_uuid
      responses:
        200:
          description: OK
      tags:
      - Tenants
    put:
      summary: Put Tenants
      description: Put tenants.
      operationId: putV1TenantsTenantUu
      x-api-path-slug: v1tenantstenant-uuid-put
      parameters:
      - in: body
        name: tenant
        description: tenant
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: tenant_uuid
        description: tenant_uuid
      responses:
        200:
          description: OK
      tags:
      - Tenants
  /v1/tenants/{tenant_uuid}/event-search:
    get:
      summary: Get Tenants Event Search
      description: Get tenants event search.
      operationId: getV1TenantsTenantUuEventSearch
      x-api-path-slug: v1tenantstenant-uuideventsearch-get
      parameters:
      - in: query
        name: query
        description: query
      - in: path
        name: tenant_uuid
        description: tenant_uuid
      responses:
        200:
          description: Successful response
      tags:
      - Tenants
      - Event
      - Search
  /v1/tenants/{tenant_uuid}/events:
    get:
      summary: Get Tenants Events
      description: Get tenants events.
      operationId: getV1TenantsTenantUuEvents
      x-api-path-slug: v1tenantstenant-uuidevents-get
      parameters:
      - in: query
        name: end_date
        description: end_date
      - in: query
        name: start_date
        description: start_date
      - in: query
        name: tag
        description: tag
      - in: path
        name: tenant_uuid
        description: tenant_uuid
      responses:
        200:
          description: OK
      tags:
      - Tenants
      - Events
    post:
      summary: Post Tenants Events
      description: Post tenants events.
      operationId: postV1TenantsTenantUuEvents
      x-api-path-slug: v1tenantstenant-uuidevents-post
      parameters:
      - in: body
        name: events
        description: events
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: tenant_uuid
        description: tenant_uuid
      responses:
        200:
          description: Successful response
      tags:
      - Tenants
      - Events
  /v1/tenants/{tenant_uuid}/events/{uuid}:
    get:
      summary: Get Tenants Events
      description: Get tenants events.
      operationId: getV1TenantsTenantUuEventsUu
      x-api-path-slug: v1tenantstenant-uuideventsuuid-get
      parameters:
      - in: path
        name: tenant_uuid
        description: tenant_uuid
      - in: path
        name: uuid
        description: uuid
      responses:
        200:
          description: Successful response
      tags:
      - Tenants
      - Events
    put:
      summary: Put Tenants Events
      description: Put tenants events.
      operationId: putV1TenantsTenantUuEventsUu
      x-api-path-slug: v1tenantstenant-uuideventsuuid-put
      parameters:
      - in: body
        name: event
        description: event
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: tenant_uuid
        description: tenant_uuid
      - in: path
        name: uuid
        description: uuid
      responses:
        200:
          description: Successful response
      tags:
      - Tenants
      - Events
    delete:
      summary: Delete Tenants Events
      description: Delete tenants events.
      operationId: deleteV1TenantsTenantUuEventsUu
      x-api-path-slug: v1tenantstenant-uuideventsuuid-delete
      parameters:
      - in: path
        name: tenant_uuid
        description: tenant_uuid
      - in: path
        name: uuid
        description: uuid
      responses:
        200:
          description: Successful response
      tags:
      - Tenants
      - Events
  /v2/catalog:
    get:
      summary: Get Catalog
      description: Get catalog.
      operationId: getV2Catalog
      x-api-path-slug: v2catalog-get
      responses:
        200:
          description: Successful response
      tags:
      - Catalog
  /v2/service_instances/{instanceId}:
    put:
      summary: Put Service Instances
      description: Put service instances.
      operationId: putV2ServiceInstancesInstance
      x-api-path-slug: v2service-instancesinstanceid-put
      parameters:
      - in: query
        name: accepts_incomplete
        description: accepts_incomplete
      - in: path
        name: instanceId
        description: instanceId
      - in: body
        name: request
        description: request
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: Successful response
      tags:
      - Service
      - Instances
    delete:
      summary: Delete Service Instances
      description: Delete service instances.
      operationId: deleteV2ServiceInstancesInstance
      x-api-path-slug: v2service-instancesinstanceid-delete
      parameters:
      - in: query
        name: accepts_incomplete
        description: accepts_incomplete
      - in: path
        name: instanceId
        description: instanceId
      - in: query
        name: plan_id
        description: plan_id
      - in: query
        name: service_id
        description: service_id
      responses:
        200:
          description: Successful response
      tags:
      - Service
      - Instances
    patch:
      summary: Patch Service Instances
      description: Patch service instances.
      operationId: patchV2ServiceInstancesInstance
      x-api-path-slug: v2service-instancesinstanceid-patch
      parameters:
      - in: query
        name: accepts_incomplete
        description: accepts_incomplete
      - in: path
        name: instanceId
        description: instanceId
      - in: body
        name: request
        description: request
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: Successful response
      tags:
      - Service
      - Instances
  /v2/service_instances/{instanceId}/last_operation:
    get:
      summary: Get Service Instances Last Operation
      description: Get service instances last operation.
      operationId: getV2ServiceInstancesInstanceLastOperation
      x-api-path-slug: v2service-instancesinstanceidlast-operation-get
      parameters:
      - in: path
        name: instanceId
        description: instanceId
      responses:
        200:
          description: Successful response
      tags:
      - Service
      - Instances
      - Last
      - Operation
  /v2/service_instances/{instanceId}/service_bindings/{bindingId}:
    put:
      summary: Put Service Instances Service Bindings Bindingid
      description: Put service instances service bindings bindingid.
      operationId: putV2ServiceInstancesInstanceServiceBindingsBinding
      x-api-path-slug: v2service-instancesinstanceidservice-bindingsbindingid-put
      parameters:
      - in: path
        name: bindingId
        description: bindingId
      - in: path
        name: instanceId
        description: instanceId
      - in: body
        name: request
        description: request
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: Successful response
      tags:
      - Service
      - Instances
      - Service
      - Bindings
      - Bindingid
    delete:
      summary: Delete Service Instances Service Bindings Bindingid
      description: Delete service instances service bindings bindingid.
      operationId: deleteV2ServiceInstancesInstanceServiceBindingsBinding
      x-api-path-slug: v2service-instancesinstanceidservice-bindingsbindingid-delete
      parameters:
      - in: path
        name: bindingId
        description: bindingId
      - in: path
        name: instanceId
        description: instanceId
      - in: query
        name: plan_id
        description: plan_id
      - in: query
        name: service_id
        description: service_id
      responses:
        200:
          description: Successful response
      tags:
      - Service
      - Instances
      - Service
      - Bindings
      - Bindingid
  /v1/group/createGroup:
    post:
      summary: Create Group
      description: Create group.
      operationId: createGroup
      x-api-path-slug: v1groupcreategroup-post
      parameters:
      - in: header
        name: 'Authorization: Bearer'
        description: OAuth2 token
      - in: body
        name: body
        description: Request body
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Predix-Zone-Id
        description: Zone ID
      responses:
        200:
          description: OK
      tags:
      - Group
  /v1/group/deleteGroup:
    post:
      summary: Delete Group
      description: Delete group.
      operationId: deleteGroup
      x-api-path-slug: v1groupdeletegroup-post
      parameters:
      - in: header
        name: 'Authorization: Bearer'
        description: OAuth2 token
      - in: body
        name: body
        description: Request body
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Predix-Zone-Id
        description: Zone ID
      responses:
        200:
          description: OK
      tags:
      - Group
  /v1/object/preregisterObject:
    post:
      summary: Object Pre-Register
      description: Pre-register object with image.<br> Individual ID must be designated
        by user.
      operationId: userIssue
      x-api-path-slug: v1objectpreregisterobject-post
      parameters:
      - in: formData
        name: applyFlag
        description: '* DO NOT USE'
      - in: header
        name: 'Authorization: Bearer'
        description: OAuth2 token
      - in: formData
        name: individualId
        description: Individual ID
      - in: header
        name: Predix-Zone-Id
        description: Zone ID
      - in: formData
        name: registImage
        description: 'Image data(Max file size: 5MByte)'
      responses:
        200:
          description: OK
      tags:
      - Object
      - Pre-Register
  /v1/object/preregisterObjectWithoutID:
    post:
      summary: Object Pre-Register without ID
      description: Pre-register object with image.<br> Individual ID will be issued
        from system.
      operationId: systemIssue
      x-api-path-slug: v1objectpreregisterobjectwithoutid-post
      parameters:
      - in: formData
        name: applyFlag
        description: '* DO NOT USE'
      - in: header
        name: 'Authorization: Bearer'
        description: OAuth2 token
      - in: header
        name: Predix-Zone-Id
        description: Zone ID
      - in: formData
        name: registImage
        description: 'Image data(Max file size: 5MByte)'
      responses:
        200:
          description: OK
      tags:
      - Object
      - Pre-Register
      - Without
      - ID
  /v1/object/deleteRegisteredObject:
    post:
      summary: Delete Registered Object
      description: Delete registered object.
      operationId: deleteRegularRegistration
      x-api-path-slug: v1objectdeleteregisteredobject-post
      parameters:
      - in: header
        name: 'Authorization: Bearer'
        description: OAuth2 token
      - in: body
        name: body
        description: Request body
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Predix-Zone-Id
        description: Zone ID
      responses:
        200:
          description: OK
      tags:
      - Registered
      - Object
  /v1/object/deletePreregisteredObject:
    post:
      summary: Delete Pre-Registered Object
      description: Delete pre-registered object.
      operationId: deleteTempRegistration
      x-api-path-slug: v1objectdeletepreregisteredobject-post
      parameters:
      - in: header
        name: 'Authorization: Bearer'
        description: OAuth2 token
      - in: body
        name: body
        description: Request body
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Predix-Zone-Id
        description: Zone ID
      responses:
        200:
          description: OK
      tags:
      - Pre-Registered
      - Object
  /v1/object/setObjectDoNotRegisterFlag:
    post:
      summary: Switch Apply Flag
      description: '* DO NOT USE. This API will be deleted.<br>Switch the Apply flag
        on or off.'
      operationId: config
      x-api-path-slug: v1objectsetobjectdonotregisterflag-post
      parameters:
      - in: header
        name: 'Authorization: Bearer'
        description: OAuth2 token
      - in: body
        name: body
        description: Request body
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Predix-Zone-Id
        description: Zone ID
      responses:
        200:
          description: OK
      tags:
      - Switch
      - Apply
      - Flag
  /v1/object/setGroupDoNotRegisterFlag:
    post:
      summary: Switch Apply Flag per Group
      description: '* DO NOT USE. This API will be deleted.<br>Switch the Apply flag
        per group'
      operationId: groupConfig
      x-api-path-slug: v1objectsetgroupdonotregisterflag-post
      parameters:
      - in: header
        name: 'Authorization: Bearer'
        description: OAuth2 token
      - in: body
        name: body
        description: Request body
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Predix-Zone-Id
        description: Zone ID
      responses:
        200:
          description: OK
      tags:
      - Switch
      - Apply
      - Flag
      - Per
      - Group
  /v1/group/putInGroup:
    post:
      summary: Put Object in Group
      description: Put Object in Group.
      operationId: joinGroup
      x-api-path-slug: v1groupputingroup-post
      parameters:
      - in: header
        name: 'Authorization: Bearer'
        description: OAuth2 token
      - in: body
        name: body
        description: Request body
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Predix-Zone-Id
        description: Zone ID
      responses:
        200:
          description: OK
      tags:
      - Object
      - In
      - Group
  /v1/group/removeFromGroup:
    post:
      summary: Remove Object from Group
      description: Remove Object from Group.
      operationId: leaveGroup
      x-api-path-slug: v1groupremovefromgroup-post
      parameters:
      - in: header
        name: 'Authorization: Bearer'
        description: OAuth2 token
      - in: body
        name: body
        description: Request body
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Predix-Zone-Id
        description: Zone ID
      responses:
        200:
          description: OK
      tags:
      - Remove
      - Object
      - From
      - Group
  /v1/object/registerObject:
    post:
      summary: Register Object
      description: Register Object. A registered object can be queried from Query
        APIs.
      operationId: apply
      x-api-path-slug: v1objectregisterobject-post
      parameters:
      - in: header
        name: 'Authorization: Bearer'
        description: OAuth2 token
      - in: body
        name: body
        description: Request body
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Predix-Zone-Id
        description: Zone ID
      responses:
        200:
          description: OK
      tags:
      - Register
      - Object
  /v1/object/registerGroup:
    post:
      summary: Register Object per Group
      description: Register Object per Group. A registered object can be queried from
        Query APIs.
      operationId: groupApply
      x-api-path-slug: v1objectregistergroup-post
      parameters:
      - in: header
        name: 'Authorization: Bearer'
        description: OAuth2 token
      - in: body
        name: body
        description: Request body
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Predix-Zone-Id
        description: Zone ID
      responses:
        200:
          description: OK
      tags:
      - Register
      - Object
      - Per
      - Group
  /v1/object/listObjects:
    post:
      summary: List Registered Objects
      description: List registered Objects.
      operationId: reference
      x-api-path-slug: v1objectlistobjects-post
      parameters:
      - in: header
        name: 'Authorization: Bearer'
        description: OAuth2 token
      - in: body
        name: body
        description: Request body
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Predix-Zone-Id
        description: Zone ID
      responses:
        200:
          description: OK
      tags:
      - List
      - Registered
      - Objects
  /v1/group/listGroups:
    post:
      summary: List Groups
      description: List groups
      operationId: groupReference
      x-api-path-slug: v1grouplistgroups-post
      parameters:
      - in: header
        name: 'Authorization: Bearer'
        description: OAuth2 token
      - in: body
        name: body
        description: Request body
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Predix-Zone-Id
        description: Zone ID
      responses:
        200:
          description: OK
      tags:
      - List
      - Groups
  /v1/object/checkPreregisteredObject:
    post:
      summary: Check Pre-Registered Object
      description: Check a score of Pre-Registered Object.
      operationId: check
      x-api-path-slug: v1objectcheckpreregisteredobject-post
      parameters:
      - in: header
        name: 'Authorization: Bearer'
        description: OAuth2 token
      - in: formData
        name: individualId
        description: Individual ID
      - in: header
        name: Predix-Zone-Id
        description: Zone ID
      - in: formData
        name: registImage
        description: 'Image data(Max file size: 5MByte)'
      responses:
        200:
          description: OK
      tags:
      - Check
      - Pre-Registered
      - Object
  /v1/query/queryByObject:
    post:
      summary: Query by Object
      description: Query image by object.
      operationId: dozicheck
      x-api-path-slug: v1queryquerybyobject-post
      parameters:
      - in: header
        name: 'Authorization: Bearer'
        description: OAuth2 token
      - in: formData
        name: checkResultDisplayNumber
        description: 'Result display number: Specify number of verification result
          to retrieve'
      - in: formData
        name: idSpecificationFlag
        description: 'ID specification flag (0: Query with all registered objects
          , 1: Query with specified object by individual ID)'
      - in: formData
        name: individualId
        description: 'Individual ID: Use CSV form when specifying multiple IDs'
      - in: header
        name: Predix-Zone-Id
        description: Zone ID
      - in: formData
        name: queryImage
        description: 'Query image data(Max file size: 5MByte)'
      responses:
        200:
          description: OK
      tags:
      - Query
      - By
      - Object
  /v1/query/queryByGroup:
    post:
      summary: Query by Group
      description: Query image per group.
      operationId: groupzicheck
      x-api-path-slug: v1queryquerybygroup-post
      parameters:
      - in: header
        name: 'Authorization: Bearer'
        description: OAuth2 token
      - in: formData
        name: checkResultDisplayNumber
        description: 'Result display number: Specify number of verification result
          to retrieve'
      - in: formData
        name: groupId
        description: 'Group ID: Use CSV form when specifying multiple IDs'
      - in: formData
        name: idSpecificationFlag
        description: 'ID specification flag(0: Query with all registered objects ,
          1: Query with specified object by groupId)'
      - in: header
        name: Predix-Zone-Id
        description: Zone ID
      - in: formData
        name: queryImage
        description: 'Query image data(Max file size: 5MByte)'
      responses:
        200:
          description: OK
      tags:
      - Query
      - By
      - Group
  /dags:
    get:
      summary: Get Dags
      description: Get dags.
      operationId: getDAGsUsingGET
      x-api-path-slug: dags-get
      parameters:
      - in: query
        name: maxUpdateTime
        description: maxUpdateTime
      - in: query
        name: minUpdateTime
        description: minUpdateTime
      - in: query
        name: name
        description: name
      - in: query
        name: page
        description: Results page you want to retrieve (0
      - in: query
        name: size
        description: Number of records per page
      - in: query
        name: sort
        description: 'Sorting criteria in the format: property(,asc|desc)'
      - in: query
        name: tag
        description: tag
      - in: query
        name: type
        description: type
      responses:
        200:
          description: Successful response
      tags:
      - Dags
    post:
      summary: Post Dags
      description: Post dags.
      operationId: saveDAGUsingPOST
      x-api-path-slug: dags-post
      parameters:
      - in: body
        name: dag
        description: dag
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: Successful response
      tags:
      - Dags
  /dags/pause/{dagName}:
    put:
      summary: Put Dags Pause
      description: Put dags pause.
      operationId: pauseDAGUsingPUT
      x-api-path-slug: dagspausedagname-put
      parameters:
      - in: path
        name: dagName
        description: dagName
      responses:
        200:
          description: Successful response
      tags:
      - Dags
      - Pause
  /dags/status/{dagName}:
    get:
      summary: Get Dags Status
      description: Get dags status.
      operationId: getDAGStatusUsingGET
      x-api-path-slug: dagsstatusdagname-get
      parameters:
      - in: path
        name: dagName
        description: dagName
      responses:
        200:
          description: Successful response
      tags:
      - Dags
      - Status
  /dags/status/{dagName}/runs:
    get:
      summary: Get Dags Status Runs
      description: Get dags status runs.
      operationId: getDagRunsUsingGET
      x-api-path-slug: dagsstatusdagnameruns-get
      parameters:
      - in: path
        name: dagName
        description: dagName
      - in: query
        name: end_time
        description: end_time  or latest for latest dag run
      - in: query
        name: start_time
        description: start_time
      responses:
        200:
          description: Successful response
      tags:
      - Dags
      - Status
      - Runs
  /dags/status/{dagName}/runs/{runId}:
    get:
      summary: Get Dags Status Runs Runid
      description: Get dags status runs runid.
      operationId: getUniqueDagRunUsingGET
      x-api-path-slug: dagsstatusdagnamerunsrunid-get
      parameters:
      - in: path
        name: dagName
        description: dagName
      - in: path
        name: runId
        description: runId
      responses:
        200:
          description: Successful response
      tags:
      - Dags
      - Status
      - Runs
      - Runid
  /dags/status/{dagName}/tasks:
    get:
      summary: Get Dags Status Tasks
      description: Get dags status tasks.
      operationId: getAllDagTasksUsingGET
      x-api-path-slug: dagsstatusdagnametasks-get
      parameters:
      - in: path
        name: dagName
        description: dagName
      - in: query
        name: end_time
        description: end_time
      - in: query
        name: start_time
        description: start_time
      responses:
        200:
          description: Successful response
      tags:
      - Dags
      - Status
      - Tasks
  /dags/status/{dagName}/tasks/runs/{runId}:
    get:
      summary: Get Dags Status Tasks Runs Runid
      description: Get dags status tasks runs runid.
      operationId: getTaskStatusByRunIdUsingGET
      x-api-path-slug: dagsstatusdagnametasksrunsrunid-get
      parameters:
      - in: path
        name: dagName
        description: dagName
      - in: path
        name: runId
        description: runId
      responses:
        200:
          description: Successful response
      tags:
      - Dags
      - Status
      - Tasks
      - Runs
      - Runid
  /dags/status/{dagName}/tasks/{taskId}:
    get:
      summary: Get Dags Status Tasks Taskid
      description: Get dags status tasks taskid.
      operationId: getTaskStatusUsingGET
      x-api-path-slug: dagsstatusdagnametaskstaskid-get
      parameters:
      - in: path
        name: dagName
        description: dagName
      - in: path
        name: taskId
        description: taskId
      responses:
        200:
          description: Successful response
      tags:
      - Dags
      - Status
      - Tasks
      - Taskid
  /dags/status/{dagName}/tasks/{taskId}/runs/{runId}:
    get:
      summary: Get Dags Status Tasks Taskid Runs Runid
      description: Get dags status tasks taskid runs runid.
      operationId: getUniqueRunTaskStatusUsingGET
      x-api-path-slug: dagsstatusdagnametaskstaskidrunsrunid-get
      parameters:
      - in: path
        name: dagName
        description: dagName
      - in: path
        name: runId
        description: runId
      - in: path
        name: taskId
        description: taskId
      responses:
        200:
          description: Successful response
      tags:
      - Dags
      - Status
      - Tasks
      - Taskid
      - Runs
      - Runid
  /dags/statusall:
    get:
      summary: Get Dags Statusall
      description: Get dags statusall.
      operationId: getDagsByTenantUsingGET
      x-api-path-slug: dagsstatusall-get
      responses:
        200:
          description: Successful response
      tags:
      - Dags
      - Statusall
  /dags/tags:
    get:
      summary: Get Dags Tags
      description: Get dags tags.
      operationId: getAllDagTagsUsingGET
      x-api-path-slug: dagstags-get
      responses:
        200:
          description: Successful response
      tags:
      - Dags
      - Tags
  /dags/trigger/{dagName}/{dagId}:
    post:
      summary: Post Dags Trigger
      description: Post dags trigger.
      operationId: triggerDAGUsingPOST
      x-api-path-slug: dagstriggerdagnamedagid-post
      parameters:
      - in: query
        name: dagId
        description: dagId
      - in: query
        name: dagName
        description: Dag Reference Id
      - in: body
        name: jsonBody
        description: jsonBody
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: Successful response
      tags:
      - Dags
      - Trigger
  /dags/{dagName}:
    get:
      summary: Get Dags
      description: Get dags.
      operationId: getDAGUsingGET
      x-api-path-slug: dagsdagname-get
      parameters:
      - in: path
        name: dagName
        description: dagName
      responses:
        200:
          description: Successful response
      tags:
      - Dags
    post:
      summary: Post Dags
      description: Post dags.
      operationId: updateDAGUsingPOST_1
      x-api-path-slug: dagsdagname-post
      parameters:
      - in: path
        name: dagName
        description: dagName
      responses:
        200:
          description: Successful response
      tags:
      - Dags
    delete:
      summary: Delete Dags
      description: Delete dags.
      operationId: deleteDAGUsingDELETE
      x-api-path-slug: dagsdagname-delete
      parameters:
      - in: path
        name: dagName
        description: dagName
      responses:
        200:
          description: Successful response
      tags:
      - Dags
  /dags/{dagName}/deploy:
    post:
      summary: Post Dags Deploy
      description: Post dags deploy.
      operationId: deployDAGUsingPOST
      x-api-path-slug: dagsdagnamedeploy-post
      parameters:
      - in: path
        name: dagName
        description: dagName
      responses:
        200:
          description: Successful response
      tags:
      - Dags
      - Deploy
  /dependencies:
    get:
      summary: Get Dependencies
      description: Get dependencies.
      operationId: getDependencyListUsingGET
      x-api-path-slug: dependencies-get
      parameters:
      - in: query
        name: page
        description: Results page you want to retrieve (0
      - in: query
        name: size
        description: Number of records per page
      - in: query
        name: sort
        description: 'Sorting criteria in the format: property(,asc|desc)'
      responses:
        200:
          description: Successful response
      tags:
      - Dependencies
    post:
      summary: Post Dependencies
      description: Post dependencies.
      operationId: createDependencyUsingPOST
      x-api-path-slug: dependencies-post
      responses:
        200:
          description: Successful response
      tags:
      - Dependencies
  /dependencies/deploy:
    post:
      summary: Post Dependencies Deploy
      description: Post dependencies deploy.
      operationId: deployDependencyUsingPOST_1
      x-api-path-slug: dependenciesdeploy-post
      parameters:
      - in: query
        name: id
        description: id
      responses:
        200:
          description: Successful response
      tags:
      - Dependencies
      - Deploy
  /dependencies/deploy/{dependencyId}:
    post:
      summary: Post Dependencies Deploy Dependencyid
      description: Post dependencies deploy dependencyid.
      operationId: deployDependencyUsingPOST
      x-api-path-slug: dependenciesdeploydependencyid-post
      parameters:
      - in: path
        name: dependencyId
        description: dependencyId
      responses:
        200:
          description: Successful response
      tags:
      - Dependencies
      - Deploy
      - Dependencyid
  /dependencies/tags:
    get:
      summary: Get Dependencies Tags
      description: Get dependencies tags.
      operationId: getAllDependencyTagsUsingGET
      x-api-path-slug: dependenciestags-get
      responses:
        200:
          description: Successful response
      tags:
      - Dependencies
      - Tags
  /dependencies/undeploy:
    post:
      summary: Post Dependencies Undeploy
      description: Post dependencies undeploy.
      operationId: undeployDependencyUsingPOST_1
      x-api-path-slug: dependenciesundeploy-post
      parameters:
      - in: query
        name: id
        description: id
      responses:
        200:
          description: Successful response
      tags:
      - Dependencies
      - Undeploy
  /dependencies/undeploy/{dependencyId}:
    post:
      summary: Post Dependencies Undeploy Dependencyid
      description: Post dependencies undeploy dependencyid.
      operationId: undeployDependencyUsingPOST
      x-api-path-slug: dependenciesundeploydependencyid-post
      parameters:
      - in: path
        name: dependencyId
        description: dependencyId
      responses:
        200:
          description: Successful response
      tags:
      - Dependencies
      - Undeploy
      - Dependencyid
  /dependencies/{dependencyId}:
    get:
      summary: Get Dependencies Dependencyid
      description: Get dependencies dependencyid.
      operationId: getDependencyUsingGET
      x-api-path-slug: dependenciesdependencyid-get
      parameters:
      - in: path
        name: dependencyId
        description: dependencyId
      responses:
        200:
          description: Successful response
      tags:
      - Dependencies
      - Dependencyid
    post:
      summary: Post Dependencies Dependencyid
      description: Post dependencies dependencyid.
      operationId: updateDependencyUsingPOST
      x-api-path-slug: dependenciesdependencyid-post
      parameters:
      - in: path
        name: dependencyId
        description: dependencyId
      responses:
        200:
          description: Successful response
      tags:
      - Dependencies
      - Dependencyid
    delete:
      summary: Delete Dependencies Dependencyid
      description: Delete dependencies dependencyid.
      operationId: deleteDependencyUsingDELETE
      x-api-path-slug: dependenciesdependencyid-delete
      parameters:
      - in: path
        name: dependencyId
        description: dependencyId
      responses:
        200:
          description: Successful response
      tags:
      - Dependencies
      - Dependencyid
  /flow-templates:
    get:
      summary: Get Flow Templates
      description: Get flow templates.
      operationId: getFlowTemplatesUsingGET
      x-api-path-slug: flowtemplates-get
      parameters:
      - in: query
        name: displayShellTemplates
        description: displayShellTemplates
      - in: query
        name: maxUpdateTime
        description: maxUpdateTime
      - in: query
        name: minUpdateTime
        description: minUpdateTime
      - in: query
        name: name
        description: name
      - in: query
        name: page
        description: Results page you want to retrieve (0
      - in: query
        name: size
        description: Number of records per page
      - in: query
        name: sort
        description: 'Sorting criteria in the format: property(,asc|desc)'
      - in: query
        name: tag
        description: tag
      - in: query
        name: type
        description: type
      responses:
        200:
          description: Successful response
      tags:
      - Flow
      - Templates
    post:
      summary: Post Flow Templates
      description: Post flow templates.
      operationId: saveFlowTemplateUsingPOST
      x-api-path-slug: flowtemplates-post
      responses:
        200:
          description: Successful response
      tags:
      - Flow
      - Templates
  /flow-templates/tags:
    get:
      summary: Get Flow Templates Tags
      description: Get flow templates tags.
      operationId: getAllFlowTemplateTagsUsingGET
      x-api-path-slug: flowtemplatestags-get
      responses:
        200:
          description: Successful response
      tags:
      - Flow
      - Templates
      - Tags
  /flow-templates/{flowTemplateId}:
    get:
      summary: Get Flow Templates Flowtemplateid
      description: Get flow templates flowtemplateid.
      operationId: getFlowTemplateUsingGET
      x-api-path-slug: flowtemplatesflowtemplateid-get
      parameters:
      - in: path
        name: flowTemplateId
        description: flowTemplateId
      responses:
        200:
          description: Successful response
      tags:
      - Flow
      - Templates
      - Flowtemplateid
    post:
      summary: Post Flow Templates Flowtemplateid
      description: Post flow templates flowtemplateid.
      operationId: updateFlowTemplateUsingPOST
      x-api-path-slug: flowtemplatesflowtemplateid-post
      parameters:
      - in: path
        name: flowTemplateId
        description: flowTemplateId
      responses:
        200:
          description: Successful response
      tags:
      - Flow
      - Templates
      - Flowtemplateid
    put:
      summary: Put Flow Templates Flowtemplateid
      description: Put flow templates flowtemplateid.
      operationId: updateFlowTemplateUsingPUT
      x-api-path-slug: flowtemplatesflowtemplateid-put
      parameters:
      - in: body
        name: flowTemplate
        description: flowTemplate
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: flowTemplateId
        description: flowTemplateId
      responses:
        200:
          description: Successful response
      tags:
      - Flow
      - Templates
      - Flowtemplateid
    delete:
      summary: Delete Flow Templates Flowtemplateid
      description: Delete flow templates flowtemplateid.
      operationId: deleteFlowTemplateUsingDELETE
      x-api-path-slug: flowtemplatesflowtemplateid-delete
      parameters:
      - in: path
        name: flowTemplateId
        description: flowTemplateId
      responses:
        200:
          description: Successful response
      tags:
      - Flow
      - Templates
      - Flowtemplateid
  /flow-templates/{flowTemplateId}/download:
    get:
      summary: Get Flow Templates Flowtemplateid Download
      description: Get flow templates flowtemplateid download.
      operationId: getFlowTemplateFileUsingGET
      x-api-path-slug: flowtemplatesflowtemplateiddownload-get
      parameters:
      - in: path
        name: flowTemplateId
        description: flowTemplateId
      responses:
        200:
          description: Successful response
      tags:
      - Flow
      - Templates
      - Flowtemplateid
      - Download
  /flow-templates/{flowTemplateId}/flows:
    get:
      summary: Get Flow Templates Flowtemplateid Flows
      description: Get flow templates flowtemplateid flows.
      operationId: getFlowsUsingGET_1
      x-api-path-slug: flowtemplatesflowtemplateidflows-get
      parameters:
      - in: path
        name: flowTemplateId
        description: flowTemplateId
      - in: query
        name: maxUpdateTime
        description: maxUpdateTime
      - in: query
        name: minUpdateTime
        description: minUpdateTime
      - in: query
        name: name
        description: name
      - in: query
        name: page
        description: Results page you want to retrieve (0
      - in: query
        name: size
        description: Number of records per page
      - in: query
        name: sort
        description: 'Sorting criteria in the format: property(,asc|desc)'
      - in: query
        name: tag
        description: tag
      - in: query
        name: type
        description: type
      responses:
        200:
          description: Successful response
      tags:
      - Flow
      - Templates
      - Flowtemplateid
      - Flows
    post:
      summary: Post Flow Templates Flowtemplateid Flows
      description: Post flow templates flowtemplateid flows.
      operationId: saveFlowUsingPOST_1
      x-api-path-slug: flowtemplatesflowtemplateidflows-post
      parameters:
      - in: path
        name: flowTemplateId
        description: flowTemplateId
      - in: query
        name: launch
        description: launch
      responses:
        200:
          description: Successful response
      tags:
      - Flow
      - Templates
      - Flowtemplateid
      - Flows
  /flow-templates/{flowTemplateId}/flows/{flowId}:
    get:
      summary: Get Flow Templates Flowtemplateid Flows Flowid
      description: Get flow templates flowtemplateid flows flowid.
      operationId: getFlowUsingGET_1
      x-api-path-slug: flowtemplatesflowtemplateidflowsflowid-get
      parameters:
      - in: path
        name: flowId
        description: flowId
      - in: path
        name: flowTemplateId
        description: flowTemplateId
      responses:
        200:
          description: Successful response
      tags:
      - Flow
      - Templates
      - Flowtemplateid
      - Flows
      - Flowid
    post:
      summary: Post Flow Templates Flowtemplateid Flows Flowid
      description: Post flow templates flowtemplateid flows flowid.
      operationId: updateFlowUsingPOST_1
      x-api-path-slug: flowtemplatesflowtemplateidflowsflowid-post
      parameters:
      - in: body
        name: flow
        description: flow
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: flowId
        description: flowId
      responses:
        200:
          description: Successful response
      tags:
      - Flow
      - Templates
      - Flowtemplateid
      - Flows
      - Flowid
    delete:
      summary: Delete Flow Templates Flowtemplateid Flows Flowid
      description: Delete flow templates flowtemplateid flows flowid.
      operationId: deleteFlowUsingDELETE_1
      x-api-path-slug: flowtemplatesflowtemplateidflowsflowid-delete
      parameters:
      - in: path
        name: flowId
        description: flowId
      responses:
        200:
          description: Successful response
      tags:
      - Flow
      - Templates
      - Flowtemplateid
      - Flows
      - Flowid
  /flow-templates/{flowTemplateId}/flows/{flowId}/config:
    get:
      summary: Get Flow Templates Flowtemplateid Flows Flowid Config
      description: Get flow templates flowtemplateid flows flowid config.
      operationId: listFlowConfigFilesUsingGET_1
      x-api-path-slug: flowtemplatesflowtemplateidflowsflowidconfig-get
      parameters:
      - in: path
        name: flowId
        description: flowId
      responses:
        200:
          description: Successful response
      tags:
      - Flow
      - Templates
      - Flowtemplateid
      - Flows
      - Flowid
      - Config
    post:
      summary: Post Flow Templates Flowtemplateid Flows Flowid Config
      description: Post flow templates flowtemplateid flows flowid config.
      operationId: addFlowConfigFileUsingPOST_1
      x-api-path-slug: flowtemplatesflowtemplateidflowsflowidconfig-post
      parameters:
      - in: path
        name: flowId
        description: flowId
      responses:
        200:
          description: Successful response
      tags:
      - Flow
      - Templates
      - Flowtemplateid
      - Flows
      - Flowid
      - Config
  /flow-templates/{flowTemplateId}/flows/{flowId}/config/{fileName}:
    get:
      summary: Get Flow Templates Flowtemplateid Flows Flowid Config Filename
      description: Get flow templates flowtemplateid flows flowid config filename.
      operationId: getFlowConfigFileUsingGET_1
      x-api-path-slug: flowtemplatesflowtemplateidflowsflowidconfigfilename-get
      parameters:
      - in: path
        name: fileName
        description: fileName
      - in: path
        name: flowId
        description: flowId
      responses:
        200:
          description: Successful response
      tags:
      - Flow
      - Templates
      - Flowtemplateid
      - Flows
      - Flowid
      - Config
      - Filename
    delete:
      summary: Delete Flow Templates Flowtemplateid Flows Flowid Config Filename
      description: Delete flow templates flowtemplateid flows flowid config filename.
      operationId: deleteFlowConfigFileUsingDELETE_1
      x-api-path-slug: flowtemplatesflowtemplateidflowsflowidconfigfilename-delete
      parameters:
      - in: path
        name: fileName
        description: fileName
      - in: path
        name: flowId
        description: flowId
      responses:
        200:
          description: Successful response
      tags:
      - Flow
      - Templates
      - Flowtemplateid
      - Flows
      - Flowid
      - Config
      - Filename
  /flow-templates/{flowTemplateId}/flows/{flowId}/launch:
    post:
      summary: Post Flow Templates Flowtemplateid Flows Flowid Launch
      description: Post flow templates flowtemplateid flows flowid launch.
      operationId: launchUsingPOST_1
      x-api-path-slug: flowtemplatesflowtemplateidflowsflowidlaunch-post
      parameters:
      - in: path
        name: flowId
        description: flowId
      - in: body
        name: launchRequest
        description: launchRequest
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: Successful response
      tags:
      - Flow
      - Templates
      - Flowtemplateid
      - Flows
      - Flowid
      - Launch
  /flow-templates/{flowTemplateId}/flows/{flowId}/stop:
    post:
      summary: Post Flow Templates Flowtemplateid Flows Flowid Stop
      description: Post flow templates flowtemplateid flows flowid stop.
      operationId: stopUsingPOST_1
      x-api-path-slug: flowtemplatesflowtemplateidflowsflowidstop-post
      parameters:
      - in: path
        name: flowId
        description: flowId
      responses:
        200:
          description: Successful response
      tags:
      - Flow
      - Templates
      - Flowtemplateid
      - Flows
      - Flowid
      - Stop
  /flow-templates/{flowTemplateId}/flows/{flowId}/tags:
    get:
      summary: Get Flow Templates Flowtemplateid Flows Flowid Tags
      description: Get flow templates flowtemplateid flows flowid tags.
      operationId: getFlowTagsUsingGET
      x-api-path-slug: flowtemplatesflowtemplateidflowsflowidtags-get
      parameters:
      - in: path
        name: flowId
        description: flowId
      responses:
        200:
          description: Successful response
      tags:
      - Flow
      - Templates
      - Flowtemplateid
      - Flows
      - Flowid
      - Tags
    post:
      summary: Post Flow Templates Flowtemplateid Flows Flowid Tags
      description: Post flow templates flowtemplateid flows flowid tags.
      operationId: saveFlowTagsUsingPOST_1
      x-api-path-slug: flowtemplatesflowtemplateidflowsflowidtags-post
      parameters:
      - in: path
        name: flowId
        description: flowId
      - in: body
        name: tags
        description: tags
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: Successful response
      tags:
      - Flow
      - Templates
      - Flowtemplateid
      - Flows
      - Flowid
      - Tags
  /flow-templates/{flowTemplateId}/list:
    get:
      summary: Get Flow Templates Flowtemplateid List
      description: Get flow templates flowtemplateid list.
      operationId: listFlowTemplateAnalyticFileUsingGET
      x-api-path-slug: flowtemplatesflowtemplateidlist-get
      parameters:
      - in: path
        name: flowTemplateId
        description: flowTemplateId
      responses:
        200:
          description: Successful response
      tags:
      - Flow
      - Templates
      - Flowtemplateid
      - List
  /flow-templates/{flowTemplateId}/tags:
    get:
      summary: Get Flow Templates Flowtemplateid Tags
      description: Get flow templates flowtemplateid tags.
      operationId: getTemplateTagsUsingGET
      x-api-path-slug: flowtemplatesflowtemplateidtags-get
      parameters:
      - in: path
        name: flowTemplateId
        description: flowTemplateId
      responses:
        200:
          description: Successful response
      tags:
      - Flow
      - Templates
      - Flowtemplateid
      - Tags
    post:
      summary: Post Flow Templates Flowtemplateid Tags
      description: Post flow templates flowtemplateid tags.
      operationId: saveTemplateTagsUsingPOST
      x-api-path-slug: flowtemplatesflowtemplateidtags-post
      parameters:
      - in: path
        name: flowTemplateId
        description: flowTemplateId
      - in: body
        name: tags
        description: tags
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: Successful response
      tags:
      - Flow
      - Templates
      - Flowtemplateid
      - Tags
  /flows:
    get:
      summary: Get Flows
      description: Get flows.
      operationId: getFlowsUsingGET
      x-api-path-slug: flows-get
      parameters:
      - in: query
        name: maxUpdateTime
        description: maxUpdateTime
      - in: query
        name: minUpdateTime
        description: minUpdateTime
      - in: query
        name: name
        description: name
      - in: query
        name: page
        description: Results page you want to retrieve (0
      - in: query
        name: size
        description: Number of records per page
      - in: query
        name: sort
        description: 'Sorting criteria in the format: property(,asc|desc)'
      - in: query
        name: tag
        description: tag
      - in: query
        name: type
        description: type
      responses:
        200:
          description: Successful response
      tags:
      - Flows
    post:
      summary: Post Flows
      description: Post flows.
      operationId: saveDirectFlowUsingPOST
      x-api-path-slug: flows-post
      responses:
        200:
          description: Successful response
      tags:
      - Flows
  /flows/tags:
    get:
      summary: Get Flows Tags
      description: Get flows tags.
      operationId: getAllFlowTagsUsingGET
      x-api-path-slug: flowstags-get
      responses:
        200:
          description: Successful response
      tags:
      - Flows
      - Tags
  /flows/{flowId}:
    post:
      summary: Post Flows Flowid
      description: Post flows flowid.
      operationId: updateDirectFlowUsingPOST
      x-api-path-slug: flowsflowid-post
      parameters:
      - in: path
        name: flowId
        description: flowId
      responses:
        200:
          description: Successful response
      tags:
      - Flows
      - Flowid
    delete:
      summary: Delete Flows Flowid
      description: Delete flows flowid.
      operationId: deleteFlowUsingDELETE
      x-api-path-slug: flowsflowid-delete
      parameters:
      - in: path
        name: flowId
        description: flowId
      responses:
        200:
          description: Successful response
      tags:
      - Flows
      - Flowid
  /flows/{flowId}/config:
    get:
      summary: Get Flows Flowid Config
      description: Get flows flowid config.
      operationId: listFlowConfigFilesUsingGET
      x-api-path-slug: flowsflowidconfig-get
      parameters:
      - in: path
        name: flowId
        description: flowId
      responses:
        200:
          description: Successful response
      tags:
      - Flows
      - Flowid
      - Config
    post:
      summary: Post Flows Flowid Config
      description: Post flows flowid config.
      operationId: addFlowConfigFileUsingPOST
      x-api-path-slug: flowsflowidconfig-post
      parameters:
      - in: path
        name: flowId
        description: flowId
      responses:
        200:
          description: Successful response
      tags:
      - Flows
      - Flowid
      - Config
  /flows/{flowId}/config/{fileName}:
    get:
      summary: Get Flows Flowid Config Filename
      description: Get flows flowid config filename.
      operationId: getFlowConfigFileUsingGET
      x-api-path-slug: flowsflowidconfigfilename-get
      parameters:
      - in: path
        name: fileName
        description: fileName
      - in: path
        name: flowId
        description: flowId
      responses:
        200:
          description: Successful response
      tags:
      - Flows
      - Flowid
      - Config
      - Filename
    delete:
      summary: Delete Flows Flowid Config Filename
      description: Delete flows flowid config filename.
      operationId: deleteFlowConfigFileUsingDELETE
      x-api-path-slug: flowsflowidconfigfilename-delete
      parameters:
      - in: path
        name: fileName
        description: fileName
      - in: path
        name: flowId
        description: flowId
      responses:
        200:
          description: Successful response
      tags:
      - Flows
      - Flowid
      - Config
      - Filename
  /flows/{flowId}/create-template:
    post:
      summary: Post Flows Flowid Create Template
      description: Post flows flowid create template.
      operationId: createTemplateFromDirectFlowUsingPOST
      x-api-path-slug: flowsflowidcreatetemplate-post
      parameters:
      - in: path
        name: flowId
        description: flowId
      responses:
        200:
          description: Successful response
      tags:
      - Flows
      - Flowid
      - Template
  /flows/{flowId}/download:
    get:
      summary: Get Flows Flowid Download
      description: Get flows flowid download.
      operationId: getFlowAnalyticFileUsingGET
      x-api-path-slug: flowsflowiddownload-get
      parameters:
      - in: path
        name: flowId
        description: flowId
      responses:
        200:
          description: Successful response
      tags:
      - Flows
      - Flowid
      - Download
  /flows/{flowId}/tags:
    post:
      summary: Post Flows Flowid Tags
      description: Post flows flowid tags.
      operationId: saveFlowTagsUsingPOST
      x-api-path-slug: flowsflowidtags-post
      parameters:
      - in: path
        name: flowId
        description: flowId
      - in: body
        name: tags
        description: tags
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: Successful response
      tags:
      - Flows
      - Flowid
      - Tags
  /flows/{flowName}:
    get:
      summary: Get Flows Flowname
      description: Get flows flowname.
      operationId: getFlowUsingGET
      x-api-path-slug: flowsflowname-get
      parameters:
      - in: path
        name: flowName
        description: flowName
      - in: query
        name: id
        description: id
      responses:
        200:
          description: Successful response
      tags:
      - Flows
      - Flowname
  /flows/{flowName}/launch:
    post:
      summary: Post Flows Flowname Launch
      description: Post flows flowname launch.
      operationId: launchUsingPOST
      x-api-path-slug: flowsflownamelaunch-post
      parameters:
      - in: path
        name: flowName
        description: flowName
      - in: body
        name: launchRequest
        description: launchRequest
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: Successful response
      tags:
      - Flows
      - Flowname
      - Launch
  /flows/{flowName}/stop:
    post:
      summary: Post Flows Flowname Stop
      description: Post flows flowname stop.
      operationId: stopUsingPOST
      x-api-path-slug: flowsflownamestop-post
      parameters:
      - in: path
        name: flowName
        description: flowName
      responses:
        200:
          description: Successful response
      tags:
      - Flows
      - Flowname
      - Stop
  /instances:
    get:
      summary: Get Instances
      description: Get instances.
      operationId: findInstancesUsingGET
      x-api-path-slug: instances-get
      parameters:
      - in: query
        name: flowName
        description: flowName
      - in: query
        name: maxUpdateTime
        description: maxUpdateTime
      - in: query
        name: minUpdateTime
        description: minUpdateTime
      - in: query
        name: name
        description: name
      - in: query
        name: page
        description: Results page you want to retrieve (0
      - in: query
        name: size
        description: Number of records per page
      - in: query
        name: sort
        description: 'Sorting criteria in the format: property(,asc|desc)'
      - in: query
        name: statuses
        description: statuses
      - in: query
        name: tag
        description: tag
      - in: query
        name: type
        description: type
      responses:
        200:
          description: Successful response
      tags:
      - Instances
  /instances/{instanceId}:
    get:
      summary: Get Instances Instanceid
      description: Get instances instanceid.
      operationId: getInstanceUsingGET
      x-api-path-slug: instancesinstanceid-get
      parameters:
      - in: path
        name: instanceId
        description: instanceId
      responses:
        200:
          description: Successful response
      tags:
      - Instances
      - Instanceid
    delete:
      summary: Delete Instances Instanceid
      description: Delete instances instanceid.
      operationId: stopInstanceUsingDELETE
      x-api-path-slug: instancesinstanceid-delete
      parameters:
      - in: path
        name: instanceId
        description: instanceId
      responses:
        200:
          description: Successful response
      tags:
      - Instances
      - Instanceid
  /instances/{instanceId}/appattempts/{attemptId}/containers:
    get:
      summary: Get Instances Instanceid Appattempts Attemptid Containers
      description: Get instances instanceid appattempts attemptid containers.
      operationId: getInstanceAttemptContainersUsingGET
      x-api-path-slug: instancesinstanceidappattemptsattemptidcontainers-get
      parameters:
      - in: path
        name: attemptId
        description: attemptId
      - in: path
        name: instanceId
        description: instanceId
      responses:
        200:
          description: Successful response
      tags:
      - Instances
      - Instanceid
      - Appattempts
      - Attemptid
      - Containers
  /instances/{instanceId}/config:
    get:
      summary: Get Instances Instanceid Config
      description: Get instances instanceid config.
      operationId: listInstanceConfigFileUsingGET
      x-api-path-slug: instancesinstanceidconfig-get
      parameters:
      - in: path
        name: instanceId
        description: instanceId
      responses:
        200:
          description: Successful response
      tags:
      - Instances
      - Instanceid
      - Config
  /instances/{instanceId}/config/{fileName}:
    get:
      summary: Get Instances Instanceid Config Filename
      description: Get instances instanceid config filename.
      operationId: getInstanceConfigFileUsingGET
      x-api-path-slug: instancesinstanceidconfigfilename-get
      parameters:
      - in: path
        name: fileName
        description: fileName
      - in: path
        name: instanceId
        description: instanceId
      responses:
        200:
          description: Successful response
      tags:
      - Instances
      - Instanceid
      - Config
      - Filename
  /instances/{instanceId}/containers:
    get:
      summary: Get Instances Instanceid Containers
      description: Get instances instanceid containers.
      operationId: getInstanceContainersUsingGET
      x-api-path-slug: instancesinstanceidcontainers-get
      parameters:
      - in: path
        name: instanceId
        description: instanceId
      responses:
        200:
          description: Successful response
      tags:
      - Instances
      - Instanceid
      - Containers
  /instances/{instanceId}/containers/{containerId}/logs:
    get:
      summary: Get Instances Instanceid Containers Containerid Logs
      description: Get instances instanceid containers containerid logs.
      operationId: getInstanceContainerLogsUsingGET
      x-api-path-slug: instancesinstanceidcontainerscontaineridlogs-get
      parameters:
      - in: path
        name: containerId
        description: containerId
      - in: path
        name: instanceId
        description: instanceId
      responses:
        200:
          description: Successful response
      tags:
      - Instances
      - Instanceid
      - Containers
      - Containerid
      - Logs
  /instances/{instanceId}/containers/{containerId}/logs/{logName}:
    get:
      summary: Get Instances Instanceid Containers Containerid Logs Logname
      description: Get instances instanceid containers containerid logs logname.
      operationId: getInstanceContainerLogContentsUsingGET
      x-api-path-slug: instancesinstanceidcontainerscontaineridlogslogname-get
      parameters:
      - in: path
        name: containerId
        description: containerId
      - in: path
        name: instanceId
        description: instanceId
      - in: query
        name: length
        description: length
      - in: path
        name: logName
        description: logName
      - in: query
        name: offset
        description: offset
      responses:
        200:
          description: Successful response
      tags:
      - Instances
      - Instanceid
      - Containers
      - Containerid
      - Logs
      - Logname
  /instances/{instanceId}/sparkproxy/**:
    get:
      summary: Get Instances Instanceid Sparkproxy **
      description: Get instances instanceid sparkproxy **.
      operationId: getInstanceSparkProxyUsingGET
      x-api-path-slug: instancesinstanceidsparkproxy-get
      parameters:
      - in: path
        name: instanceId
        description: instanceId
      responses:
        200:
          description: Successful response
      tags:
      - Instances
      - Instanceid
      - Sparkproxy
      - '**'
    head:
      summary: Head Instances Instanceid Sparkproxy **
      description: Head instances instanceid sparkproxy **.
      operationId: getInstanceSparkProxyUsingHEAD
      x-api-path-slug: instancesinstanceidsparkproxy-head
      parameters:
      - in: path
        name: instanceId
        description: instanceId
      responses:
        200:
          description: Successful response
      tags:
      - Head
      - Instances
      - Instanceid
      - Sparkproxy
      - '**'
    post:
      summary: Post Instances Instanceid Sparkproxy **
      description: Post instances instanceid sparkproxy **.
      operationId: getInstanceSparkProxyUsingPOST
      x-api-path-slug: instancesinstanceidsparkproxy-post
      parameters:
      - in: path
        name: instanceId
        description: instanceId
      responses:
        200:
          description: Successful response
      tags:
      - Instances
      - Instanceid
      - Sparkproxy
      - '**'
    put:
      summary: Put Instances Instanceid Sparkproxy **
      description: Put instances instanceid sparkproxy **.
      operationId: getInstanceSparkProxyUsingPUT
      x-api-path-slug: instancesinstanceidsparkproxy-put
      parameters:
      - in: path
        name: instanceId
        description: instanceId
      responses:
        200:
          description: Successful response
      tags:
      - Instances
      - Instanceid
      - Sparkproxy
      - '**'
    delete:
      summary: Delete Instances Instanceid Sparkproxy **
      description: Delete instances instanceid sparkproxy **.
      operationId: getInstanceSparkProxyUsingDELETE
      x-api-path-slug: instancesinstanceidsparkproxy-delete
      parameters:
      - in: path
        name: instanceId
        description: instanceId
      responses:
        200:
          description: Successful response
      tags:
      - Instances
      - Instanceid
      - Sparkproxy
      - '**'
    options:
      summary: Options Instances Instanceid Sparkproxy **
      description: Options instances instanceid sparkproxy **.
      operationId: getInstanceSparkProxyUsingOPTIONS
      x-api-path-slug: instancesinstanceidsparkproxy-options
      parameters:
      - in: path
        name: instanceId
        description: instanceId
      responses:
        200:
          description: Successful response
      tags:
      - Options
      - Instances
      - Instanceid
      - Sparkproxy
      - '**'
    patch:
      summary: Patch Instances Instanceid Sparkproxy **
      description: Patch instances instanceid sparkproxy **.
      operationId: getInstanceSparkProxyUsingPATCH
      x-api-path-slug: instancesinstanceidsparkproxy-patch
      parameters:
      - in: path
        name: instanceId
        description: instanceId
      responses:
        200:
          description: Successful response
      tags:
      - Instances
      - Instanceid
      - Sparkproxy
      - '**'
  /instances/{instanceId}/submit-logs:
    get:
      summary: Get Instances Instanceid Submit Logs
      description: Get instances instanceid submit logs.
      operationId: getSparkSubmitLogsUsingGET
      x-api-path-slug: instancesinstanceidsubmitlogs-get
      parameters:
      - in: path
        name: instanceId
        description: instanceId
      - in: query
        name: length
        description: length
      - in: query
        name: offset
        description: offset
      responses:
        200:
          description: Successful response
      tags:
      - Instances
      - Instanceid
      - Submit
      - Logs
  /v1/collections/{collectionName}/features:
    get:
      summary: Return feature
      description: |-
        Returns GeoJSON of type FeatureCollection containing all GeoJSON features
        from the named collection with a matching GeoJSON id.
      operationId: returns-geojson-of-type-featurecollection-containing-all-geojson-featuresfrom-the-named-collection-w
      x-api-path-slug: v1collectionscollectionnamefeatures-get
      parameters:
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Return
      - Feature
    delete:
      summary: Delete from the named collection all features with a matching GeoJSON
        id.
      description: Delete from the named collection all features with a matching GeoJSON
        id. This could be 0, 1 or many features.
      operationId: delete-from-the-named-collection-all-features-with-a-matching-geojson-id-this-could-be-0-1-or-many-f
      x-api-path-slug: v1collectionscollectionnamefeatures-delete
      parameters:
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - From
      - Named
      - Collection
      - ""
      - Features
      - Matching
      - GeoJSON
      - Id
    post:
      summary: Insert an individual feature into a collection.
      description: |-
        Insert a new feature into the the named collection. The GeoJSON id is used to identify the feature.
        The GeoJSON id included in the url must match the top level id member of the feature provided.
      operationId: insert-a-new-feature-into-the-the-named-collection-the-geojson-id-is-used-to-identify-the-featurethe
      x-api-path-slug: v1collectionscollectionnamefeatures-post
      parameters:
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Insert
      - Individual
      - Feature
      - Into
      - Collection
    put:
      summary: Update all features in a collection with a matching GeoJSON id.
      description: Updates the attributes and geometry of matching features in the
        named collection.  This could be 0, 1 or many features.
      operationId: updates-the-attributes-and-geometry-of-matching-features-in-the-named-collection--this-could-be-0-1-
      x-api-path-slug: v1collectionscollectionnamefeatures-put
      parameters:
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Features
      - In
      - Collection
      - Matching
      - GeoJSON
      - Id
  /v1/collections/{collectionName}/collectionSize:
    get:
      summary: Return the size of a collection.
      description: |-
        Returns the size of the specified collection to decide whether to use the whole collection for spatial query
        or not.
      operationId: returns-the-size-of-the-specified-collection-to-decide-whether-to-use-the-whole-collection-for-spati
      x-api-path-slug: v1collectionscollectionnamecollectionsize-get
      parameters:
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Return
      - Size
      - Of
      - Collection
  /v1/collections/{collectionName}/spatial-query:
    post:
      summary: |-
        For 'within' operator - find all points within an area.
        For 'nearest' operator - return the nearest point to the one specified.
        For 'lineIntersectsLine' - find all points of intersection between two linestrings.
      description: |-
        'Within' returns GeoGJSON of type FeatureCollection containing all GeoJSON features within the provided polygon.
        'Nearest' returns a FeatureCollection with the longitude and latitude of the nearest point.
        'LineIntersectsLine' returns a FeatureCollection containing all points of intersection as GeoJSON features.
      operationId: within-returns-geogjson-of-type-featurecollection-containing-all-geojson-features-within-the-provide
      x-api-path-slug: v1collectionscollectionnamespatialquery-post
      parameters:
      - in: body
        name: body
        description: For within query - a geojson polygon which we wish to search
        schema:
          $ref: '#/definitions/holder'
      - in: query
        name: No Name
      - in: query
        name: operator
        description: The type of spatial query
      responses:
        200:
          description: OK
      tags:
      - For
      - Within
      - Operator
      - '-'
      - Find
      - ""
      - Points
      - Within
      - Area
      - For
      - Nearest
      - Operator
      - '-'
      - Return
      - Nearest
      - Point
      - To
      - Specified
      - For
      - LineIntersectsLine
      - '-'
      - Find
      - ""
      - Points
      - Of
      - Intersection
      - Between
      - Two
      - Linestrings
  /v1/collections/{collectionName}/text:
    get:
      summary: Free text search of a feature collection
      description: |-
        Returns GeoJSON of type FeatureCollection containing all GeoJSON features from the named collection that match
        the supplied search string.

        The search text consists of one or more strings that can be space or comma separated. A match with a given
        feature occurs only if an exact match can be found for each of the strings in the search text amongst a
        concatenation of the values of child members of the top level 'properties' member of the feature,
        together with the value of its GeoJSON id. The matching is case insensitve, partial matches and
        wildcard searching is not supported.

        Examples of search text:

         - 28,West End,Histon
         - 240.000 V
         - Company Owned
      operationId: returns-geojson-of-type-featurecollection-containing-all-geojson-features-from-the-named-collection-
      x-api-path-slug: v1collectionscollectionnametext-get
      parameters:
      - in: query
        name: No Name
      - in: query
        name: q
        description: The search text
      responses:
        200:
          description: OK
      tags:
      - Free
      - Text
      - Search
      - Of
      - Feature
      - Collection
  /v1/maps:
    get:
      summary: List all maps for a customer
      description: |-
        Returns an array of maps for the specified customer. The array contains
        the name and identifier for each map.
      operationId: returns-an-array-of-maps-for-the-specified-customer-the-array-containsthe-name-and-identifier-for-ea
      x-api-path-slug: v1maps-get
      parameters:
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - List
      - ""
      - Mapsa
      - Customer
    post:
      summary: Create a map
      description: Creates a map with the specified name.
      operationId: creates-a-map-with-the-specified-name
      x-api-path-slug: v1maps-post
      parameters:
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Map
  /v1/maps/{mapId}:
    get:
      summary: Return map details
      description: |-
        For the specified map identifier, returns the map properties and an
        array of the associated layers. For each layer, the identifier, name and
        Uniform Resource Identifier (URI) are returned.
      operationId: for-the-specified-map-identifier-returns-the-map-properties-and-anarray-of-the-associated-layers-for
      x-api-path-slug: v1mapsmapid-get
      parameters:
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Return
      - Map
      - Details
    delete:
      summary: Delete a map
      description: |-
        Deletes the map with the specified identifier. Any layers associated
        with the map are also deleted.
      operationId: deletes-the-map-with-the-specified-identifier-any-layers-associatedwith-the-map-are-also-deleted
      x-api-path-slug: v1mapsmapid-delete
      parameters:
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Map
    put:
      summary: Rename a map
      description: Updates the name of the map that has the specified identifier.
      operationId: updates-the-name-of-the-map-that-has-the-specified-identifier
      x-api-path-slug: v1mapsmapid-put
      parameters:
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Rename
      - Map
  /v1/maps/{mapId}/orderlayers:
    post:
      summary: Update order of layers
      description: Updates the order of layers for a given map.
      operationId: updates-the-order-of-layers-for-a-given-map
      x-api-path-slug: v1mapsmapidorderlayers-post
      parameters:
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Order
      - Of
      - Layers
  /v1/maps/{mapId}/layers:
    post:
      summary: Create a new layer
      description: Creates a new layer and associates it with the specified map.
      operationId: creates-a-new-layer-and-associates-it-with-the-specified-map
      x-api-path-slug: v1mapsmapidlayers-post
      parameters:
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - New
      - Layer
  /v1/maps/{mapId}/layers/{layerId}:
    get:
      summary: Return layer details
      description: |-
        For the layer identified by the map and layer identifiers, returns the
        layer details (identifier, name, Uniform Resource Identifier (URI), and
        visibility).
      operationId: for-the-layer-identified-by-the-map-and-layer-identifiers-returns-thelayer-details-identifier-name-u
      x-api-path-slug: v1mapsmapidlayerslayerid-get
      parameters:
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Return
      - Layer
      - Details
    put:
      summary: Update the layer properties
      description: |-
        For the layer identified by the specified map and layer identifiers,
        updates the layer properties.
      operationId: for-the-layer-identified-by-the-specified-map-and-layer-identifiersupdates-the-layer-properties
      x-api-path-slug: v1mapsmapidlayerslayerid-put
      parameters:
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Layer
      - Properties
    delete:
      summary: Delete a layer
      description: Deletes the layer identified by the specified map and layer identifiers.
      operationId: deletes-the-layer-identified-by-the-specified-map-and-layer-identifiers
      x-api-path-slug: v1mapsmapidlayerslayerid-delete
      parameters:
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Layer
  /v1/maps/{mapId}/layers/{layerId}/style:
    get:
      summary: Retrieves style data for a layer
      description: |-
        Retrieve style data for the layer identified by the specified map and
        layer identifiers.
      operationId: retrieve-style-data-for-the-layer-identified-by-the-specified-map-andlayer-identifiers
      x-api-path-slug: v1mapsmapidlayerslayeridstyle-get
      parameters:
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Retrieves
      - Style
      - Dataa
      - Layer
    put:
      summary: Update the style data for a layer
      description: |-
        Update the style data for the layer identified by the specified map and
        layer identifiers.
      operationId: update-the-style-data-for-the-layer-identified-by-the-specified-map-andlayer-identifiers
      x-api-path-slug: v1mapsmapidlayerslayeridstyle-put
      parameters:
      - in: body
        name: body
        description: Style data
        schema:
          $ref: '#/definitions/holder'
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Style
      - Dataa
      - Layer
  /v1/tenants/{tenant_uuid}/configurations:
    get:
      summary: Get Tenants Configurations
      description: Get tenants configurations.
      operationId: getV1TenantsTenantUuConfigurations
      x-api-path-slug: v1tenantstenant-uuidconfigurations-get
      parameters:
      - in: query
        name: configurationUuid
        description: configurationUuid
      - in: path
        name: tenant_uuid
        description: tenant_uuid
      responses:
        200:
          description: OK
      tags:
      - Tenants
      - Configurations
    post:
      summary: Post Tenants Configurations
      description: Post tenants configurations.
      operationId: postV1TenantsTenantUuConfigurations
      x-api-path-slug: v1tenantstenant-uuidconfigurations-post
      parameters:
      - in: body
        name: configurations
        description: configurations
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: tenant_uuid
        description: tenant_uuid
      responses:
        200:
          description: OK
      tags:
      - Tenants
      - Configurations
  /v1/tenants/{tenant_uuid}/configurations/{uuid}:
    get:
      summary: Get Tenants Configurations
      description: Get tenants configurations.
      operationId: getV1TenantsTenantUuConfigurationsUu
      x-api-path-slug: v1tenantstenant-uuidconfigurationsuuid-get
      parameters:
      - in: path
        name: tenant_uuid
        description: tenant_uuid
      - in: path
        name: uuid
        description: uuid
      responses:
        200:
          description: OK
      tags:
      - Tenants
      - Configurations
    put:
      summary: Put Tenants Configurations
      description: Put tenants configurations.
      operationId: putV1TenantsTenantUuConfigurationsUu
      x-api-path-slug: v1tenantstenant-uuidconfigurationsuuid-put
      parameters:
      - in: body
        name: configuration
        description: configuration
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: tenant_uuid
        description: tenant_uuid
      - in: path
        name: uuid
        description: uuid
      responses:
        200:
          description: OK
      tags:
      - Tenants
      - Configurations
    delete:
      summary: Delete Tenants Configurations
      description: Delete tenants configurations.
      operationId: deleteV1TenantsTenantUuConfigurationsUu
      x-api-path-slug: v1tenantstenant-uuidconfigurationsuuid-delete
      parameters:
      - in: path
        name: tenant_uuid
        description: tenant_uuid
      - in: path
        name: uuid
        description: uuid
      responses:
        200:
          description: OK
      tags:
      - Tenants
      - Configurations
  /v1/tenants/{tenant_uuid}/email:
    post:
      summary: Post Tenants Email
      description: Post tenants email.
      operationId: postV1TenantsTenantUuEmail
      x-api-path-slug: v1tenantstenant-uuidemail-post
      parameters:
      - in: body
        name: applicationMessage
        description: applicationMessage
        schema:
          $ref: '#/definitions/holder'
      - in: query
        name: configuration
        description: configuration
      - in: path
        name: tenant_uuid
        description: tenant_uuid
      responses:
        200:
          description: OK
      tags:
      - Tenants
      - Email
  /v1/tenants/{tenant_uuid}/usage:
    get:
      summary: Get Tenants Usage
      description: Get tenants usage.
      operationId: getV1TenantsTenantUuUsage
      x-api-path-slug: v1tenantstenant-uuidusage-get
      parameters:
      - in: query
        name: end_date
        description: end_date
      - in: query
        name: start_date
        description: start_date
      - in: path
        name: tenant_uuid
        description: tenant_uuid
      responses:
        200:
          description: OK
      tags:
      - Tenants
      - Usage
  /v1/registrations:
    post:
      summary: Post Registrations
      description: |-
        The following parameters can be used to validate the user's request.
        The parameters are optional, but the sample code includes email as part of the requestParams.post method.
      operationId: postV1Registrations
      x-api-path-slug: v1registrations-post
      parameters:
      - in: body
        name: body
        description: Body Parameters
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Registrations
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