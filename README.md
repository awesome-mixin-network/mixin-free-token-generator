# mixin-free-token-generator
![cover](https://github.com/wenewzhang/mixin_labs-python-bot/raw/master/Bitcoin_python.jpg)
A python flask code to generate auth_token for creating mixin network account for free and secure

Full Mixin network resource [index](https://github.com/awesome-mixin-network/index_of_Mixin_Network_resource)

## Python 3 installation:
This tool is written in Python 3.7.2 So you need to install Python 3.7.2 or above.

macOS
```bash
brew upgrade
brew install python@3
```

Ubuntu, install python 3.7.2 from the third apt source.
```bash
sudo apt update
sudo apt install software-properties-common
sudo add-apt-repository ppa:deadsnakes/ppa
```

When prompt like below, press Enter to continue:
```bash
Press [ENTER] to continue or Ctrl-c to cancel adding it.
```
Update the source, then install python3.7, python3.7-venv
```bash
sudo apt update
sudo apt install python3.7 python3.7-venv
sudo ln -s /usr/bin/python3.7 /usr/bin/python3
```

check both python3 and python3-venv are installed
```bash
$ python3 -V
Python 3.7.2
```

```bash
root@n2:~ python3 -m venv -h
usage: venv [-h] [--system-site-packages] [--symlinks | --copies] [--clear]
            [--upgrade] [--without-pip] [--prompt PROMPT]
            ENV_DIR [ENV_DIR ...]
Creates virtual Python environments in one or more target directories.
positional arguments:
  ENV_DIR               A directory to create the environment in.

optional arguments:
  -h, --help            show this help message and exit
  --system-site-packages
                        Give the virtual environment access to the system
                        site-packages dir.
  --symlinks            Try to use symlinks rather than copies, when symlinks
                        are not the default for the platform.
  --copies              Try to use copies rather than symlinks, even when
                        symlinks are the default for the platform.
  --clear               Delete the contents of the environment directory if it
                        already exists, before environment creation.
  --upgrade             Upgrade the environment directory to use this version
                        of Python, assuming Python has been upgraded in-place.
  --without-pip         Skips installing or upgrading pip in the virtual
                        environment (pip is bootstrapped by default)
  --prompt PROMPT       Provides an alternative prompt prefix for this
                        environment.

Once an environment has been created, you may wish to activate it, e.g. by
sourcing an activate script in its bin directory
```

## Create mixin_labs-python-bot project

You need clone the repo 
```bash
git clone https://github.com/myrual/mixin_labs-python-bot
cd mixin_labs-python-bot
python3 -m venv ./
```

Run **python3 -m venv** , following file and folder are created:
```bash
wenewzha:mixin_labs-python-bot wenewzhang$ ls
bin		include		lib		pyvenv.cfg
```

Once a virtual environment has been created, it can be “activated” using a script in the virtual environment’s binary directory.
```bash
wenewzha:mixin_labs-python-bot wenewzhang$ source ./bin/activate
(mixin_labs-python-bot) wenewzha:mixin_labs-python-bot wenewzhang$
```
So that “python” or "pip" invoke from the virtual environment, and you can run installed scripts without having to use their full path.

## Install required packages by "virtual environment"

Use pip to upgrade pip itself, and install required packages.
```bash
pip install --upgrade pip
pip install -r requirements.txt
```


