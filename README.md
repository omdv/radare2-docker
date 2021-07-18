This Docker image encapsulates the Radare2 reverse-engineering framework with ghidra decompiler plugin.

Replace `$(pwd)` with your directory
```
docker run --rm -it --cap-drop=ALL --cap-add=SYS_PTRACE -v $(pwd):/home/nonroot/workdir omdv/radare2
```
