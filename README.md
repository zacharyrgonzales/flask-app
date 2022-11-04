### Documentation

Built flask application and deployment yaml file for k8s using this article for reference - https://medium.com/featurepreneur/deploying-a-flask-app-to-kubernetes-f05c93866aff

Built ci/cd pipeline in github actions using this article for reference (note I did not build an eks cluster) - https://dev.to/leandronsp/deploy-to-kubernetes-using-github-actions-including-slack-notification-11je

Since I built the flask app from scratch there wasen't a lot of vulnerable code to improve so I focused on hardening the app against owasp top 10 by adding an sbom step, static and dynamic code analysis and secrets detection steps using owasp zap and trivy github actions - https://github.com/zaproxy/action-full-scan, https://github.com/aquasecurity/trivy-action