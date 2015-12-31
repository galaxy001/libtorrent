# libtorrent

## Sources

BitTorrent & BitTornado
````
rsync -a rsync://rsync.gentoo.org/gentoo-portage/net-p2p/ ./gentoo-portage/net-p2p/

ftp://ftp.cn.debian.org/gentoo/distfiles/BitTorrent-4.4.0.tar.gz
http://download2.bittornado.com/download/BitTornado-0.3.18.tar.gz, http://www.bittornado.com/download.html
````

### Gentoo Packages

#### net-p2p/bittornado
````python
	Available versions:  0.3.18-r2 ~0.3.18-r3 {PYTHON_TARGETS="python2_7"}
	Installed versions:  0.3.18-r2(01:20:47 PM 12/31/2015)
	Homepage:            http://www.bittornado.com/
	Description:         TheShad0w's experimental BitTorrent client
````

#### net-p2p/bittorrent
````python
	Available versions:  [M]4.4.0-r2 [M]4.4.0-r3 {aqua gtk PYTHON_TARGETS="python2_7"}
	Installed versions:  4.4.0-r3(03:19:45 AM 12/30/2015)(-aqua -gtk PYTHON_TARGETS="python2_7")
	Homepage:            http://www.bittorrent.com/
	Description:         Tool for distributing files via a distributed network of nodes
````
##### Masks

Dead upstream, security issues, see [bug #557856](https://bugs.gentoo.org/show_bug.cgi?id=557856) Removal in a month  
Affected packages net-p2p/bittorrent  
Author/Date Sergey Popov <pinkbyte@gentoo.org> (25 Nov 2015)

````
GLSAMaker/CVETool Bot (gentoo-dev) 2015-08-15 15:58:59 UTC

CVE-2015-5474 (http://nvd.nist.gov/nvd.cfm?cvename=CVE-2015-5474):
  BitTorrent and uTorrent allow remote attackers to inject command line parameters and execute 
  arbitrary commands via a crafted URL using the (1) bittorrent or (2) magnet protocol.
````




