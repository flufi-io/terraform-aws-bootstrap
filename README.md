# terraform-aws-bootstrap


# terraform-module-template
A terraform module will have:
- [ ] default branch protection
  - [ ] checks
    - [ ] terratest
    - [ ] tfsec
    - [ ] dependabot
    - [ ] terraform-docs
    - [ ] atlantis
    - [ ] terraform format
  - [ ] require signed commits
- [ ] config files
  - [ ] .gitignore
  - [ ] .terraform-docs.yml
  - [ ] CODEOWNERS
  - [ ] PULL_REQUEST_TEMPLATE.md
- [ ] credentials and secrets
  - [ ] OIDC between a sandbox AWS Account and GitHub
  - [ ] SOPS for secrets
- [ ] terraform files
  - [ ] main.tf
  - [ ] variables.tf
  - [ ] outputs.tf
  - [ ] versions.tf
- [ ] examples
- [ ] tests
- [ ] README.md
  - [ ] Usage
  - [ ] terraform-docs
  - [ ] How to
    - [ ] test
    - [ ] terraform-docs
    - [ ] Add a module to the Terraform Registry
    - [ ] Import existing resources.