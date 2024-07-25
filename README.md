# Fuse

The ultimate AI assistant for Platform Engineers, crafted by the Botkube Team.

![Using fuse in CLI](docs/assets/prompt.gif)

## Installation

### macOS & Linux

Fuse is available via [Homebrew](https://brew.sh) and as a downloadable binary from the [releases page](https://github.com/kubeshop/fuse-releases/releases).

#### Homebrew

| Install                                    | Upgrade                                    |
|--------------------------------------------|--------------------------------------------|
| `brew install kubeshop/fuse-releases/fuse` | `brew upgrade kubeshop/fuse-releases/fuse` |


<details><summary><strong>Using <code>curl</code> on Linux</strong></summary>
<p>


Download the Fuse CLI binary and move it to a directory in your `$PATH`:

```shell
curl -Lo fuse https://github.com/kubeshop/fuse-releases/releases/latest/download/fuse-linux-amd64
chmod +x fuse && mv fuse /usr/local/bin/fuse
```

> [!NOTE]
> You may need to use sudo to run the mv command as it moves the binary file to the `/usr/local/bin/` directory.

</p>
</details> 

### Windows

Use [curl](https://curl.se/windows/) to download the Fuse CLI binary:

```shell
curl -Lo fuse https://github.com/kubeshop/fuse-releases/releases/latest/download/fuse-windows-amd64.exe
```

Move the binary to a directory in your `%PATH%`.

<details><summary><strong>Other Platforms</strong></summary>
<p>


Download the Fuse CLI binary and move it to a directory in your `$PATH`/`%PATH%`:

```shell
export OS=<your-os> # allowed values: darwin, linux, windows
export ARCH=<your-arch> # allowed values: amd64, arm64, armv7
export SUFFIX="" # set to ".exe" if OS is 'windows'
curl -Lo fuse https://github.com/kubeshop/fuse-releases/releases/latest/download/fuse-${OS}-${ARCH}${SUFFIX}
chmod +x fuse && mv fuse /usr/local/bin/fuse
```

</p>
</details> 

## Getting Started

After downloading the CLI, you can start experimenting right away:

```shell
fuse list my GKE instances and their status
```
