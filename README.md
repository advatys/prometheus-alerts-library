# prometheus-alerts-library
This repo contains prometheus-rule manifest to fire alerts for CPU and RAM usage by all pods.

Please define values of labels in values.yaml
And the add the same lables in your prometheus instance in field ruleSelector.matchLabels  to mount these rules. 

Eg;

 ruleSelector:
    matchLabels:
      role: alert-rules
      prometheus: example

Reference: https://github.com/prometheus-operator/prometheus-operator/blob/master/Documentation/user-guides/alerting.md#fire-alerts