# singularity-docker-fedora27-buildenv-singularity-git-release-2.4
fedora27 build env for singularity/git-release-2.4

example Dockerfile provided for convenience.

Running without installation:
```
export OUT=`mktemp -d` && echo building in ${OUT} && \
singularity run -H ${OUT}  shub://truatpasteurdotfr/singularity-docker-fedora27-buildenv-singularity-git-release-2.4
```
Building:
```
sudo singularity build singularity-docker-fedora27-buildenv-singularity-git-release-2.4.simg  Singularity
```
Download and rename:
```
singularity pull --name "singularity-docker-fedora27-buildenv-singularity-git-release-2.4" shub://truatpasteurdotfr/singularity-docker-fedora27-buildenv-singularity-git-release-2.4
```
Running with a separate $HOME 
```
mkdir -p  ~/singularity.d/home/singularity-docker-fedora27-buildenv-singularity-git-release-2.4
singularity run -H  ~/singularity.d/home/singularity-docker-fedora27-buildenv-singularity-git-release-2.4 singularity-docker-fedora27-buildenv-singularity-git-release-2.4.simg
```
