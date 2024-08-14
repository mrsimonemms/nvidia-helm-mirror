# nvidia-helm-mirror

Mirror for the NVIDIA Helm charts

<!-- toc -->

* [Getting started](#getting-started)
* [Contributing](#contributing)
  * [Open in a container](#open-in-a-container)

<!-- Regenerate with "pre-commit run -a markdown-toc" -->

<!-- tocstop -->

## Getting started

This acts as a mirror to the NVIDIA Helm chart. Please see
[the docs](https://docs.nvidia.com/datacenter/cloud-native/gpu-operator/latest/getting-started.html)
for installation and usage instructions.

1. Add the NVIDIA mirror Helm repository:

   ```shell
   helm repo add nvidia-mirror https://mrsimonemms.github.io/nvidia-helm-mirror \
       && helm repo update
   ```

1. Install the GPU operator

   ```shell
   helm install --wait --generate-name \
     -n gpu-operator --create-namespace \
     nvidia-mirror/gpu-operator
   ```

## Contributing

### Open in a container

* [Open in a container](https://code.visualstudio.com/docs/devcontainers/containers)
