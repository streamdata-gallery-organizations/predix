---
swagger: "2.0"
x-collection-name: Predix
x-complete: 0
info:
  title: Predix Analytics Runtime Update the default tag query for the tenant.
  version: 1.0.0
  description: Updates the default tag query including all information (query string,
    fieldnamespecifier, tagnamespecifer, description etc.) associated with the query.
host: predix-acs.run.aws-usw02-pr.ice.predix.io
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
        2:
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
        2:
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
        2:
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
        2:
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
        2:
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
        2:
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
        2:
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
        2:
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
        2:
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
        2:
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
        2:
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
        2:
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
        2:
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
        2:
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
        2:
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
        2:
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