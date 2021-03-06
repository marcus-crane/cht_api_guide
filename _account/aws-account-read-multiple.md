---
title: AWS Accounts in CloudHealth
position: 2
description: Get a list of all AWS Accounts that are enabled in the CloudHealth Platform.
type: get
endpoint: https://chapi.cloudhealthtech.com/v1/aws_accounts
content_markdown: |-
  The results of this API call are paginated.
parameters:
  - name: page
    content: Specify the page number for results
  - name: per_page
    content: Specify how many results should be displayed per page. Default value is 30.
right_code_blocks:
  - code_block: |-
      curl --request GET -H 'Content-Type: application/json' "https://chapi.cloudhealthtech.com/v1/aws_accounts?api_key=<your_api_key>"
    title: All results
    language: bash
  - code_block: |-
      curl --request GET -H 'Content-Type: application/json' "https://chapi.cloudhealthtech.com/v1/aws_accounts?api_key=<your_api_key>&page=2"
    title: Specific page
    language: bash
  - code_block: |-
      curl --request GET -H 'Content-Type: application/json' "https://chapi.cloudhealthtech.com/v1/aws_accounts?api_key=<your_api_key>&page=3&per_page=100"
    title: Results per page
    language: bash
---
