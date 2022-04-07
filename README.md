This project provides a Spack cache (source and binary) for bootstrapping on systems without network
access. 

Instructions
------------

1. Place this directory on the desired system.
2. `cd ${SPACK_ROOT}`  Switch directories to your Spack root directory
3. `mkdir share/spack/bootstrap/local`
4. `cp share/spack/bootstrap/github-actions/clingo.json share/spack/bootstrap/local/`
5. Copy the bootstrap.yaml file from this repo to `etc/spack/bootstrap.yaml`
6. Edit `etc/spack/bootstrap.yaml` such that the 'url' line is the local path to this repo.
7. Run `spack spec freetype` to test.
