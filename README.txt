When installing botdefender in user space you need
	- read permission on all log files that are meant to be parsed
	- sudo rights for the user on the botdefender ip-table:
		botdefender ALL=(root:root) NOPASSWD: /sbin/iptables -D botdefender *,/sbin/iptables -L botdefender *,/sbin/iptables -I botdefender *,/sbin/iptables -F botdefender
You may also want to make sudo less talkative:
	Defaults:botdefender    !syslog

