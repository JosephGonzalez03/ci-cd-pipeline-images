# ci-cd-pipeline-images
This repo contains image for my local ci/cd pipeline. The pipeline serves as a practice exercise to
better understand cd/ci design, and as a means for maintaining my own REST APIs.

### Git Repo Branches
The following are the branches present in each REST API repo: 
* feature/*
* development
* release
* main

### Features
Feature branches are created to introduce new features or to refactor exiting features.
Feature branches must implement the agreed upon feature and have passing unit
tests which prove its functionality. The functionality of other features must not be 
affected, or those features' unit tests must also be updated to reflect any changes. If 
and only if these requirements are met shall a feature branch be merged into the 
development branch.

### Development
The development branch is where new features are further integrated with the existing code 
base. At this stage, the API's documentation and schema are updated to reflect the changes
introduced by the new feature. Contract tests are also written to validate the API's schema.
The documentation must be validated against the schema and contract tests must be run with
mocked endpoints in the case of web provider and test data in the case of database provider.

### Release
