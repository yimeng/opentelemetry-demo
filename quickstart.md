kubectl apply --namespace otel-demo -f opentelemetry-demo.yaml
kubectl port-forward svc/opentelemetry-demo-frontendproxy --address 0.0.0.0 8080:8080 -n otel-demo
