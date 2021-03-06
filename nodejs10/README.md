## node10-helper
This helper image is used for building and testing NodeJS applications.

It includes:
- [node 10.19.0](https://nodejs.org)

### Build
The build of the helper image itself is realized by Jenkins using this repository. During the build of the actual applications or service (realized outside this repo) this image will be used as a helper to compile and test the code. The helper is not supposed to be promoted to production deployments as such.

### Usage
The helper can be used calling the ```h_nodejs10``` the k8 agent. This can be configured by specifying the name at ```environments.<env>.agent.name```. Example:
```
environments.generic.agent.name: 's_mini+h_nodejs10'
```
