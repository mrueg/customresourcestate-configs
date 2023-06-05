# customresourcestate-configs

Custom resource state configurations for [kube-state-metrics](https://github.com/kubernetes/kube-state-metrics)

[[_TOC_]]

## OpenPolicyAgent Gatekeeper

Generates metric series based on the status of Constraint objects exposing the following information:

* kube_customresource_gatekeeper_violations_total

Number of total violations against a constraint

* kube_customresource_gatekeeper_violation_info

Info about individual violation per constraint

## Cert-Manager

Generates metric series per Certificate:

* kube_customresource_certificate_valid_not_before

Before this timestamp the certificate is not valid.

* kube_customresource_certificate_valid_not_after

After this timestamp the certificate is not valid anymore.

* kube_customresource_certificate_transition_info

Generates one metric series per Issuer:

* kube_customresource_issuer_transition_info

Shows transition state of the Issuer object

