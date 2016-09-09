Q: What is Botdefender?
A: Botdefender is simple and flexible tool to lock out the bad guys from your
   host. It waits on changes in log files (similar to tail -f), scans new entries
   for attack/bot patterns and locks out IPs by adding roules into your iptables.
   Your instance is completely self-supporting and does not send our receive anything.

Q: What does it append on?
A: Botdefender needs some logs to parse, iptables for locking addresses out and
   sudo access to iptables if not run as root.

Q: How to install?
A: Just drop the files somewhere and make sure, it is run with the according parameters.
   Currently there is no service script yet, so for now you will have to add it to your
   systemd/initd/... manually.

