# busybox-static-binaries-fat

busybox v1.37.0 static binaries

```console
$ file busybox-aarch64-linux-gnu busybox-arm-linux-gnueabi busybox-arm-linux-gnueabihf busybox-mips-linux-gnu busybox-mips64-linux-gnuabi64 busybox-mips64el-linux-gnuabi64 busybox-mipsel-linux-gnu busybox-powerpc64le-linux-gnu busybox-riscv32-linux-gnu busybox-riscv64-linux-gnu busybox-x86_64-linux-gnu
busybox-aarch64-linux-gnu:       ELF 64-bit LSB executable, ARM aarch64, version 1 (GNU/Linux), statically linked, BuildID[sha1]=c0d32d2c7779f0182fb521440ceebf65d8d73259, for GNU/Linux 3.7.0, stripped
busybox-arm-linux-gnueabi:       ELF 32-bit LSB executable, ARM, EABI5 version 1 (SYSV), statically linked, BuildID[sha1]=428669ce1f342418908e584d6ec03592668454fe, for GNU/Linux 3.2.0, stripped
busybox-arm-linux-gnueabihf:     ELF 32-bit LSB executable, ARM, EABI5 version 1 (GNU/Linux), statically linked, BuildID[sha1]=a800b3886cf2495f25bf900837837ac5591820a7, for GNU/Linux 3.2.0, stripped
busybox-mips-linux-gnu:          ELF 32-bit MSB executable, MIPS, MIPS32 rel2 version 1 (SYSV), statically linked, BuildID[sha1]=91be1aef881c2a63b779d8b3065d39b6299b30ce, for GNU/Linux 3.2.0, stripped
busybox-mips64-linux-gnuabi64:   ELF 64-bit MSB executable, MIPS, MIPS64 rel2 version 1 (SYSV), statically linked, BuildID[sha1]=23e8d4722dc9e9db648c905ac4d00ccd4f455d9f, for GNU/Linux 3.2.0, stripped
busybox-mips64el-linux-gnuabi64: ELF 64-bit LSB executable, MIPS, MIPS64 rel2 version 1 (SYSV), statically linked, BuildID[sha1]=89bee626876c0f96af40345f5f37fad458c9c091, for GNU/Linux 3.2.0, stripped
busybox-mipsel-linux-gnu:        ELF 32-bit LSB executable, MIPS, MIPS32 rel2 version 1 (SYSV), statically linked, BuildID[sha1]=52790368901d9fc06b1db0b5f6ad99453bbb9185, for GNU/Linux 3.2.0, stripped
busybox-powerpc64le-linux-gnu:   ELF 64-bit LSB executable, 64-bit PowerPC or cisco 7500, OpenPOWER ELF V2 ABI, version 1 (GNU/Linux), statically linked, BuildID[sha1]=ae84f3db2d28eddb6ce8e8dd2b3b3e9e706f684a, for GNU/Linux 3.10.0, stripped
busybox-riscv32-linux-gnu:       ELF 32-bit LSB executable, UCB RISC-V, RVC, double-float ABI, version 1 (GNU/Linux), statically linked, for GNU/Linux 5.4.0, stripped
busybox-riscv64-linux-gnu:       ELF 64-bit LSB executable, UCB RISC-V, RVC, double-float ABI, version 1 (SYSV), statically linked, BuildID[sha1]=d7704dfb8f315c2f0f1ca18e92417a85c6004b20, for GNU/Linux 4.15.0, stripped
busybox-x86_64-linux-gnu:        ELF 64-bit LSB executable, x86-64, version 1 (GNU/Linux), statically linked, BuildID[sha1]=53b32d20159004311b16cae8a3b1a070af4eb558, for GNU/Linux 3.2.0, stripped
```

