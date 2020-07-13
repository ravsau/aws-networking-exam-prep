
## How Cloudfront delivers content? 
  - After you configure CloudFront to deliver your content, here's what happens when users request your files:

      - A user accesses your website or application and requests one or more files, such as an image file and an HTML file.

      - DNS routes the request to the CloudFront POP (edge location) that can best serve the request—typically the nearest CloudFront POP in terms of latency—and routes the request to that edge location.

      - In the POP, CloudFront checks its cache for the requested files. If the files are in the cache, CloudFront returns them to the user. If the files are not in the cache, it does the following:

      - CloudFront compares the request with the specifications in your distribution and forwards the request for the files to your origin server for the corresponding file type—for example, to your Amazon S3 bucket for image files and to your HTTP server for HTML files.

      - The origin servers send the files back to the edge location.

      - As soon as the first byte arrives from the origin, CloudFront begins to forward the files to the user. CloudFront also adds the files to the cache in the edge location for the next time someone requests those files.
  
  - https://docs.aws.amazon.com/AmazonCloudFront/latest/DeveloperGuide/HowCloudFrontWorks.html
  
  
  
  ## Cloudfront User Request flow
  User-->Cloudfront POP--> Cloudfront Regional Cache--> Origin
