# dast-wf
A Dynamic Analysis workflow using OWASP Zap

The workflow uses official OWASP ZAP step with the add hoc needed parameters and configuration.

In essence the similar docker command would look like:
```bash
docker run --rm -v $(pwd):/zap/wrk/:rw -t owasp/zap2docker-stable zap-full-scan.py -t https://target.gr -g generic.conf -r target_report.html
```
