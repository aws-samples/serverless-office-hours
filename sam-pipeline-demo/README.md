# ohdemo-app

SAM hello world application with Gitlab pipeline config. This application was created during demo: https://youtu.be/_1pD4aXV5sU

```
├── .aws-sam
│   └── pipeline
│       └── pipelineconfig.toml
├── .gitlab-ci.yml
├── assume-role.sh
├── hello-world
│   ├── app.js
│   ├── package.json
└── template.yaml
```

### Files explanation

`pipelineconfig.toml`: This file saves the information of bootstrapped resources which is later used to setup pipeline config.
`.gitlab-ci.yml`: Actual pipeline config for Gitlab.
`assume-role.sh`: Shell script which assumes PipelineExecutionRole in the account and provides temporary credentials for use during Gitlab execution.
`template.yaml`: Template file for the SAM application.

### How to use this package?

In order to use this package 

1. please update `pipelineconfig.toml` file with your resources ARNs.
2. Remove `.gitlab-ci.yml` file.
3. Run `sam pipeline init` command and select `Gitlab` from the options.

Another way is to follow this [demo](https://youtu.be/_1pD4aXV5sU) and that will create the `pipelineconfig.toml` and `.gitlab-ci.yml` file your application.
