# SDT316 — AWS Infrastructure Assignment

## Task 2.5 — Public subnet routing

The `0.0.0.0/0` route pointing to the Internet Gateway is what makes the subnet public: it provides a path to destinations outside the VPC. If it were deleted, the EC2 instance would lose direct internet connectivity even if it still had a public IPv4 address and inbound security group rules allowed HTTP and SSH.

## Task 3.4 — Security group troubleshooting

Before the security group change, the browser showed `ERR_CONNECTION_TIMED_OUT`, not `connection refused`. The instance served `HTTP/1.1 200 OK` locally, but its security group did not permit inbound TCP port 80, so that traffic was dropped; by contrast, `connection refused` typically means a TCP connection reached a host that had no service accepting connections on that port.

## Task 4.5 — S3 public access

Disabling **Block Public Access** removes a safeguard that otherwise prevents a public bucket policy from taking effect; it does not grant public read access by itself. The bucket policy supplies that permission through `Principal: "*"` and `s3:GetObject` for the website objects. Both changes were necessary for this assignment's direct public S3 website endpoint.

## Website URL

http://sdt316-naumenko-site.s3-website.eu-central-1.amazonaws.com/
