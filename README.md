# dvc-cc-test## About DVC-CC
This branch was automated created with the tool DVC-CC. This tool connects DVC (https://dvc.org/) to CC (www.curious-containers.cc) to run your defined stages with DVC in a docker on your cloud system with CC. [More information about DVC-CC](https://github.com/deep-projects/dvc-cc)

## DVC-Status


<details><summary>Before Execution</summary>
<p>

```
WARNING: Output 'tensorboard'(Stage: 'dvc/train.dvc') is missing version info. Cache for it will not be collected. Use dvc repro to get your pipeline up to date.
WARNING: Output 'model.h5'(Stage: 'dvc/train.dvc') is missing version info. Cache for it will not be collected. Use dvc repro to get your pipeline up to date.
WARNING: Output 'summary.yml'(Stage: 'dvc/train.dvc') is missing version info. Cache for it will not be collected. Use dvc repro to get your pipeline up to date.
Data and pipelines are up to date.

```

</p>
</details>




<details><summary>After Execution</summary>
<p>

```
	new:                tensorboard
	new:                tensorboard/train/events.out.tfevents.1570443630.pepper01.334.272.v2
	new:                tensorboard/train/events.out.tfevents.1570443631.pepper01.profile-empty
	new:                tensorboard/train/plugins/profile/2019-10-07_10-20-31/local.trace
	new:                tensorboard/validation/events.out.tfevents.1570443631.pepper01.334.1073.v2
	new:                model.h5
	new:                summary.yml

```

</p>
</details>



## How to rerun this experiment:
The following sections describe how you can rerun the dvc stages yourself.
### Pure command line (run the experiment local)
```
python source/train.py --num_of_kernels 5 --activation_function relu

```
### Using DVC (run the experiment local)
```
dvc repro -P
```
### Using CC (run the experiment on a server)
```
faice exec cc_execution_file.red.yml
```
## Executed System
The scipt ran on the following system:


<details><summary>GPU(s)</summary>
<p>

```
                          name    memory.total [MiB]
====================================================
          Tesla V100-PCIE-16GB             16130 MiB

```

</p>
</details>




<details><summary>Other Hardware</summary>
<p>

```
H/W path         Device   Class          Description
====================================================
/0/0                      memory         754GiB System memory
/0/1                      processor      Intel(R) Xeon(R) Gold 6130 CPU @ 2.10GHz
/0/2                      processor      Intel(R) Xeon(R) Gold 6130 CPU @ 2.10GHz
/0/100/1f.2               memory         Memory controller

```

</p>
</details>




<details><summary>Software</summary>
<p>

```
Package              Version      
-------------------- -------------
absl-py              0.8.0        
appdirs              1.4.3        
asciimatics          1.11.0       
asn1crypto           0.24.0       
astor                0.8.0        
atpublic             1.0          
attrs                19.2.0       
backcall             0.1.0        
bcrypt               3.1.7        
bleach               3.1.0        
certifi              2019.9.11    
cffi                 1.12.3       
chardet              3.0.4        
colorama             0.4.1        
configobj            5.0.6        
configparser         4.0.2        
contextlib2          0.5.5        
cryptography         2.7          
cycler               0.10.0       
decorator            4.4.0        
defusedxml           0.6.0        
distro               1.4.0        
dvc                  0.60.1+ee976a
dvc-cc-agent         0.8.8        
dvc-cc-connector     0.8.1        
entrypoints          0.3          
flufl.lock           3.2          
funcy                1.13         
future               0.17.1       
gast                 0.2.2        
gitdb2               2.0.6        
GitPython            3.0.2        
google-pasta         0.1.7        
grandalf             0.6          
grpcio               1.24.0       
h5py                 2.10.0       
humanize             0.5.1        
idna                 2.6          
inflect              2.1.0        
ipykernel            5.1.2        
ipython              7.8.0        
ipython-genutils     0.2.0        
ipywidgets           7.5.1        
jedi                 0.15.1       
Jinja2               2.10.1       
joblib               0.14.0       
jsonpath-ng          1.4.3        
jsonschema           3.0.2        
jupyter              1.0.0        
jupyter-client       5.3.3        
jupyter-console      6.0.0        
jupyter-core         4.5.0        
Keras-Applications   1.0.8        
Keras-Preprocessing  1.1.0        
keyring              10.6.0       
keyrings.alt         3.0          
kiwisolver           1.1.0        
Markdown             3.1.1        
MarkupSafe           1.1.1        
matplotlib           3.1.1        
mistune              0.8.4        
mock                 3.0.5        
nanotime             0.5.2        
nbconvert            5.6.0        
nbformat             4.4.0        
networkx             2.3          
notebook             6.0.1        
numpy                1.17.2       
opt-einsum           3.1.0        
packaging            19.2         
pandas               0.25.1       
pandocfilters        1.4.2        
paramiko             2.6.0        
parso                0.5.1        
pathspec             0.5.9        
pexpect              4.7.0        
pickleshare          0.7.5        
Pillow               6.2.0        
pip                  19.2.3       
ply                  3.11         
prometheus-client    0.7.1        
prompt-toolkit       2.0.9        
protobuf             3.9.2        
ptyprocess           0.6.0        
pyasn1               0.4.7        
pycparser            2.19         
pycrypto             2.6.1        
pyfiglet             0.8.post1    
Pygments             2.4.2        
pygobject            3.26.1       
pyjson               1.3.0        
PyNaCl               1.3.0        
pyparsing            2.4.2        
pyrsistent           0.15.4       
python-dateutil      2.8.0        
pytz                 2019.2       
pyxdg                0.25         
PyYAML               5.1.2        
pyzmq                18.1.0       
qtconsole            4.5.5        
red-connector-ssh    1.0          
requests             2.22.0       
ruamel.yaml          0.16.5       
ruamel.yaml.clib     0.2.0        
schema               0.7.1        
scikit-learn         0.21.3       
scipy                1.3.1        
scp                  0.13.2       
seaborn              0.9.0        
SecretStorage        2.3.1        
Send2Trash           1.5.0        
setuptools           41.2.0       
shortuuid            0.5.0        
six                  1.11.0       
sklearn              0.0          
smmap2               2.0.5        
tensorboard          2.0.0        
tensorflow-estimator 2.0.0        
tensorflow-gpu       2.0.0        
termcolor            1.1.0        
terminado            0.8.2        
testpath             0.4.2        
torch                1.2.0        
torchvision          0.4.0        
tornado              6.0.3        
tqdm                 4.36.1       
traitlets            4.3.2        
treelib              1.5.5        
urllib3              1.25.6       
wcwidth              0.1.7        
webencodings         0.5.1        
Werkzeug             0.16.0       
wheel                0.30.0       
widgetsnbextension   3.5.1        
wrapt                1.11.2       

```

</p>
</details>


