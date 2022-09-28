# K8_Test

ku create deploy testing01 --image sreehatsha:rollingupdate:v1  --replicas 3 --dry-run -o yaml

ku expose deployment --name service-np testing01 --port=8080 --target-port=80 --type=NodePort -o yaml --dry-run
