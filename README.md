This Docker image encapsulates the Radare2 reverse-engineering framework with ghidra decompiler plugin.

To run this image after installing Docker, use a command like this, replacing "~/workdir" with the path to your working directory on the underlying host:

docker run --rm -it --cap-drop=ALL --cap-add=SYS_PTRACE -v ~workdir:/home/nonroot/workdir omdv/radare2

Then run r2 or other Radare2 commands inside the container. Before running the application, create ~/workdir on your host.

This Dockerfile is based on the instructions documented in the official Radare2 Dockerfile file.

