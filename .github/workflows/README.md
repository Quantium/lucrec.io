# GitHub Actions Workflows

## Deploy to AWS S3

This workflow automatically deploys the site to AWS S3 when code is pushed to the `main` branch.

### Required GitHub Secrets

Configure the following secrets in your GitHub repository (Settings → Secrets and variables → Actions):

1. **AWS_ACCESS_KEY_ID** - Your AWS access key ID
2. **AWS_SECRET_ACCESS_KEY** - Your AWS secret access key
3. **AWS_REGION** - AWS region (e.g., `us-east-1`, `us-west-2`, `eu-west-1`)
4. **S3_BUCKET_NAME** - Name of your S3 bucket (e.g., `my-bucket-name`)
5. **CLOUDFRONT_DISTRIBUTION_ID** (optional) - CloudFront distribution ID if you're using CloudFront

### Setup Instructions

1. Create an S3 bucket in AWS for your site
2. Configure the bucket for static website hosting:
   - Enable "Static website hosting"
   - Set index document to `index.html`
   - Set up bucket policy to allow public read access
3. (Optional) Set up CloudFront distribution for the S3 bucket
4. Create an IAM user with the following permissions:
   - `s3:PutObject`
   - `s3:GetObject`
   - `s3:DeleteObject`
   - `s3:ListBucket`
   - `cloudfront:CreateInvalidation` (if using CloudFront)
5. Add the secrets to your GitHub repository
6. Push to the `main` branch to trigger deployment

### Manual Deployment

You can also trigger deployments manually by going to Actions → Deploy to AWS S3 → Run workflow
