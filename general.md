# Conda

### Install conda:

```bash
wget https://repo.continuum.io/miniconda/Miniconda3-latest-Linux-x86_64.sh -O ${HOME}/miniconda.sh
bash ${HOME}/miniconda.sh -b -p ${HOME}/miniconda
rm ${HOME}/miniconda.sh

export PATH=${HOME}/miniconda/bin:$PATH
```
### Use conda
Create new environment
```bash
conda -c environment_name
```

Create new environment with specific python version
```bash
conda -c environment_name python=3.6 -y
```

Create new environment and install packages
```bash
conda -c environment_name package1 package2
```

Create environment from file
```bash
conda env create -f env.yml
```

List pakcages in environments
```bash
conda list -n environment_name

# Or if the environment is active:
conda list
```

List existing environments
```bash
conda info --envs
```



