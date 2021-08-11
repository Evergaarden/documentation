#Чеклист проверок мобильного приложения


| Check name | Short Description  | Level C | Level B | Level A |
| :--------- | :----------------- | :------ | :------ | :------ |
| Unit test | It has unit tests. And the unit tests are running in a CI system. | :white_check_mark: | :white_check_mark: | :white_check_mark: |
| High Test coverage | Its test coverage is over 80%. |  | :white_check_mark: | :white_check_mark: |
| [Config in env-var](https://12factor.net/config) | Its config can be overridden via environment variable.  |  | :white_check_mark: | :white_check_mark: |
| [dockerignore](https://docs.docker.com/engine/reference/builder/#dockerignore-file) | It has dockerignore to reduce the Docker image size. |  | :white_check_mark: | :white_check_mark: |
| [No latest tag](https://twitter.com/thockin/status/1085223284122087424) | Its Docker image tag is not `latest` or `master`. |  | :white_check_mark: | :white_check_mark: |
| [Dependabot](https://dependabot.com/) | Its dependencies are automatically updated. |  | :white_check_mark: | :white_check_mark: |
| [Automated build](../concepts/automated-build.md) | Its build process is automated (binary build and Docker image build is in this scope). | :white_check_mark: | :white_check_mark: | :white_check_mark: |
| [Automatic build](../concepts/automatic-build.md) | Its automated build process is running in CI/CD system. |  |  | :white_check_mark: |
| Automated deploy | Its deploy process is automated. | :white_check_mark: | :white_check_mark: | :white_check_mark: |
| Automatic deploy | Its automated deploy process is running in CI/CD system. |  | :white_check_mark: | :white_check_mark: |
| [Gradual deploy](../concepts/gradual-deploy.md) | Its deploy can be gradual if you want. |  |  | :white_check_mark: |
| [Automated rollback](../concepts/automated-rollback.md) | Its rollback process is automated. |  | :white_check_mark: | :white_check_mark: |

## :chart_with_downwards_trend: Observability
Observability affects team productivity and system availability. If observability is low, the team will take a longer time to notice/investigate a problem occurred in production. And it will make MTTR (Mean Time To Recover) longer.