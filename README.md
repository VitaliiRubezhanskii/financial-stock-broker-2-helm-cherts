1. Add repository `helm repo add financial-stock-broker-2 https://vitaliirubezhanskii.github.io/financial-stock-broker-2-helm-charts`
2. Package chart for each service: `helm package charts/accout`, `helm package charts/analytics`, `helm package charts/order`, `helm package charts/quotes-provider`, `helm package charts/api-gateway`
3.  helm install <service-name> https://vitaliirubezhanskii.github.io/financial-stock-broker-2-helm-charts/<service-name>-0.3.5.tgz -n kafka 