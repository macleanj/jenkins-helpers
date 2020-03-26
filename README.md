# Overview
To support the building, compiling and testing process, the jenkins-builder can be assisted by specific code. Think of needing NodeJS or Maven as part of the build process. Instead of making one huge agent with all specific code included the pod containing the builder and agent can be supplemented with a helper.

Examples are:
- NodeJS0
- Clojure

See the specific documentation how to extend the agent with one or more helpers.