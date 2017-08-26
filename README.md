# libtorrent

## Sources

### BitTorrent & BitTornado

````
rsync -a rsync://rsync.gentoo.org/gentoo-portage/net-p2p/ ./gentoo-portage/net-p2p/

ftp://ftp.cn.debian.org/gentoo/distfiles/BitTorrent-4.4.0.tar.gz
http://download2.bittornado.com/download/BitTornado-0.3.18.tar.gz, http://www.bittornado.com/download.html
````

#### BitTorrent 5.3 source code

Available from [Internet Archive 2010-05-30](http://web.archive.org/web/20100330145634/http://www.bittorrent.com/btusers/download/directory-list)

````
BitTorrent-5.3-GPL.tar.gz	February 4, 2009, 6:01 pm
````

Available till [2010-08-31](http://web.archive.org/web/20100831070823/http://www.bittorrent.com/btusers/download/directory-list).  
See also <https://github.com/santazhang/BitTorrent-5.3-GPL> and <https://github.com/kenorb-contrib/BitTorrent> ([mirrored](https://github.com/galaxysd/BitTorrent)).

##### Install BTL-0.31dev-r0 from BitTorrent-5.3-GPL

````bash
python2 -m ensurepip --upgrade
pip2 install ./python_BTL_BitTorrent-5.3-GPL/
````

Remember `cfv` requires Python2.

There are [some 4.4.0 patches](gentoo-portage/net-p2p/bittorrent/files) that newer than 5.30. Considering merge them later.

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

Well, the 2010 version should *contain* this bug.


