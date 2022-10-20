1. Create Dockerfile for express-app (use `yarn` instead of `npm`)
2. Create Helm chart for express-app (in charts folder)
  - Resctrict access for your app with provied ip list 
  ```bash
  46.199.32.134
  46.199.32.135
  46.199.32.136
  ```
  - pass `TEST_VAR` environment variable trought helm chart and check its value `GET /envVars`
3. Create github actions pipeline with specified stages (bellow is a list with requered stages, but you can add something else):
``` 
  - Build
  - Test
  - Deploy
```

When task is done - open PR.