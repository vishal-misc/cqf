# India Quants, Python Installaion Using Docker by Kannan Singaravelu
# For implementation, refer to the installation video

## Installation 
step 1: create directory in your project directory and cd into it 
        `mkdir pythonlab && cd pythonlab`
step 2: save the requirments file on this folder
step 3: run ubuntu container 
        install Docker Desktop from https://www.docker.com/get-started
        `docker run -d --name pythonlab -it -p 2305:2305 -h ksingara -v $(pwd):/root/pythonlab ubuntu:latest /bin/bash`
step 4: to interact and execute with already running container
        `docker exec -it pythonlab bash`
step 5: update package index files on the system
        `apt update -y`
step 6: upgrade packages
        `apt upgrade -y`
step 7: install command line tool
        `apt install wget`
step 8: install miniconda (for linux)
        `wget https://repo.anaconda.com/miniconda/Miniconda3-latest-Linux-x86_64.sh`
        `bash Miniconda3-latest-Linux-x86_64.sh`
        remove miniconda installation file to save space
        `rm Miniconda3-latest-Linux-x86_64.sh`
step 9: refresh the terminal 
        `bash`
step 10: install libraries 
        `pip install -r requirements.txt`
step 11: run jupyter lab [set ip to allow all ports]
        `jupyter lab --allow-root --port 2305 --ip 0.0.0.0`


## Datasets
a. download csv files from https://github.com/kannansingaravelu/datasets

## References
a. https://github.com/kannansingaravelu/datasets
b. https://www.docker.com/get-started/
c. https://stackoverflow.com
d. https://docs.python.org/3.6

## Most Popular Bootcamps
a. Algorithmic Trading - Part1		                
b. Algorithmic Trading - Part2
c. Advanced Machine Learning - Part1
d. Advanced Machine Learning - Part2
e. R for Quant Finance & Machine Learning
f. Decentralized Finance Technologies 
g. Advanced Ensemble Modeling

