# github_action_trials


Features in GitHub to create custon Automated Workflows
- automate SDLC workflows
- implement CI CD DevOps


Demo 

- sign in to GH
- Create a repo
- In the repo create afolder .github/workflows folder
- In the folder create a YAML file with .yml extension
- Add the content of the workflow in the file
- commit and push the changes
- Go to Repo main page and click "Actions" tab
- Select the workflow from the left side logs and check the logs and results


Terms:
 workflow: collection of jobs, defined in a YAML file
 name:
 Events: any activity in the repo that can trigger a workflow 
 on: 
 Jobs: collection of steps
 jobs:
 Steps: actions to be taken, commands, scripts
 steps:
 Needs: Chaining the Jobs 
 needs


Features:
- Fully integrated with GH
- Respond to any GH event
- Community-powered workflows
- Any platform, any language, any cloud
- Linux, macOS, windows and containers
- Matrix builds
- Streaming, searchable, linkable logs
- Build-in secret store
- Easy to write, easy to share


Components of GH actions
        trigger         use
events ------> workflow ------> Actions

Events:
- GH triggered events: push, pull_request, public
- Scheduled events: schedule
- Manually triggered: workflow_dispatch(external systems)

Workflows:
- Workflows are like pipelines
- codify useful, customized processes
- .yaml syntax
- .github/workflows
- workflow files glue together existing actions in sequence
    - listen for particular events
    - then run pre-existing actions
    - or shell scripts
- Actions run in VMs (Linux, Win, Mac) Or Docker on Linux VM
- Logs streaming and artifacts
- Secret store with each repo or organization

Actions:
- Reusable units of code
- Referencing vs authoring actions
- Administrative features
- Storing shared Actions
- Post your actions to the GitHub Marketplace

- Monolithic action:
    - check out the code
    - Build and test
    - Release

- Chainable action:
    - create draft release
    - generate release notes
    - edit release, add notes
