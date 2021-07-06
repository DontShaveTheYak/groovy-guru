# Groovy IntelliSense for Visual Studio Code

A WIP extension for [Visual Studio Code](https://code.visualstudio.com/) based on the [Groovy Language Server](https://github.com/prominic/groovy-language-server).

## Install

### Latest prebuilt extension

```sh
curl -s https://api.github.com/repos/DontShaveTheYak/groovy-guru/releases/latest \
| grep "browser_download_url.*vsix" \
| cut -d : -f 2,3 \
| tr -d \" \
| wget -qi -

code --install-extension groovy-guru-*.vsix
```

To install a specfic version, download the `vsix` file from the [releases](https://github.com/DontShaveTheYak/groovy-guru/releases) page.

### Build from source

To build from the command line, run the following command:

```sh
./gradlew build -Pversion=${VERSION}
```

You need to pass in a valid version so the client can download the server from the releases page.

The extension will be created in the `./build` folder.

## Acknowledgements
* [Groovy Language Server](https://github.com/prominic/groovy-language-server)
* [Moonshine IDE](https://moonshine-ide.com)
<!-- * [Best-README-Template](https://github.com/othneildrew/Best-README-Template) -->
