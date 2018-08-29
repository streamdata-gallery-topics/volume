---
swagger: "2.0"
x-collection-name: Google Books
x-complete: 0
info:
  title: Google Books API Remove Volume
  description: Removes a volume from a bookshelf.
  contact:
    name: Google
    url: https://google.com
  version: v1
host: www.googleapis.com
basePath: /books/v1
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /mylibrary/bookshelves/{shelf}/addVolume:
    post:
      summary: Add Volume
      description: Adds a volume to a bookshelf.
      operationId: books.mylibrary.bookshelves.addVolume
      x-api-path-slug: mylibrarybookshelvesshelfaddvolume-post
      parameters:
      - in: query
        name: reason
        description: The reason for which the book is added to the library
      - in: path
        name: shelf
        description: ID of bookshelf to which to add a volume
      - in: query
        name: source
        description: String to identify the originator of this request
      - in: query
        name: volumeId
        description: ID of volume to add
      responses:
        200:
          description: OK
      tags:
      - Volume
  /mylibrary/bookshelves/{shelf}/clearVolumes:
    post:
      summary: Clear Volumes
      description: Clears all volumes from a bookshelf.
      operationId: books.mylibrary.bookshelves.clearVolumes
      x-api-path-slug: mylibrarybookshelvesshelfclearvolumes-post
      parameters:
      - in: path
        name: shelf
        description: ID of bookshelf from which to remove a volume
      - in: query
        name: source
        description: String to identify the originator of this request
      responses:
        200:
          description: OK
      tags:
      - Volume
  /mylibrary/bookshelves/{shelf}/moveVolume:
    post:
      summary: Move Voume
      description: Moves a volume within a bookshelf.
      operationId: books.mylibrary.bookshelves.moveVolume
      x-api-path-slug: mylibrarybookshelvesshelfmovevolume-post
      parameters:
      - in: path
        name: shelf
        description: ID of bookshelf with the volume
      - in: query
        name: source
        description: String to identify the originator of this request
      - in: query
        name: volumeId
        description: ID of volume to move
      - in: query
        name: volumePosition
        description: Position on shelf to move the item (0 puts the item before the
          current first item, 1 puts it between the first and the second and so on
      responses:
        200:
          description: OK
      tags:
      - Volume
  /mylibrary/bookshelves/{shelf}/removeVolume:
    post:
      summary: Remove Volume
      description: Removes a volume from a bookshelf.
      operationId: books.mylibrary.bookshelves.removeVolume
      x-api-path-slug: mylibrarybookshelvesshelfremovevolume-post
      parameters:
      - in: query
        name: reason
        description: The reason for which the book is removed from the library
      - in: path
        name: shelf
        description: ID of bookshelf from which to remove a volume
      - in: query
        name: source
        description: String to identify the originator of this request
      - in: query
        name: volumeId
        description: ID of volume to remove
      responses:
        200:
          description: OK
      tags:
      - Volume
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