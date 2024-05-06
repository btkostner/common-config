<h1 align="center">
  Common Config
</h1>

<p align="center">
  a framework for syncing multiple repositories with common configuration files
</p>

> [!NOTE]
> This project is still in the planning phase. If it sounds interesting to you, please [open a discussion](https://github.com/btkostner/common-config/discussions/new/choose) for features you want, and try using the original version of this project, [stordco/actions-sync](https://github.com/stordco/actions-sync)

Common config is a framework for scripting and templating files across multiple repositories. It's designed to run in a CI pipeline like GitHub actions, and open a PR with the changes. It has a number of features and advantages over other solutions:

- Run scripts in any language
- Template files with dynamic data
- Open a PR with the changes

## Differences

## GitHub repository templates

GitHub repository templates are great for starting a new project, however once you start managing multiple repositories, you'll notice it starts to break down.

1. It only templates files on initial repository creation. This means if you update the template, you have to take developer time to manually update all the repositories.

2. It does not allow for dynamic data. This means you can't template files with data from the repository, like the repository name, or anything else. This limits its usefulness.

## [Microplane](https://github.com/Clever/microplane)

Microplane is a great tool for running a script against multple repositories. Common config was built with Microplane in mind, but tries to make some things a bit easier for a larger team.

1. Common config templates are stored in a repository. This makes it easier to collaborate on the templates, and keeps everything in the open.

2. Common config is designed to be run in a CI pipeline. This means you don't need to setup a developer environment to run, and you can easily set it up to run on a schedule.

3. Templating is first class is common config. Technically you can do this with Microplane, but it's up to you to implement it.

## License

This project is licensed under the MIT license. See the [LICENSE](LICENSE) file for more info.
