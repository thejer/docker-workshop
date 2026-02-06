(This README documents pipeline-specific utilities.)

If you don't have `uv` installed locally, there's a small Docker-backed wrapper in this directory.

- Make the wrapper executable and run it from this folder:

```bash
chmod +x ./uv
./uv --version
```

- To use `uv` as a regular command, add this folder to your `PATH` (optional):

```bash
export PATH="$PWD":$PATH
# then
uv --version
```

The wrapper runs the official `ghcr.io/astral-sh/uv:latest` image and forwards all arguments to the `uv` binary inside the container.

