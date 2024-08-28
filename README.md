# "Exfil with Curl" Action for Offensive Security Workflows

A reusable Github action intended to be used in red teaming and security assessments of CI/CD pipelines. This action uses the `curl` binary to `POST` the provided data to a specified endpoint.

Part of the RascalRunner family of Github offensive security tools.

## Inputs

- `inputs.url` - a fully qualified url to send the `POST` payload to
- `inputs.data` - data to be sent to `inputs.url`, will be base64'ed prior to sending to fix issues with whitespace and newlines
