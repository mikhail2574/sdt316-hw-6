# SDT316 — AWS VPC, EC2 and S3 evidence

This folder contains screenshots from the actual AWS Academy exercises and AWS infrastructure setup, plus the three required written answers.

## Evidence

| File | Evidence |
| --- | --- |
| `screenshots/01-modules-5-7-knowledge-checks.png` | Scores for Modules 5, 6, and 7 knowledge checks |
| `screenshots/02-labs-1-3-scores.png` | Lab 1, 2, and 3 scores |
| `screenshots/03-vpc-route-table.png` | `sdt316-vpc` with local and Internet Gateway routes |
| `screenshots/04-public-subnet.png` | Public subnet with `10.0.1.0/24` and auto-assign public IP enabled |
| `screenshots/05-ec2-instance.png` | Running EC2 instance in the intended VPC/subnet |
| `screenshots/06-ssh-nginx-local-200.png` | SSH session, nginx service state, local HTTP 200 response |
| `screenshots/07-browser-http-timeout.png` | Browser timeout before HTTP was allowed |
| `screenshots/08-browser-nginx-working.png` | nginx welcome page accessible from browser |
| `screenshots/09-s3-website.png` | Public S3 static website endpoint working |
| `answers.md` | Responses for Tasks 2.5, 3.4, 4.5 and site URL |

AWS 12-digit account IDs visible in the original AWS Console screenshots have been covered with opaque rectangles.

## Evidence limitations

- The AWS Academy screenshots show **knowledge-check and lab scores**, not the dedicated module-completion progress page requested by the assignment. If needed, add a screenshot of the Modules 5–7 completion/progress view.
- Lab 3's visible score is **60/100**; whether that qualifies as completed depends on the course requirements.
- The Route Table screenshot identifies the VPC, but the package does not contain a separate **Your VPCs** overview screenshot.
- The S3 screenshot displays `Created by MN` rather than a full name. If strict marking requires a full name, update `index.html` in S3 and recapture the page.
- The S3 website may stop being reachable if the bucket is made private or deleted after submission.
