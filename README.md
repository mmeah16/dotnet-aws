# .NET and AWS

This repository demonstrates how to use .NET with a variety of different AWS services.

## Cognito

AWS Cognito is a service that enables developers to add authentication, authorization, and user management to their web and mobile applications.

In this application, Cognito is used to generate access tokens to use as Bearer tokens for secure endpoints.

## Setting Secrets

Setting secrets is an effective way to commit code changes to version control without exposing credentials. Setting secrets can be done with the following commands.

```console
# Generate a secrets file

dotnet user-secrets init

# Syntax to assign a user secrets value for Authority (child of JwtBearer)

dotnet user-secrets set "JwtBearer:Authority" "https://cognito-idp.<AWS_REGION>.amazonaws.com/<AWS_REGION>_<USER-POOL-ID>"
```
