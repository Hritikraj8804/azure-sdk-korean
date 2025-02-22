# Azure SDK Contribution Guide (기여하기)

본 저장소는 [Microsoft Open Source Code of Conduct(Microsoft 오픈 소스 규정)](https://opensource.microsoft.com/codeofconduct/)를 준수합니다.
자세한 내용은 [준수 사항 FAQ(영문)](https://opensource.microsoft.com/codeofconduct/faq/)를 참조하세요.
또는 opencode@microsoft.com에 궁금한 사항을 문의하거나 의견을 제시하실 수 있습니다.

The Azure SDK project welcomes contributions and suggestions.  Most contributions require you to agree to a Contributor License Agreement (CLA) declaring that you have the right to, and actually do, grant us the rights to use your contribution. For details, visit https://cla.microsoft.com.

When you submit a pull request, a CLA-bot will automatically determine whether you need to provide a CLA and decorate the PR appropriately (e.g., label, comment). Simply follow the instructions provided by the bot. You will only need to do this once across all repos using our CLA.

## Azure SDK Korean GitHub Pages Site Contributions

Here's the general contribution process:

- Fork this Repository using the button at the top on right corner.
- Clone your forked repository to your pc ( git clone "url from clone option.)
- Create a new branch for your modifications (ie. `git branch new-user` and check it out `git checkout new-user` or simply do `git checkout -b new-user`)
- Add your files (`git add -A`), commit (`git commit -m "added myself"`) and push (`git push origin new-user`)
- Create a pull request
- Star this repository

##  Wait for Pull Request to merge

##  Celebrate - you've done your pull request!!

## Codespaces

Codespaces is new technology that allows you to use a container as your development environment. This repo provides a Codespaces container which is supported by both GitHub Codespaces and VS Code Codespaces.

### GitHub Codespaces

1. From the Azure SDK GitHub repo, click on the "Code -> Open with Codespaces" button.
1. Open a Terminal
1. Execute the following command and `Ctrl+Click` the link generated.  A new window will open with the Azure SDK website.

    ```bash
    bundle install
    bundle exec jekyll serve
    ```
Note: If you encounter a `Not Found` error while accessing the website, try adding `/azure-sdk-korean/` to the end of the URL.

### VS Code Codespaces

1. Install the [VS Code Remote Extension Pack](https://marketplace.visualstudio.com/items?itemName=ms-vscode-remote.vscode-remote-extensionpack)
1. When you open the Azure SDK repo in VS Code, it will prompt you to open the project in the Dev Container. If it does not prompt you, then hit `Ctrl+Shift+P`, and select "Remote-Containers: Open Folder in Container...". And you can create a Dev Container by using a container configuration template in Jekyll.
1. Open a Terminal
1. Press `Ctrl+Shift+T` or execute the following command and `Ctrl+Click` the link generated.  A new window will open with the Azure SDK website.

    ```bash
    bundle install
    bundle exec jekyll serve
    ```
Note: If you encounter a `Not Found` error while accessing the website, try adding `/azure-sdk-korean/` to the end of the URL.

## Full Local Setup

This site uses Jekyll and GitHub pages. Installation instructions can be found here: https://jekyllrb.com/docs/installation

Here's how to setup the site locally:

1. [Install Ruby+DevKit 2.6](https://rubyinstaller.org/downloads/) - Don't install 2.7, it doesn't work with this site.

    You can find complete installation instructions here: https://jekyllrb.com/docs/installation

1. Restart your machine

    You may need to restart your machine after installing Ruby.

1. Install Jekyll

    ```bash
    gem install jekyll bundler
    ```

1. Install Dependencies

    Run the following command from the root of the azure-sdk project.

    ```bash
    bundle install
    ```

1. Open a terminal and execute the following command to start the site:

    ```bash
    bundle exec jekyll serve
    ```

1. Open a browser to https://127.0.0.1:4000 to run the site.
