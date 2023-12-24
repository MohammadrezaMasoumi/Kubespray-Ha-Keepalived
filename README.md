you should set a VIP ( Virtual IP ) that is the way to comminucate to our Master Nodes.
first of all we should configure Haproxy TCP Frontend and set VIP ( Like x.x.x.x:6443 ) , second you should  set your backend servers to proxy your requests to kube api servers ports.
Keepalived is the manager of VIP and handle the VIP termination between two Haproxys by running a script every one second. 
