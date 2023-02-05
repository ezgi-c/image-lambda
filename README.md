# Lab Class 17 - AWS: S3 and Lambda

## Documentation

- a description of how to use your lambda.  
We created function named ImageSummarizer in Lambda, and connected it to our S3 bucket that accepts image files.  
We added an event trigger to the Lambda function which activates when a file is added to the bucket.  
We also configured Lambda role policy to access actions on the S3 buckets such as `GetObject` and `PutObject`
- a description of any issues you encountered during deployment of this lambda.  
I reviewed the lecture and the whiteboard David created to complete the lab. I was able to get it to work up to the point David got it to work. I currently get the following error for which I plan to spend more time to troubleshoot:

    ``` js
    Response
    {
    "errorType": "SyntaxError",
    "errorMessage": "Unexpected token o in JSON at position 1",
    "trace": [
        "SyntaxError: Unexpected token o in JSON at position 1",
        "    at JSON.parse (<anonymous>)",
        "    at Runtime.handler (file:///var/task/index.mjs:24:26)",
        "    at process.processTicksAndRejections (node:internal/process/task_queues:95:5)"
    ]
    }
    ```

- a link to your images.json file.  
 [summary.json](https://ezgi-images.s3.us-west-2.amazonaws.com/summary.json)  
 [summary.json](https://s3.console.aws.amazon.com/s3/object/ezgi-images?region=us-west-2&prefix=summary.json)
