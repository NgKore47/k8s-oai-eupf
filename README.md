# OAI-eUPF

This readme provides guidelines for deploying OAI 5G Core with an eBPF-based User Plane Function (UPF).
### Step 1: Clone this repository
```bash
git clone https://github.com/wafi981/-k8s-oai-eupf.git ~/k8s-oai-eupf
cd ~/k8s-oai-eupf
```
### Step 2: Install make and deploy rke2 kubernetes cluster
```bash
sudo apt install make -y
make node-prep
```
### Step 3: After rke2 installation deploy oai-5g-core with oai-ran-simulator
```bash
make oai
```
This will deploy end-to-end 5g core on kubernetes

