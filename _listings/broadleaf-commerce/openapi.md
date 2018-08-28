swagger: "2.0"
x-collection-name: Broadleaf Commerce
x-complete: 1
info:
  title: Broadleaf Commerce API
  description: the-default-broadleaf-commerce-apis
  version: 1.0.0
host: demo.broadleafcommerce.org
basePath: /api/v1
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /catalog/category/{id}/media:
    get:
      summary: Get Catalog Category Media
      description: Get catalog category media.
      operationId: getCatalogCategoryMedia
      x-api-path-slug: catalogcategoryidmedia-get
      parameters:
      - in: path
        name: id
        description: id
      responses:
        200:
          description: OK
      tags:
      - Catalog
      - Category
      - Media
  /catalog/product/{productId}/media:
    get:
      summary: Get Catalog Product Media
      description: Get catalog product media.
      operationId: getCatalogProductProductMedia
      x-api-path-slug: catalogproductproductidmedia-get
      parameters:
      - in: path
        name: productId
        description: productId
      responses:
        200:
          description: OK
      tags:
      - Catalog
      - Product
      - Media
  /catalog/sku/{skuId}/media:
    get:
      summary: Get Catalog Sku Skuid Media
      description: Get catalog sku skuid media.
      operationId: getCatalogSkuSkuMedia
      x-api-path-slug: catalogskuskuidmedia-get
      parameters:
      - in: path
        name: skuId
        description: skuId
      responses:
        200:
          description: OK
      tags:
      - Catalog
      - Sku
      - Skuid
      - Media