https://sealos.io/zh-Hans/docs/lifecycle-management/quick-start/installation
sealos run labring/kubernetes:v1.25.0 labring/helm:v3.8.2 labring/calico:v3.24.1 --single
kubectl apply --namespace otel-demo -f opentelemetry-demo.yaml
kubectl port-forward svc/opentelemetry-demo-frontendproxy --address 0.0.0.0 8080:8080 -n otel-demo
