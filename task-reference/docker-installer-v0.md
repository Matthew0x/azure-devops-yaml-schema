---
title: DockerInstaller@0 - Docker CLI installer v0 task
description: Install Docker CLI on agent machine.
ms.date: 08/10/2022
monikerRange: ">=azure-pipelines-2019.1"
---

# DockerInstaller@0 - Docker CLI installer v0 task

<!-- :::description::: -->
:::moniker range=">=azure-pipelines-2019.1"

<!-- :::editable-content name="description"::: -->
Install Docker CLI on agent machine.
<!-- :::editable-content-end::: -->

:::moniker-end
<!-- :::description-end::: -->

<!-- :::syntax::: -->
## Syntax

:::moniker range=">=azure-pipelines-2019.1"

```yaml
# Docker CLI installer v0
# Install Docker CLI on agent machine.
- task: DockerInstaller@0
  inputs:
    dockerVersion: '17.09.0-ce' # string. Required. Docker Version. Default: '17.09.0-ce'.
    #releaseType: 'stable' # 'stable' | 'edge' | 'test' | 'nightly'. Release type. Default: 'stable'.
```

:::moniker-end
<!-- :::syntax-end::: -->

<!-- :::inputs::: -->
## Inputs

<!-- :::item name="dockerVersion"::: -->
:::moniker range=">=azure-pipelines-2019.1"

**`dockerVersion`** - **Docker Version**<br>
Type: string. Required. Default value: '17.09.0-ce'.<br>
<!-- :::editable-content name="helpMarkDown"::: -->
Specify the version of Docker CLI to install.
<!-- :::editable-content-end::: -->

:::moniker-end
<!-- :::item-end::: -->
<!-- :::item name="releaseType"::: -->
:::moniker range=">=azure-pipelines-2019.1"

**`releaseType`** - **Release type**<br>
Type: string. Allowed values: 'stable', 'edge', 'test', 'nightly'. Default value: 'stable'.<br>
<!-- :::editable-content name="helpMarkDown"::: -->
Pick the release type to install. Nightly is not supported on Windows.
<!-- :::editable-content-end::: -->

:::moniker-end
<!-- :::item-end::: -->
<!-- :::inputs-end::: -->

<!-- :::outputVariables::: -->
## Output variables

:::moniker range=">=azure-pipelines-2019.1"

None.

:::moniker-end
<!-- :::outputVariables-end::: -->

<!-- :::remarks::: -->
<!-- :::editable-content name="remarks"::: -->
<!-- :::editable-content-end::: -->
<!-- :::remarks-end::: -->

<!-- :::examples::: -->
<!-- :::editable-content name="examples"::: -->
<!-- :::editable-content-end::: -->
<!-- :::examples-end::: -->

<!-- :::properties::: -->
## Requirements

:::moniker range=">=azure-pipelines-2019.1"

| Requirement | Description |
|-------------|-------------|
| Pipeline types | YAML, Classic build, Classic release |
| Runs on | Agent, DeploymentGroup |
| [Demands](/azure/devops/pipelines/process/demands) | None |
| [Capabilities](/azure/devops/pipelines/agents/agents#capabilities) | Running this task satisfies the following [demands](/azure/devops/pipelines/process/demands) for any subsequent tasks in the same job: Docker |
| [Command restrictions](/azure/devops/pipelines/security/templates#agent-logging-command-restrictions) | Any |
| [Settable variables](/azure/devops/pipelines/security/templates#agent-logging-command-restrictions) | Any |
| Agent version |  2.142.1 or greater |
| Task category | Tool |

:::moniker-end
<!-- :::properties-end::: -->

<!-- :::see-also::: -->
<!-- :::editable-content name="seeAlso"::: -->
<!-- :::editable-content-end::: -->
<!-- :::see-also-end::: -->