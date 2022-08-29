# Install WASM Runtimes  
  
## Install Wasmedge  

```
curl -sSf https://raw.githubusercontent.com/WasmEdge/WasmEdge/master/utils/install.sh | bash
```
  
Output:  
```
Detected Linux-x86_64
No path provided
Installing in /home/IamDeveloper/.wasmedge
WasmEdge Installation at /home/IamDeveloper/.wasmedge
Fetching WasmEdge-0.10.1
/tmp/wasmedge.1097 ~
######################################################################## 100.0%
~
Installing WasmEdge-0.10.1-Linux in /home/IamDeveloper/.wasmedge/include
Installing WasmEdge-0.10.1-Linux in /home/IamDeveloper/.wasmedge/lib
Installing WasmEdge-0.10.1-Linux in /home/IamDeveloper/.wasmedge/bin

source /home/IamDeveloper/.wasmedge/env to use wasmedge binaries
```
  

View your ```${HOME}/.bashrc``` and at the bottom, the install should have added:
```
. "/home/IamDeveloper/.wasmedge/env"
```
 
So you can either run ```source ${HOME}/.bashrc``` or ```source /home/IamDeveloper/.wasmedge/env``` directly.  
  
  
## Install Wasmtime  
  
```
curl https://wasmtime.dev/install.sh -sSf | bash
```
  
Output:
```
  Installing latest version of Wasmtime (v0.40.0)
    Checking for existing Wasmtime installation
    Fetching archive for Linux, version v0.40.0
https://github.com/bytecodealliance/wasmtime/releases/download/v0.40.0/wasmtime-v0.40.0-x86_64-linux.tar.xz
######################################################################## 100.0%
    Creating directory layout
  Extracting Wasmtime binaries
wasmtime-v0.40.0-x86_64-linux/
wasmtime-v0.40.0-x86_64-linux/wasmtime
wasmtime-v0.40.0-x86_64-linux/LICENSE
wasmtime-v0.40.0-x86_64-linux/README.md
     Editing user profile (/home/IamDeveloper/.bashrc)
    Finished installation. Open a new terminal to start using Wasmtime!
```
  
View your ```${HOME}/.bashrc``` and at the bottom, the install should have added:
```
export WASMTIME_HOME="$HOME/.wasmtime"

export PATH="$WASMTIME_HOME/bin:$PATH" 
```
 
Run ```source ${HOME}/.bashrc```.  
  
  
## Install Wasmer  
  
```
curl https://get.wasmer.io -sSfL | sh
```
  
Output:  
```
Welcome to the Wasmer bash installer!

               ww
               wwwww
        ww     wwwwww  w
        wwwww      wwwwwwwww
ww      wwwwww  w     wwwwwww
wwwww      wwwwwwwwww   wwwww
wwwwww  w      wwwwwww  wwwww
wwwwwwwwwwwwww   wwwww  wwwww
wwwwwwwwwwwwwww  wwwww  wwwww
wwwwwwwwwwwwwww  wwwww  wwwww
wwwwwwwwwwwwwww  wwwww  wwwww
wwwwwwwwwwwwwww  wwwww   wwww
wwwwwwwwwwwwwww  wwwww
   wwwwwwwwwwww   wwww
       wwwwwwww
           wwww

downloading: wasmer-linux-amd64
Latest release: 2.3.0
Downloading archive from https://github.com/wasmerio/wasmer/releases/download/2.3.0/wasmer-linux-amd64.tar.gz
######################################################################## 100.0%
installing: /home/IamDeveloper/.wasmer
Updating bash profile /home/IamDeveloper/.bashrc
we've added the following to your /home/IamDeveloper/.bashrc
If you have a different profile please add the following:

# Wasmer
export WASMER_DIR="/home/IamDeveloper/.wasmer"
[ -s "$WASMER_DIR/wasmer.sh" ] && source "$WASMER_DIR/wasmer.sh"
check: wasmer 2.3.0 installed successfully ✓
wasmer & wapm will be available the next time you open the terminal.
If you want to have the commands available now please execute:

source /home/IamDeveloper/.wasmer/wasmer.sh
downloading: wapm-cli-linux-amd64
Latest release: 0.5.5
Downloading archive from https://github.com/wasmerio/wapm-cli/releases/download/v0.5.5/wapm-cli-linux-amd64.tar.gz
######################################################################## 100.0%
installing: /home/IamDeveloper/.wasmer
```
  
View your ```${HOME}/.bashrc``` and at the bottom, the install should have added:
```
# Wasmer
export WASMER_DIR="/home/IamDeveloper/.wasmer"
[ -s "$WASMER_DIR/wasmer.sh" ] && source "$WASMER_DIR/wasmer.sh"
```
 
Run ```source ${HOME}/.bashrc```.  
  
  

  
