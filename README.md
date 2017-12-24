# arautosprata

Repository containing my D&amp;D group website.

## Install

Clone the repository:

```
git clone git@github.com:hugomarques/arautosprata.git
```

Build project:

```
cd arautosprata/
bundle install
```

## Run

Execute the following command:

```
jekyll serve
```

For details how to run a jekyll website, check [Jekyll](https://jekyllrb.com/docs/home/).

## Deploy

Verify you have AWS credentials. Export your credentials:

```
export ACCESS_KEY=<YOUR_AWS_ACCESS_KEY>
export SECRET_KEY=<YOUR_AWS_SECRET_KEY>
```

Verify you have a existing S3 bucket configured for static website hosting.

Build the website and deploy with s3_website:

```
jekyll build
s3_website push
```

## References

1. Jekyll: https://jekyllrb.com/docs/home/
2. s3_website: https://github.com/laurilehmijoki/s3_website
3. AWS S3: https://docs.aws.amazon.com/AmazonS3/latest/dev/WebsiteHosting.html
