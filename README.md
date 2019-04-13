# rootless-jnlp-slave

This is an image based on [jenkins/jnlp-slave](https://hub.docker.com/r/jenkins/jnlp-slave/) running with non root user id.

This ensures that you can run a jnlp-slave based image in restricted environments, like Kubernetes where certain PodSecurityPolicies are activated for security reasons.
Specifically only allow the container to be run as [MustRunAsNonRoot](https://kubernetes.io/docs/concepts/policy/pod-security-policy/#users-and-groups)