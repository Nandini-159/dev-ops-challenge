Created S3 Bucket 1 (Primary Origin)

Uploaded index.html → “Hello, CDN origin is working fine”

Enabled OAC access later, kept bucket private.

Created S3 Bucket 2 (Secondary Origin)

Created folder devops-folder/

Uploaded index.html inside that folder → “Hello, CDN 2 origin is working fine”

Created CloudFront Distribution

Added Primary S3 bucket as the default origin

Enabled OAC

Set Minimum TTL = 48 hours for default behavior

Viewer protocol → Redirect HTTP to HTTPS

Added Second Origin in CloudFront

Selected Secondary S3 bucket as second origin

Created Behavior for /devops-folder/*

Path pattern: /devops-folder/*

Attached to Secondary Bucket

Viewer protocol: Redirect HTTP → HTTPS

OAC Applied Automatically

CloudFront added bucket policies for secure access (kept both S3 buckets private)

Tested Output

https://xxxx.cloudfront.net/ → Hello, CDN origin is working fine

https://xxxx.cloudfront.net/devops-folder/ → Hello, CDN 2 origin is working fine