# bundled commands
```console
$ qemu-aarch64-static ./busybox-aarch64-linux-gnu
BusyBox v1.37.0 (2026-04-26 02:43:41 UTC) multi-call binary.
BusyBox is copyrighted by many authors between 1998-2015.
Licensed under GPLv2. See source distribution for detailed
copyright notices.

Usage: busybox [function [arguments]...]
   or: busybox --list[-full]
   or: busybox --show SCRIPT
   or: busybox --install [-s] [DIR]
   or: function [arguments]...

	BusyBox is a multi-call binary that combines many common Unix
	utilities into a single executable.  Most people will create a
	link to busybox for each function they wish to use and BusyBox
	will act like whatever it was invoked as.

Currently defined functions:
	[, [[, acpid, add-shell, addgroup, adduser, adjtimex, arch, arp,
	arping, ascii, ash, awk, base32, base64, basename, bc, beep,
	blkdiscard, blkid, blockdev, bootchartd, brctl, bunzip2, bzcat, bzip2,
	cal, cat, chat, chattr, chgrp, chmod, chown, chpasswd, chpst, chroot,
	chrt, chvt, cksum, clear, cmp, comm, conspy, cp, cpio, crc32, crond,
	crontab, cryptpw, cttyhack, cut, date, dc, dd, deallocvt, delgroup,
	deluser, depmod, devmem, df, dhcprelay, diff, dirname, dmesg, dnsd,
	dnsdomainname, dos2unix, dpkg, dpkg-deb, du, dumpkmap, dumpleases,
	echo, ed, egrep, eject, env, envdir, envuidgid, ether-wake, expand,
	expr, factor, fakeidentd, fallocate, false, fatattr, fbset, fbsplash,
	fdflush, fdformat, fdisk, fgconsole, fgrep, find, findfs, flock, fold,
	free, freeramdisk, fsck, fsck.minix, fsfreeze, fstrim, fsync, ftpd,
	ftpget, ftpput, fuser, getfattr, getopt, getty, grep, groups, gunzip,
	gzip, halt, hd, hdparm, head, hexdump, hexedit, hostid, hostname,
	httpd, hush, hwclock, i2cdetect, i2cdump, i2cget, i2cset, i2ctransfer,
	id, ifconfig, ifdown, ifenslave, ifplugd, ifup, inetd, init, insmod,
	install, ionice, iostat, ip, ipaddr, ipcalc, ipcrm, ipcs, iplink,
	ipneigh, iproute, iprule, iptunnel, kbd_mode, kill, killall, killall5,
	klogd, last, less, link, linux32, linux64, linuxrc, ln, loadfont,
	loadkmap, logger, login, logname, logread, losetup, lpd, lpq, lpr, ls,
	lsattr, lsmod, lsof, lspci, lsscsi, lsusb, lzcat, lzma, lzop, makedevs,
	makemime, man, md5sum, mdev, mesg, microcom, mim, mkdir, mkdosfs,
	mke2fs, mkfifo, mkfs.ext2, mkfs.minix, mkfs.vfat, mknod, mkpasswd,
	mkswap, mktemp, modinfo, modprobe, more, mount, mountpoint, mpstat, mt,
	mv, nameif, nanddump, nandwrite, nbd-client, nc, netstat, nice, nl,
	nmeter, nohup, nologin, nproc, nsenter, nslookup, ntpd, od, openvt,
	partprobe, passwd, paste, patch, pgrep, pidof, ping, ping6,
	pipe_progress, pivot_root, pkill, pmap, popmaildir, poweroff, powertop,
	printenv, printf, ps, pscan, pstree, pwd, pwdx, raidautorun, rdate,
	rdev, readahead, readlink, readprofile, realpath, reboot, reformime,
	remove-shell, renice, reset, resize, resume, rev, rm, rmdir, rmmod,
	route, rpm, rpm2cpio, rtcwake, run-init, run-parts, runlevel, runsv,
	runsvdir, rx, script, scriptreplay, sed, seedrng, sendmail, seq,
	setarch, setconsole, setfattr, setfont, setkeycodes, setlogcons,
	setpriv, setserial, setsid, setuidgid, sh, sha1sum, sha256sum, sha3sum,
	sha512sum, showkey, shred, shuf, slattach, sleep, smemcap, softlimit,
	sort, split, ssl_client, start-stop-daemon, stat, strings, stty, su,
	sulogin, sum, sv, svc, svlogd, svok, swapoff, swapon, switch_root,
	sync, sysctl, syslogd, tac, tail, tar, taskset, tc, tcpsvd, tee,
	telnet, telnetd, test, tftp, tftpd, time, timeout, top, touch, tr,
	traceroute, traceroute6, tree, true, truncate, ts, tsort, tty, ttysize,
	tunctl, ubiattach, ubidetach, ubimkvol, ubirename, ubirmvol, ubirsvol,
	ubiupdatevol, udhcpc, udhcpc6, udhcpd, udpsvd, uevent, umount, uname,
	unexpand, uniq, unix2dos, unlink, unlzma, unshare, unxz, unzip, uptime,
	users, usleep, uudecode, uuencode, vconfig, vi, vlock, volname, w,
	wall, watch, watchdog, wc, wget, which, who, whoami, whois, xargs, xxd,
	xz, xzcat, yes, zcat, zcip
```
