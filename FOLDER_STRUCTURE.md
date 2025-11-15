# FOLDER_STRUCTURE.md
### Project Folder Architecture

Below is the recommended structure for the AI-Resilience-Orchestrator repository.

```
AI-Resilience-Orchestrator/
│
├── agents/
│   ├── detection/
│   │   └── detector.py
│   ├── controller/
│   │   └── ai_controller.py
│   └── deployment/
│       └── deployer.py
│
├── core/
│   ├── events/
│   ├── interfaces/
│   └── utils/
│
├── simulations/
│   ├── docker/
│   │   └── docker-compose.yml
│   └── kubernetes/
│       └── manifests/
│
├── tests/
│   ├── unit/
│   └── integration/
│
├── docs/
│   ├── images/
│   └── diagrams/
│
├── examples/
│   └── sample-failure-events.json
│
├── README.md
├── ARCHITECTURE.md
├── CONTRIBUTING.md
├── CODE_OF_CONDUCT.md
├── ROADMAP.md
├── SETUP.md
└── requirements.txt
```

### Notes:
- `agents/` contains the 3 brains of the system.  
- `core/` contains utilities shared by agents.  
- `simulations/` contains Docker + K8s testing environments.  
- `tests/` holds automated test suites.  
- `docs/` stores diagrams, images, and documentation assets.

This structure keeps the project modular, clean, and scalable.
