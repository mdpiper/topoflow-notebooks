# topoflow-notebooks

Jupyter notebooks for diagnosing integration issues with TopoFlow.

## Usage

Login to ***beach***.
Change to the execution server directory
and add the execution server to your PATH.
```bash
cd /home/csdms/wmt/topoflow.1
PATH=$PWD/conda/bin:$PATH
```

Clone this repository and change to its top-level directory.
```bash
git clone https://github.com/mdpiper/topoflow-notebooks nb
cd nb
```

Start a Jupyter notebook, but don't open it in a browser.
```bash
jupyter notebook --no-browser
```
When the notebook starts, look at the port it's using.
It'll be something like `8888`.

On your local machine,
`ssh` into this port on ***beach***.
```bash
ssh -N -L 8888:localhost:8888 [username@]beach.colorado.edu
```

Go to [http://localhost:8888](http://localhost:8888).
