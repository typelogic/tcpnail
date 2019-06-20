# Server
`nc -l -p $port`
`tcpdump -i eth0 port $port -w $pcapfile`

# Client
`echo 'hello world' | nc $ipaddr $port`

# Why
I turned off vsftpd service and there is no listener server process at port 21. Yet, `nc` reported it as open. 
