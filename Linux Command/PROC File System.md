## /proc

- Created in RAM everytime system bootsup
- We can Read and Write information , but it is only temporary
- To edit info in proc we need to have root privilige

### Any change make to /proc file will be reset if we boot our system again to make the change temporary what we need to do is :-

### Remove the comment symbol "#" from the file /etc/sysctl.conf

### command will be vi /etc/sysctl.conf