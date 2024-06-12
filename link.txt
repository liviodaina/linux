openvpn client linux

https://community.openvpn.net/openvpn/wiki/OpenVPN3Linux
profile downloaded from vpn... server
openvpn3 configs-list
openvpn3 session-start --config profile-266.ovpn
openvpn3 sessions-list
openvpn3 session-manage --disconnect -o /net/openvpn/v3/sessions/76305c9es4274s4b60sa007sd456868c36aa
.
prova modifica inplace
----
openvpn3_dev.repo

https://copr.fedorainfracloud.org/coprs/ojab/openvpn3/

livio@fed10:~/opevpn$ cat /etc/yum.repos.d/openvpn3_dev.repo 
[copr:copr.fedorainfracloud.org:dsommers:openvpn3-devsnapshots]
name=Copr repo for openvpn3-devsnapshots owned by dsommers
baseurl=https://download.copr.fedorainfracloud.org/results/dsommers/openvpn3-devsnapshots/fedora-$releasever-$basearch/
type=rpm-md
skip_if_unavailable=True
gpgcheck=1
gpgkey=https://download.copr.fedorainfracloud.org/results/dsommers/openvpn3-devsnapshots/pubkey.gpg
repo_gpgcheck=0
enabled=1
enabled_metadata=1
