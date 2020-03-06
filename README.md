# Simple roslibpy Examples using Jupyter

Jupyter enabled Docker Image running python3 and roslibpy.

## Run the Examples

The Docker image can be built, run and pushed using repo2docker. This tool
generates an image from the source code repository.

### Install repo2docker

```zsh
python3 -m pip install jupyter-repo2docker
```

### Build and Run the Image

To run the image simply call

```zsh
jupyter-repo2docker .
```

### Adding dependencies

Additional Python libraries can be added to the `./environment.yml` file. These
libraries will be automatically installed in the environment using `conda`.
Example usage can be found here
[here](https://github.com/binder-examples/conda).

### Executing post-build Commands

Arbitrary commands can be executed after the build process by adding them to the
`postBuild` file, which will run from the shell.

