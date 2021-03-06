---
swagger: "2.0"
x-collection-name: Open Science Framework
x-complete: 0
info:
  title: Open Science Framework Retrieve the Content of a Wiki
  description: |-
    Retrieves the plaintext content of a wiki in markdown format.
    ####Returns
    Returns `text/markdown` of the wiki content itself.
    If the request is unsuccessful, plaintext with the error message will be displayed.
  contact:
    name: OSF
    url: https://osf.io/support
    email: support@osf.io
  version: "2.0"
host: test-api.osf.io
basePath: /v2
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /wikis/{wiki_id}/content/:
    get:
      summary: Retrieve the Content of a Wiki
      description: |-
        Retrieves the plaintext content of a wiki in markdown format.
        ####Returns
        Returns `text/markdown` of the wiki content itself.
        If the request is unsuccessful, plaintext with the error message will be displayed.
      operationId: wiki_content
      x-api-path-slug: wikiswiki-idcontent-get
      parameters:
      - in: path
        name: wiki_id
        description: The unique identifier of the wiki
      responses:
        200:
          description: OK
      tags:
      - Wikis
      - Wiki
      - Content
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