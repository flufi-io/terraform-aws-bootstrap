# terraform-aws-bootstrap


## terraform-module-template
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
  - [ ] include administrators
- [ ] config files
  - [ ] .gitignore
  - [ ] .terraform-docs.yml
  - [ ] CODEOWNERS
  - [ ] PULL_REQUEST_TEMPLATE.md
  - [ ] GitHub Actions
    - [ ] tfsec.yml
    - [ ] terraform-docs.yml
    - [ ] terratest.yml
    - [ ] atlantis.yml
    - [ ] terraform-fmt.yml
- [ ] credentials and secrets
  - [ ] OIDC between a sandbox AWS Account and GitHub
  - [ ] SOPS for secrets
- [ ] default terraform files
  - [ ] main.tf
  - [ ] variables.tf
  - [ ] outputs.tf
  - [ ] versions.tf
- [ ] examples
  - [ ] complete
    - [ ] main.tf
    - [ ] variables.tf
    - [ ] outputs.tf
    - [ ] versions.tf
- [ ] tests
  - [ ] complete
- [ ] README.md
  - [ ] Usage
  - [ ] How to
    - [ ] test
    - [ ] terraform-docs
    - [ ] Add a module to the Terraform Registry
    - [ ] Import existing resources.
  - [ ] terraform-docs
  - [ ] License

Considerations
* All the files will be managed by
terraform with github_repository_file
* The template will be versioned
* All the secrets or sensitive values must be encrypted with SOPS

## terraform-aws-account(DRAFT)
- [ ] default accounts

  - [ ] root, it will not be used for any purpose
  - [ ] master, will manage the AWS Organization
  - [ ] billing
  - [ ] dev
  - [ ] prod, at least one
  - [ ] sandbox (it will be used with terratest)
  - [ ] backups (must have a restricted access)