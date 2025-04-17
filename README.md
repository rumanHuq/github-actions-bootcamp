## Instructions
You will need Github personal access token(classic) with workflow enabled from [here](https://github.com/settings/tokens)

```sh
# Demo Curl command to invoke the webhook
curl -X POST https://api.github.com/repos/rumanHuq/github-actions-bootcamp/dispatches \
  -H "Accept: application/vnd.github+json" \
  -H "Authorization: Bearer <YOUR_TOKEN>" \
  -d '{"event_type": "webhook", "client_payload": {"deployment_target": "prod"}}'
```
