# cert-manager

This README documents the cert-manager integration as Nirmata add-on on Kubernetes clusters.

### What is the cert-manager?

Cert-manager is a native Kubernetes certificate management controller. It can help with issuing certificates from a variety of sources, such as Let's Encrypt, HashiCorp Vault, Venafi, a simple signing key pair, or self-signed. It will ensure certificates are valid and up to date, and attempt to renew certificates at a configured time before expiry.



### How do I get set up?
1. Clone this repository or add its contents to your own private Git repository.
2. Create a Nirmata catalog application with a Git upstream and select the cert-manager repository. You can optionally select the kustomization.
3. Edit the catalog application and select an add-on category (e.g. Security). This is required to select the application as an add-on.
4. Update a Cluster Type, or create a new one, and select the cert-manager add-on application in the "Add-Ons" section. Ensure that the namespace you use is "**cert-manager**" and environment is "cert-manager -< cluster-name >"
5. Create clusters using the cluster type.
6. If the addon is to be added to a running cluster, create an environment with the namespace "**cert-manager**" and choose this environment while deploying the application
7. Verify that the application is running in Nirmata. 

### Who do I talk to?
For issues, contact support@nirmata.com
