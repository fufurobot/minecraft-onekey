create a bash project: one key deployable minecraft server by apptainer. 

it probes the ssh passwordless closure, find the the most powerful server in the least busy ones, use fake-chroot to deploy a proper minecraft server, and use ssh tunnel to route to all network interfaces on the host it executes on a random port. 

a proper server is:
1. a version solver for mods that which minecraft server type and verions it works on.
2. the newest minecraft version with fabric if mod folder is specified at all
3. a http readonly server on another random port that serves the client side properly as a single .zip. 

a mod folder must contain subfolder of (server) and (client) for installment. 

a ssh passwordless closure is what the host can reach and get a shell by ssh in finite number of hops without providing password.

the apptainer bundle should contain a newest fabric minecraft server and client to serve. 

PKGBUILD will provided for arch linux build. i am not planning to support other linux distro. 


