# release-note
helm chart for urnr - release note share system

우리누리 릴리즈노트 공유 시스템의 helm 차트입니다.
아키텍쳐를 위한 의존성으로 아래의 다른 차트들이 포함되어 있습니다.

### DB
mysql-operator
https://mysql.github.io/mysql-operator

mysql-innodbcluster
https://mysql.github.io/mysql-operator

### Monitoring
kube-prometheus-stack
https://prometheus-community.github.io/helm-charts
    
### Logging
fluent-bit
https://fluent.github.io/helm-charts

opensearch
https://opensearch-project.github.io/helm-charts

opensearch-dashboards
https://opensearch-project.github.io/helm-charts

### MQ
 kafka
 https://charts.bitnami.com/bitnami

 ### In-memory DB
redis-cluster
https://charts.bitnami.com/bitnami

### CD
argo-cd
https://argoproj.github.io/argo-helm

기본적으로 실행하기 위한 SC, PV, PVC가 포함되어 있으며, LoadBanlancer 타입의 서비스로 프론트엔드와 백엔드를 연결합니다.
모니터링을 위한 서비스 모니터와 관련 파드 설정이 되어있습니다.

