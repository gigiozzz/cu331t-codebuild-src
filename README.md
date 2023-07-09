# cu331t-codebuild-src

a simple project to test AWS Codebuild

## How to run locally

### Prerequisites

https://docs.aws.amazon.com/codebuild/latest/userguide/use-codebuild-agent.html

### Command to run
```bash
./codebuild_build.sh -c -d \
  -b ./buildspec-app.yaml \
  -i public.ecr.aws/codebuild/amazonlinux2-x86_64-standard:5.0 \
  -s ./ \
  -a ./ \
  -e ./parameters.env
```
