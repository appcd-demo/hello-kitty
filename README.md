# hello-kitty

<a href="https://docs.stackgen.com/getting-started"><img src="https://img.shields.io/badge/StackGen%20docs-141416?style=flat&logo=data:image/svg+xml;base64,PD94bWwgdmVyc2lvbj0iMS4wIiBlbmNvZGluZz0iVVRGLTgiPz4KPHN2ZyBpZD0iTGF5ZXJfMiIgZGF0YS1uYW1lPSJMYXllciAyIiB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHZpZXdCb3g9IjAgMCAzODcuNSA2MDAiPgogIDxkZWZzPgogICAgPHN0eWxlPgogICAgICAuY2xzLTEgewogICAgICAgIGZpbGw6ICM3OWM4NDI7CiAgICAgIH0KCiAgICAgIC5jbHMtMSwgLmNscy0yIHsKICAgICAgICBzdHJva2Utd2lkdGg6IDBweDsKICAgICAgfQoKICAgICAgLmNscy0yIHsKICAgICAgICBmaWxsOiAjM2VhOGY0OwogICAgICB9CiAgICA8L3N0eWxlPgogIDwvZGVmcz4KICA8cGF0aCBjbGFzcz0iY2xzLTEiIGQ9Im0yNDguODUsMzEzLjJsLTQzLjA4LDQzLjA4YzMuODcsMTIuNzIuODEsMjcuMS05LjIzLDM3LjE0bC05Mi45NSw5Mi45NWMtMTAuOTYsMTAuOTYtMTEuMDEsMjguODQtLjExLDM5Ljg1LDUuMzMsNS4zOSwxMi40NCw4LjM2LDIwLjAxLDguMzhoLjA4YzcuNTUsMCwxNC42NC0yLjk0LDE5Ljk4LTguMjhsMTM5LjIzLTEzOS4yM2MxMS4wMi0xMS4wMiwxMS4wMi0yOC45NCwwLTM5Ljk2bC0zMy45My0zMy45M1oiLz4KICA8cGF0aCBjbGFzcz0iY2xzLTIiIGQ9Im0xMjQuNiw0MDAuMzdoLjA4YzcuNTUsMCwxNC42NC0yLjk0LDE5Ljk4LTguMjhsMTM5LjIzLTEzOS4yM2M1LjM0LTUuMzQsOC4yOC0xMi40Myw4LjI4LTE5Ljk4cy0yLjk0LTE0LjY0LTguMjgtMTkuOThMMTQ0LjY1LDczLjY3Yy01LjM0LTUuMzQtMTIuNDMtOC4yOC0xOS45OC04LjI4aC0uMDhjLTcuNTguMDItMTQuNjgsMy0yMC4wMSw4LjM4LTEwLjksMTEuMDItMTAuODUsMjguOS4xLDM5Ljg1bDkyLjk1LDkyLjk0YzcuMDMsNy4wMywxMC45LDE2LjM3LDEwLjksMjYuMzFzLTMuODcsMTkuMjgtMTAuOSwyNi4zMWwtOTIuOTUsOTIuOTVjLTEwLjk2LDEwLjk2LTExLjAxLDI4Ljg0LS4xLDM5Ljg1LDUuMzMsNS4zOSwxMi40NCw4LjM2LDIwLjAxLDguMzhaIi8+CiAgPHBhdGggY2xhc3M9ImNscy0xIiBkPSJtMTQzLjU1LDIwNy45Yy01LjM0LTUuMzQtMTIuNDMtOC4yOC0xOS45OC04LjI4aC0uMDhjLTcuNTguMDItMTQuNjgsMy0yMC4wMSw4LjM4LTEwLjksMTEuMDItMTAuODUsMjguOS4xMSwzOS44NWw0MC4wMyw0MC4wMywzOS45Ni0zOS45Ni00MC4wMy00MC4wM1oiLz4KPC9zdmc+&labelColor=141416&logoColor=white" alt="badge for stackgen docs" height=35 /></a>

hello-kitty is a static website that shows random photos of a cat from an S3 bucket. It is written in Python and can be deployed to AWS Lambda and S3. 

We encourage you to use StackGen to generate IaC for this sample app. StackGen provides a powerful and flexible way to define and manage your infrastructure.

Get started with IaC generation for this repo by following the instructions on [StackGen Documentation](https://docs.stackgen.com/getting-started)

### Environment variables

- IMAGES_BUCKET: S3 bucket name where images are stored

## Other Sample Projects to try

- [retroboard](https://github.com/appcd-demo/retroboard) - python app that can be deployed to AWS Lambda, DynamoDB, SQS, S3, SNS

## Example Github Actions Workflows

This demo repo includes a few examples of Github Actions Workflows that you can use to deploy your app. Fork this repo and follow below instructions to deploy your own copy.

> [!NOTE]
> You'll need to add `AWS_ROLE_TO_ASSUME` as a secret in your repository settings to use below workflows.
- [infra-pr.yml](.github/workflows/infra-pr.yml) - This workflow is triggered when any changes are detected in the `infra/terraform` directory. It comments with Terraform plan output on the PR.
- [infra-apply.yml](.github/workflows/infra-apply.yml) - This workflow is triggered when a PR is merged to main. It applies the changes to AWS.

> [!IMPORTANT]
> You'll need to add `APPSTACK_ID` as a variable in your repository settings to use below workflows.

- [manual-pull.yml](.github/workflows/manual-pull.yml) - This workflow is triggered when you click the `Run workflow` button. It uses the `appcd-dev/download-action` to download the IaC for the appstack and creates a PR with the changes.
## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.

## Photo credits

Attribution for photos in images/ is in text files in the same directory.
