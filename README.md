# wealth-wise

## A smart personal finance platform that tracks expenses, automates budgeting, and provides real-time insights, using a cloud-native, full-stack microservices architecture.

apps/
│
├── backend-api/
│   ├── user-service/ (Spring Boot)
│   ├── transaction-service/ (Spring Boot)
│   |── report-service/ (Spring Boot + Mongo)
│   
│
├── budget-service/ (Next.js API)
├── notification-service/ (Node.js + Redis/Firebase)

com.wealthwise.user
├── controller
├── service
├── repository
├── model
├── config
└── dto

wealthwise/
│
├── apps/
│   ├── web-frontend/                # React.js web app
│   │   ├── public/
│   │   ├── src/
│   │   ├── package.json
│   │   └── README.md
│   │
│   ├── mobile-app/                  # React Native app
│   │   ├── src/
│   │   ├── assets/
│   │   ├── package.json
│   │   └── README.md
│   │
│   ├── backend-api/                 # Spring Boot main backend
│   │   ├── src/
│   │   ├── pom.xml
│   │   ├── Dockerfile
│   │   └── README.md
│   │
│   ├── budget-service/              # Node.js microservice (e.g., budgeting)
│   │   ├── src/
│   │   ├── package.json
│   │   ├── Dockerfile
│   │   └── README.md
│
├── libs/                            # Shared libs/types/components (optional)
│   ├── ui-components/
│   ├── api-types/
│   └── README.md
│
├── deploy/
│   ├── kubernetes/                  # K8s manifests/Helm charts
│   │   ├── backend-api-deployment.yaml
│   │   ├── budget-service-deployment.yaml
│   │   ├── web-frontend-deployment.yaml
│   │   ├── mobile-app-deployment.yaml
│   │   ├── postgres-statefulset.yaml
│   │   ├── mongodb-deployment.yaml
│   │   ├── ingress.yaml
│   │   └── README.md
│   ├── docker/                      # Extra Docker compose files if needed
│   │   └── docker-compose.dev.yml
│   ├── scripts/
│   │   └── db-migrate.sh
│   └── README.md
│
├── docs/
│   ├── architecture/
│   │   └── high-level-design.md
│   ├── api/
│   │   ├── openapi.yaml
│   │   └── budget-service-swagger.yaml
│   ├── user-guides/
│   │   └── getting-started.md
│   └── README.md
│
├── .github/
│   ├── workflows/
│   │   ├── ci-dev.yml
│   │   ├── cd-prod.yml
│   │   └── codeql.yml
│   └── ISSUE_TEMPLATE/
│       ├── bug_report.md
│       └── feature_request.md
│
├── .env.example
├── .gitignore
├── README.md
├── LICENSE
└── CONTRIBUTING.md