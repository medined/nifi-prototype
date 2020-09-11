# Tasks

## Testing Tasks

* Utility to create PDF file. Use "lorem ipsum" to generate text on each page. The number of pages, words, paragraphs and columns should be configurable. The generated text should be available separately so that the OCR process can be compared to ground truth.

* Utility to watch an S3 bucket and send a pre-signed URL for new objects to an SQS bucket. Additional information for the SQS message will be defined later but will include a least three PUT pre-signed URLs.

* Utiltiy to send "fake" metrics to ElasticSearch.

## OCR Tasks

* NiFi flow to monitor SQS queue. ExecuteStreamCommand can be used to run python scripts as needed. For each message:
    * read message from incoming SQS queue
    * send message to ElasticSearch
    * read the PDF file at the pre-signed URL
    * store PDF file into Data Lake
    * convert PDF pages into PNG files
    * use tesseract to perform OCR
    * create searchable PDF - put to pre-signed URL and ElasticSearch
    * store searchable PDF into Data Lake
    * extract text - put to pre-signed URL and ElasticSearch
    * store text into Data Lake
    * find bounding boxes - put to pre-signed URL and ElasticSearch
    * store bounding boxes into Data Lake
    * send status message to outgoing SQS queue and ElasticSearch
    * delete message from SQS

## UI Tasks

* Create dashboard:
    * display metrics
    * display exceptions
    * display in-flight statistics
    * display completed tasks


## O&M Tasks

* Send exceptions to ElasticSerch.
* Use configurable variables when possible
