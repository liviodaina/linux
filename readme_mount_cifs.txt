#redhat mount cifs kerberos
sudo umount -f /home/livio/mount
kinit -V livio@IMETEC.IT
sudo mount -t cifs -o user=livio,cruid=livio,sec=krb5,gid=1000,uid=1000,ip=192.9.200.113 //imetec.it/root /home/livio/mount
#linuxmint
sudo umount -f /home/livio/mount
kinit -V livio@IMETEC.IT
sudo mount -t cifs -o user=livio,cruid=$(id -u livio),gid=1000,uid=1000,ip=192.9.200.113 //imetec.it/root /home/livio/mount

