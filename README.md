## Generate sealed secrets using bitnami's seal secret controller

`cat secret.yaml | kubeseal --scope cluster-wide \
--controller-namespace sealed-secrets \
--controller-name sealed-secrets-controller \
--format yaml > sealed_secret.yaml
`