# Azure resources (CW2)

## Storage (Blob)
- Storage account: carsnapstorage
- Container: media
- Primary Blob endpoint: https://carsnapstorage.blob.core.windows.net/

## Notes
- Container access: Private

## Cosmos DB
- Account: carsnapcosmosdb
- Database: carsnap
- Container: posts
- Partition key: /id

## Azure SQL
- Server: carsnap-sql-19378
- Database: carsnapdb
- Tables: Users, Likes
- Demo user: demoUser (UserId=1)

## Logic Apps
- Logic App name: la-carsnap-uploadpost
- HTTP URL: https://prod-49.uksouth.logic.azure.com:443/workflows/8d83d467824241b9a34f079387221224/triggers/When_an_HTTP_request_is_received/paths/invoke?api-version=2016-10-01&sp=%2Ftriggers%2FWhen_an_HTTP_request_is_received%2Frun&sv=1.0&sig=mM2TOWW4jV2c-qcwhKLOp0COSjc4MW2xXYHpI9vsCAg

- Logic App name: la-carsnap-getfeed
- HTTP URL: https://prod-53.uksouth.logic.azure.com/workflows/e4311ffc10e348c6bf6592acbdfa66a1/triggers/When_an_HTTP_request_is_received/paths/invoke/api/posts?api-version=2016-10-01&sp=%2Ftriggers%2FWhen_an_HTTP_request_is_received%2Frun&sv=1.0&sig=Wn88rKldqmZY70jtvAHDDRCctvRPMYtILPQl6tHn57k