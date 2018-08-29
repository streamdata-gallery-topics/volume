swagger: "2.0"
x-collection-name: Hewlett Packard Enterprise (HPE)
x-complete: 1
info:
  title: HPE OneSphere API
  description: hpe-onesphere-hybrid-cloud-management-rest-api-for-calls-requiring-authentication-use-restsession-to-get-a-token-
  termsOfService: http://www.hpe.com/onesphere
  contact:
    name: HPE OneSphere API team
    url: http://www.hpe.com/onesphere
  version: 1.0.0
host: deic02-hpe.hpeonesphere.com
basePath: /rest
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /volumes:
    get:
      summary: Get Volumes
      description: Returns volumes. It requires any project role or non-'consumer'
        global role.
      operationId: FindVolumes
      x-api-path-slug: volumes-get
      parameters:
      - in: query
        name: query
        description: URI query string to prune volumes by
      - in: query
        name: view
        description: 'Return related resources:  * `full` - include zone, volume details'
      responses:
        200:
          description: OK
      tags:
      - Volumes
    post:
      summary: Post Volumes
      description: Creates a new volume. It requires any project role or the **administrator**
        or **project creator** global role.
      operationId: CreateVolume
      x-api-path-slug: volumes-post
      parameters:
      - in: body
        name: volume
        description: Add new volume
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Volumes
  /volumes/{id}:
    delete:
      summary: Delete Volumes
      description: Delete a volume. It requires any project role or the **administrator**
        or **project creator** global role.
      operationId: DeleteVolume
      x-api-path-slug: volumesid-delete
      parameters:
      - in: path
        name: id
        description: ID of volume to delete
      responses:
        200:
          description: OK
      tags:
      - Volumes
    get:
      summary: Get Volumes
      description: Returns a volume based on its id. It requires any project role
        or non-'consumer' global role.
      operationId: GetVolumeById
      x-api-path-slug: volumesid-get
      parameters:
      - in: path
        name: id
        description: ID of volume to fetch
      responses:
        200:
          description: OK
      tags:
      - Volumes
    patch:
      summary: Patch Volumes
      description: Updates a volume. **Requires any project role or 'administrator'
        or 'project creator' global role**. Allowed fields for PATCH of volumes are
        name(add,replace), size(add,replace)
      operationId: UpdateVolume
      x-api-path-slug: volumesid-patch
      parameters:
      - in: path
        name: id
        description: ID of volume to update
      - in: body
        name: volume
        description: Update volume
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Volumes