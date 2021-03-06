---
swagger: "2.0"
x-collection-name: Instructure
x-complete: 0
info:
  title: Instructure Canvas Courses API List content migrations
  description: List content migrations.
  termsOfService: https://www.canvaslms.com/policies/api-policy
  version: v1
host: canvas.instructure.com
basePath: /api/v1
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /courses/{course_id}/content_exports:
    get:
      summary: List content exports
      description: List content exports.
      operationId: list-content-exports
      x-api-path-slug: coursescourse-idcontent-exports-get
      responses:
        200:
          description: OK
      tags:
      - Courses
      - Course
      - Id
      - Content
      - Exports
    post:
      summary: Export content
      description: Export content.
      operationId: export-content
      x-api-path-slug: coursescourse-idcontent-exports-post
      parameters:
      - in: query
        name: export_type
        description: u201ccommon_cartridgeu201dnnExport the contents of the course
          in the Common Cartridge (
      - in: query
        name: skip_notifications
        description: Don&#39;t send the notifications about the export to the user
      responses:
        200:
          description: OK
      tags:
      - Courses
      - Course
      - Id
      - Content
      - Exports
  /courses/{course_id}/content_exports/id:
    get:
      summary: Show content export
      description: Show content export.
      operationId: show-content-export
      x-api-path-slug: coursescourse-idcontent-exportsid-get
      responses:
        200:
          description: OK
      tags:
      - Courses
      - Course
      - Id
      - Content
      - Exports
      - Id
  /courses/{course_id}/content_licenses:
    get:
      summary: List licenses
      description: List licenses.
      operationId: list-licenses
      x-api-path-slug: coursescourse-idcontent-licenses-get
      responses:
        200:
          description: OK
      tags:
      - Courses
      - Course
      - Id
      - Content
      - Licenses
  /courses/{course_id}/content_migrations:
    get:
      summary: List content migrations
      description: List content migrations.
      operationId: list-content-migrations
      x-api-path-slug: coursescourse-idcontent-migrations-get
      responses:
        200:
          description: OK
      tags:
      - Courses
      - Course
      - Id
      - Content
      - Migrations
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