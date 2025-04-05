# monorepo-template
## Explained
```
/
├── apps/
│   └── <app-name>/
│       ├── compose.yaml        # docker/podman compose file for local deployment
│       ├── helm                # helm chart for app
│       ├── init                # init container source code
│       ├── integration-test    # integration test source code
│       ├── src                 # actual app source code
│       └── test                # unit test source code
│
├── environments/               # defined environments (for helmfile)
│   ├── global.yaml             # shared fields
│   ├── dev.yaml                
│   └── prod.yaml              
│ 
├── infrastructure/             # infrastructure as code
├── proto/                      # protobuf definitions
├── hack/                       # scripts, etc...
│
├── helmfile.yaml               # deployment configuration
├── buf.gen.yaml                # buf (see https://buf.build/docs/cli/) configuration
├── LICENSE
└── README.md
```