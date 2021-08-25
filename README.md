


Improved:

1.Set up AWS service(S3,SNS,SQS) and make the project run.

2.ExcelService/ExcelServiceImpl:
  Now Excel service can also upload files to S3 and delete the local one.

3.ClientService/ReportServiceImpl:
  sendDirectRequset() now change to parallel process using Threadpool and Future Interface.
  getFileBodyByReqId() now can get both PDF and excel file from Amazon s3 rather than from local.


Bug fixed:

1.ExcelServicd/ExcelGenerationServiceImpl:
  Method generateExcelReport() doesn't close the outputStream properly. Now it closed properly.


