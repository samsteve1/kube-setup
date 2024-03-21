Start by making the script files executable by running `sudo chmod +x file-name.sh`

Execute the setup-container.sh and setup-kube-tools.sh on all the nodes to install containerd, kubeadm, kubelet and kubeapiserver.

Now you are in a postion to initialize your control plane(s) with kubeadm by running these commands:
`sudo kubeadm init --pod-network-cidr=10.244.0.0/16 --apiserver-advertise-address=master-node-ip-address`
