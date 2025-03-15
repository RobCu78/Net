##
##  88      a8P         db        88        88  ##
##  88    .88'         d88b       88        88  ##
##  88   88'          d8''8b      88        88  ##
##  88 d88           d8'  '8b     88        88  ##
##  8888'88.        d8YaaaaY8b    88        88  ##
##  88P   Y8b      d8''''''''8b   88        88  ##
##  88     '88.   d8'        '8b  88        88  ##
##  88       Y8b d8'          '8b 888888888 88  ##
##                                              ##
####  ############# NetHunter ####################

[*] Checking device architecture ...

[1] NetHunter ARM64 (full)
[2] NetHunter ARM64 (minimal)
[3] NetHunter ARM64 (nano)
Enter the image you want to install: nethunter

[*] Checking package dependencies...
  proot is OK
  tar is OK
Installing axel...
Reading package lists... Done
Building dependency tree... Done
Reading state information... Done
The following NEW packages will be installed:
  axel
0 upgraded, 1 newly installed, 0 to remove and 0 not upgraded.
Need to get 24.5 kB of archives.
After this operation, 106 kB of additional disk space will be used.
Get:1 https://2.mirrors.in.sahilister.net/termux/termux-main stable/main aarch64 axel aarch64 2.17.14 [24.5 kB]
Fetched 24.5 kB in 4s (6718 B/s)
Selecting previously unselected package axel.
(Reading database ... 10885 files and directories currently installed.)
Preparing to unpack .../axel_2.17.14_aarch64.deb ...
Unpacking axel (2.17.14) ...
Setting up axel (2.17.14) ...
Reading package lists... Done                                                                               Building dependency tree... Done
Reading state information... Done                                                                           Calculating upgrade... Done
0 upgraded, 0 newly installed, 0 to remove and 0 not upgraded.
[*] Downloading rootfs...

--2025-03-15 15:06:31--  https://image-nethunter.kali.org/nethunter-fs/kali-daily/kali-nethunter-daily-dev-rootfs-full-arm64.tar.xz
Resolving image-nethunter.kali.org (image-nethunter.kali.org)... 2606:4700::6812:49f, 2606:4700::6812:59f, 104.18.5.159, ...
Connecting to image-nethunter.kali.org (image-nethunter.kali.org)|2606:4700::6812:49f|:443... connected.
HTTP request sent, awaiting response... 200 OK
Length: 2226426224 (2.1G) [application/x-xz]
Saving to: ‘kali-nethunter-daily-dev-rootfs-full-arm64.tar.xz’

kali-nethunter-daily-dev-r   5%[=>                                       ] 119.22M   170KB/s    in 1m 41s

2025-03-15 15:08:13 (1.18 MB/s) - Read error at byte 125009670/2226426224 (Software caused connection abort). Retrying.                                                                                                 
--2025-03-15 15:08:14--  (try: 2)  https://image-nethunter.kali.org/nethunter-fs/kali-daily/kali-nethunter-daily-dev-rootfs-full-arm64.tar.xz
Connecting to image-nethunter.kali.org (image-nethunter.kali.org)|2606:4700::6812:49f|:443... failed: Network is unreachable.
Connecting to image-nethunter.kali.org (image-nethunter.kali.org)|2606:4700::6812:59f|:443... failed: Network is unreachable.
Connecting to image-nethunter.kali.org (image-nethunter.kali.org)|104.18.5.159|:443... failed: Network is unreachable.
Connecting to image-nethunter.kali.org (image-nethunter.kali.org)|104.18.4.159|:443... failed: Network is unreachable.
Resolving image-nethunter.kali.org (image-nethunter.kali.org)... failed: No address associated with hostname.
wget: unable to resolve host address ‘image-nethunter.kali.org’
~ $ nethunter
┏━(Message from Kali developers)
┃
┃ This is a minimal installation of Kali Linux, you likely
┃ want to install supplementary tools. Learn how:
┃ ⇒ https://www.kali.org/docs/troubleshooting/common-minimum-setup/
┃
┗━(Run: “touch ~/.hushlogin” to hide this message)
┌──(/data/data/com.termux/files/kali)─(kali㉿localhost)-[~]
└─$ apt update && apt upgrade -y
Get:1 http://kali.download/kali kali-rolling InRelease [41.5 kB]
Get:2 http://kali.download/kali kali-rolling/main arm64 Packages [20.5 MB]
Get:3 http://kali.download/kali kali-rolling/contrib arm64 Packages [99.5 kB]
Get:4 http://kali.download/kali kali-rolling/non-free arm64 Packages [161 kB]
Get:5 http://kali.download/kali kali-rolling/non-free-firmware arm64 Packages [9,937 B]
Fetched 20.8 MB in 11s (1,875 kB/s)
247 packages can be upgraded. Run 'apt list --upgradable' to see them.
The following packages were automatically installed and are no longer required:
  libldap-2.5-0   libpython3.11-minimal  perl-modules-5.38  python3.11-minimal
  libperl5.38t64  libpython3.11-stdlib   python3.11
Use 'apt autoremove' to remove them.

Upgrading:
  abootimg                    libaudit-common         libncursesw6              libzstd1
  apt                         libaudit1               libnettle8t64             linux-base
  apt-transport-https         libbinutils             libnewt0.52               locales
  apt-utils                   libblkid1               libnftables1              locales-all
  base-files                  libbpf1                 libnftnl11                login
  base-passwd                 libbrotli1              libnghttp2-14             logrotate
  bash                        libbsd0                 libnghttp3-9              logsave
  binutils                    libbz2-1.0              libngtcp2-16              mawk
  binutils-aarch64-linux-gnu  libc-bin                libngtcp2-crypto-gnutls8  media-types
  binutils-common             libc-l10n               libnsl2                   mount
  bsdutils                    libc6                   libp11-kit0               nano
  busybox                     libcap-ng0              libpam-modules            ncurses-base
  ca-certificates             libcap2                 libpam-modules-bin        ncurses-bin
  cgpt                        libcap2-bin             libpam-runtime            ncurses-term
  coreboot-utils              libcbor0.10             libpam-systemd            nethunter-utils
  coreboot-utils-doc          libcom-err2             libpam0g                  nftables
  coreutils                   libcrypt1               libpci3                   ntpsec-ntpdate
  cron                        libctf-nobfd0           libpcre2-8-0              ntpsec-ntpdig
  cron-daemon-common          libctf0                 libpopt0                  openssh-client
  dash                        libcurl3t64-gnutls      libproc2-0                openssh-server
  dbus                        libdb5.3t64             libpsl5t64                openssh-sftp-server
  dbus-bin                    libdbus-1-3             libpython3-stdlib         openssl
  dbus-daemon                 libdebconfclient0       libreadline8t64           passwd
  dbus-session-bus-common     libedit2                librtmp1                  patch
  dbus-system-bus-common      libelf1t64              libsasl2-2                pci.ids
  dbus-user-session           liberror-perl           libsasl2-modules          pciutils
  debconf                     libexpat1               libsasl2-modules-db       perl
  debconf-i18n                libext2fs2t64           libseccomp2               perl-base
  debianutils                 libfdisk1               libselinux1               procps
  diffutils                   libffi8                 libsemanage-common        publicsuffix
  dmidecode                   libfido2-1              libsemanage2              python3
  dpkg                        libflashrom1            libsepol2                 python3-minimal
  e2fsprogs                   libftdi1-2              libsframe1                python3-ntp
  fdisk                       libgcc-s1               libslang2                 readline-common
  findutils                   libgcrypt20             libsmartcols1             runit-helper
  flashrom                    libgdbm-compat4t64      libsodium23               sed
  gcc-14-base                 libgdbm6t64             libsqlite3-0              sphinx-rtd-theme-common
  git                         libgmp10                libss2                    sudo
  git-man                     libgnutls30t64          libssh2-1t64              systemd
  gpgv                        libgpg-error0           libssl3t64                systemd-sysv
  grep                        libgpm2                 libstdc++6                sysvinit-utils
  gzip                        libgprofng0             libsystemd-shared         tar
  hostname                    libgssapi-krb5-2        libsystemd0               tree
  ifupdown                    libhogweed6t64          libtasn1-6                tzdata
  init                        libidn2-0               libtext-charwidth-perl    ucf
  init-system-helpers         libjansson4             libtext-iconv-perl        udev
  initramfs-tools             libjaylink0             libtinfo6                 usbutils
  initramfs-tools-core        libjs-sphinxdoc         libtirpc3t64              usr-is-merged
  iproute2                    libk5crypto3            libudev1                  util-linux
  iputils-ping                libkeyutils1            libunistring5             vboot-kernel-utils
  isc-dhcp-client             libklibc                libusb-1.0-0              vboot-utils
  isc-dhcp-common             libkmod2                libuuid1                  vim
  javascript-common           libkrb5-3               libwrap0                  vim-common
  kali-defaults               libkrb5support0         libx11-6                  vim-runtime
  kbd                         libldap-2.5-0           libx11-data               vim-tiny
  klibc-utils                 libldap-common          libxau6                   whiptail
  kmod                        liblocale-gettext-perl  libxcb1                   xauth
  less                        liblz4-1                libxdmcp6                 zlib1g
  libacl1                     liblzma5                libxext6                  zsh
  libapparmor1                libmd0                  libxmuu1                  zsh-common
  libapt-pkg6.0t64            libmnl0                 libxtables12              zstd
  libattr1                    libmount1               libxxhash0

Installing dependencies:
  dracut-install  libpython3.13-minimal  login.defs               python3.13
  libldap2        libpython3.13-stdlib   openssl-provider-legacy  python3.13-minimal
  libperl5.40     linux-sysctl-defaults  perl-modules-5.40        sqv

Suggested packages:
  python3.13-venv  python3.13-doc  binfmt-support

Summary:
  Upgrading: 247, Installing: 12, Removing: 0, Not Upgrading: 0
  Download size: 133 MB
  Space needed: 88.3 MB / 9,277 MB available

Get:1 http://kali.download/kali kali-rolling/main arm64 dbus-session-bus-common all 1.16.2-1 [51.6 kB]
Get:2 http://kali.darklab.sh/kali kali-rolling/main arm64 libc-l10n all 2.40-3 [724 kB]
Get:3 http://kali.download/kali kali-rolling/main arm64 locales all 2.40-3 [3,903 kB]
Get:4 http://kali.darklab.sh/kali kali-rolling/main arm64 locales-all arm64 2.40-3 [11.1 MB]
Get:6 http://kali.download/kali kali-rolling/main arm64 libc-bin arm64 2.40-3 [540 kB]
Get:8 http://kali.download/kali kali-rolling/main arm64 libperl5.40 arm64 5.40.1-2 [4,143 kB]
Get:18 http://mirrors.ocf.berkeley.edu/kali kali-rolling/main arm64 libgdbm-compat4t64 arm64 1.24-2 [50.3 kB]
Get:23 http://kali.mirror.rafal.ca/kali kali-rolling/main arm64 libgcc-s1 arm64 14.2.0-17 [54.1 kB]
Get:45 http://mirrors.ocf.berkeley.edu/kali kali-rolling/main arm64 libselinux1 arm64 3.8-3 [79.0 kB]
Get:49 http://mirrors.ocf.berkeley.edu/kali kali-rolling/main arm64 libpam-systemd arm64 257.3-1 [273 kB]
Get:61 http://kali.mirror.rafal.ca/kali kali-rolling/main arm64 libk5crypto3 arm64 1.21.3-4 [81.5 kB]
Get:9 http://kali.download/kali kali-rolling/main arm64 perl arm64 5.40.1-2 [267 kB]
Get:63 http://mirrors.ocf.berkeley.edu/kali kali-rolling/main arm64 libkeyutils1 arm64 1.6.3-4 [9,352 B]
Get:11 http://http.kali.org/kali kali-rolling/main arm64 liblocale-gettext-perl arm64 1.07-7+b1 [15.2 kB]
Get:13 http://http.kali.org/kali kali-rolling/main arm64 libtext-charwidth-perl arm64 0.04-11+b4 [9,652 B]
Get:14 http://kali.download/kali kali-rolling/main arm64 libbz2-1.0 arm64 1.0.8-6 [37.8 kB]
Get:15 http://kali.download/kali kali-rolling/main arm64 libcrypt1 arm64 1:4.4.38-1 [91.8 kB]
Get:17 http://kali.download/kali kali-rolling/main arm64 libgdbm6t64 arm64 1.24-2 [74.0 kB]
Get:77 http://kali.mirror.rafal.ca/kali kali-rolling/main arm64 dbus arm64 1.16.2-1 [70.1 kB]
Get:21 http://kali.download/kali kali-rolling/main arm64 debconf all 1.5.89 [120 kB]
Get:22 http://kali.download/kali kali-rolling/main arm64 gcc-14-base arm64 14.2.0-17 [49.1 kB]
Get:26 http://kali.download/kali kali-rolling/main arm64 libssl3t64 arm64 3.4.1-1 [2,636 kB]
Get:81 http://kali.mirror.rafal.ca/kali kali-rolling/main arm64 base-files arm64 1:2025.1.0 [76.8 kB]
Get:82 http://kali.mirror.rafal.ca/kali kali-rolling/main arm64 bash arm64 5.2.37-1.1 [1,455 kB]
Get:92 http://kali.mirror.rafal.ca/kali kali-rolling/main arm64 libkmod2 arm64 34-3 [58.9 kB]
Get:104 http://http.kali.org/kali kali-rolling/main arm64 libgmp10 arm64 2:6.3.0+dfsg-3 [535 kB]
Get:117 http://mirrors.ocf.berkeley.edu/kali kali-rolling/main arm64 initramfs-tools all 0.145 [14.9 kB]
Get:102 http://http.kali.org/kali kali-rolling/main arm64 ncurses-bin arm64 6.5+20250216-1 [432 kB]
Get:32 http://kali.download/kali kali-rolling/main arm64 libsmartcols1 arm64 2.40.4-2 [136 kB]
Get:34 http://kali.download/kali kali-rolling/main arm64 libblkid1 arm64 2.40.4-2 [164 kB]
Get:5 http://kali.darklab.sh/kali kali-rolling/main arm64 libc6 arm64 2.40-3 [2,453 kB]
Get:116 http://kali.mirror.rafal.ca/kali kali-rolling/main arm64 initramfs-tools-core all 0.145 [49.2 kB]
Get:120 http://kali.mirror.rafal.ca/kali kali-rolling/main arm64 e2fsprogs arm64 1.47.2-1 [563 kB]
Get:35 http://kali.download/kali kali-rolling/main arm64 libmount1 arm64 2.40.4-2 [191 kB]
Get:121 http://kali.mirror.rafal.ca/kali kali-rolling/main arm64 dracut-install arm64 106-5 [35.8 kB]
Get:123 http://kali.mirror.rafal.ca/kali kali-rolling/main arm64 libklibc arm64 2.0.14-1 [46.7 kB]
Get:36 http://kali.download/kali kali-rolling/main arm64 libuuid1 arm64 2.40.4-2 [36.1 kB]
Get:140 http://mirrors.ocf.berkeley.edu/kali kali-rolling/main arm64 libnghttp3-9 arm64 1.8.0-1 [63.2 kB]
Get:40 http://http.kali.org/kali kali-rolling/main arm64 libncursesw6 arm64 6.5+20250216-1 [124 kB]
Get:42 http://kali.download/kali kali-rolling/main arm64 readline-common all 8.2-6 [69.4 kB]
Get:114 http://http.kali.org/kali kali-rolling/main arm64 ncurses-term all 6.5+20250216-1 [518 kB]
Get:43 http://kali.download/kali kali-rolling/main arm64 libreadline8t64 arm64 8.2-6 [159 kB]
Get:127 http://mirror.math.princeton.edu/pub/kali kali-rolling/main arm64 cron arm64 3.0pl1-194 [84.6 kB]
Get:134 http://mirror.math.princeton.edu/pub/kali kali-rolling/main arm64 libtasn1-6 arm64 4.20.0-2 [47.3 kB]
Get:44 http://kali.download/kali kali-rolling/main arm64 libpcre2-8-0 arm64 10.45-1 [262 kB]
Get:146 http://mirror.math.princeton.edu/pub/kali kali-rolling/main arm64 libcurl3t64-gnutls arm64 8.12.1-3 [336 kB]
Get:157 http://mirrors.ocf.berkeley.edu/kali kali-rolling/main arm64 libedit2 arm64 3.1-20250104-1 [89.3 kB]
Get:160 http://mirror.math.princeton.edu/pub/kali kali-rolling/main arm64 openssh-sftp-server arm64 1:9.9p2-1 [60.4 kB]
Get:46 http://http.kali.org/kali kali-rolling/main arm64 libcap2 arm64 1:2.66-5+b1 [27.2 kB]
Get:47 http://kali.download/kali kali-rolling/main arm64 libpam0g arm64 1.7.0-3 [68.6 kB]
Get:50 http://kali.download/kali kali-rolling/main arm64 debianutils arm64 5.21 [92.1 kB]
Get:53 http://kali.download/kali kali-rolling/main arm64 systemd arm64 257.3-1 [2,922 kB]
Get:10 http://kali.darklab.sh/kali kali-rolling/main arm64 perl-base arm64 5.40.1-2 [1,525 kB]
Get:171 http://kali.mirror.rafal.ca/kali kali-rolling/main arm64 python3 arm64 3.13.1-2 [28.0 kB]
Get:181 http://http.kali.org/kali kali-rolling/main arm64 gpgv arm64 2.2.46-1+b1 [200 kB]
Get:20 http://kali.darklab.sh/kali kali-rolling/main arm64 debconf-i18n all 1.5.89 [196 kB]
Get:188 http://http.kali.org/kali kali-rolling/main arm64 libpopt0 arm64 1.19+dfsg-2 [42.8 kB]
Get:39 http://kali.darklab.sh/kali kali-rolling/main arm64 mount arm64 2.40.4-2 [154 kB]
Get:41 http://http.kali.org/kali kali-rolling/main arm64 libtinfo6 arm64 6.5+20250216-1 [341 kB]
Get:189 http://http.kali.org/kali kali-rolling/main arm64 logrotate arm64 3.22.0-1+b1 [58.7 kB]
Get:55 http://kali.darklab.sh/kali kali-rolling/main arm64 libelf1t64 arm64 0.192-4 [189 kB]
Get:192 http://kali.mirror.rafal.ca/kali kali-rolling/main arm64 libnftnl11 arm64 1.2.8-1 [60.8 kB]
Get:195 http://kali.mirror.rafal.ca/kali kali-rolling/main arm64 vim arm64 2:9.1.1113-1 [1,525 kB]
Get:57 http://kali.darklab.sh/kali kali-rolling/main arm64 libmnl0 arm64 1.0.5-3 [11.9 kB]
Get:59 http://kali.darklab.sh/kali kali-rolling/main arm64 libkrb5-3 arm64 1.21.3-4 [308 kB]
Get:204 http://mirror.math.princeton.edu/pub/kali kali-rolling/main arm64 openssl arm64 3.4.1-1 [1,390 kB]
Get:72 http://kali.darklab.sh/kali kali-rolling/main arm64 systemd-sysv arm64 257.3-1 [61.4 kB]
Get:75 http://kali.darklab.sh/kali kali-rolling/main arm64 dbus-system-bus-common all 1.16.2-1 [52.7 kB]
Get:76 http://kali.darklab.sh/kali kali-rolling/main arm64 dbus-bin arm64 1.16.2-1 [78.2 kB]
Get:198 http://kali.mirror.rafal.ca/kali kali-rolling/main arm64 vim-runtime all 2:9.1.1113-1 [7,128 kB]
Get:78 http://kali.darklab.sh/kali kali-rolling/main arm64 dbus-daemon arm64 1.16.2-1 [151 kB]
Get:80 http://http.kali.org/kali kali-rolling/main arm64 usr-is-merged all 39+nmu2 [5,936 B]
Get:85 http://kali.darklab.sh/kali kali-rolling/main arm64 dash arm64 0.5.12-12 [95.6 kB]
Get:88 http://kali.darklab.sh/kali kali-rolling/main arm64 liblz4-1 arm64 1.10.0-3 [59.6 kB]
Get:93 http://kali.darklab.sh/kali kali-rolling/main arm64 udev arm64 257.3-1 [1,338 kB]
Get:54 http://kali.download/kali kali-rolling/main arm64 libsystemd0 arm64 257.3-1 [419 kB]
Get:245 http://http.kali.org/kali kali-rolling/main arm64 libxmuu1 arm64 2:1.1.3-3+b4 [22.0 kB]
Get:254 http://http.kali.org/kali kali-rolling/main arm64 vboot-kernel-utils arm64 0~R106-15054.B+dfsg-0.1 [311 kB]
Get:258 http://mirror.math.princeton.edu/pub/kali kali-rolling/main arm64 zsh-common all 5.9-8 [4,146 kB]
Get:56 http://kali.download/kali kali-rolling/main arm64 libbpf1 arm64 1:1.5.0-2 [159 kB]
Get:97 http://http.kali.org/kali kali-rolling/main arm64 dpkg arm64 1.22.15+kali2 [1,524 kB]
Get:58 http://kali.download/kali kali-rolling/main arm64 libgssapi-krb5-2 arm64 1.21.3-4 [127 kB]
Get:64 http://http.kali.org/kali kali-rolling/main arm64 libtirpc3t64 arm64 1.3.4+ds-1.3+b1 [78.7 kB]
Get:65 http://kali.download/kali kali-rolling/main arm64 libxtables12 arm64 1.8.11-2 [30.6 kB]
Get:66 http://http.kali.org/kali kali-rolling/main arm64 libcap2-bin arm64 1:2.66-5+b1 [34.3 kB]
Get:67 http://kali.download/kali kali-rolling/main arm64 iproute2 arm64 6.13.0-1 [1,045 kB]
Get:233 http://kali.mirror.rafal.ca/kali kali-rolling/main arm64 libflashrom1 arm64 1.4.0-3 [145 kB]
Get:237 http://http.kali.org/kali kali-rolling/main arm64 libsasl2-modules arm64 2.1.28+dfsg1-9 [62.9 kB]
Get:250 http://http.kali.org/kali kali-rolling/main arm64 patch arm64 2.7.6-7+b1 [118 kB]
Get:256 http://kali.mirror.rafal.ca/kali kali-rolling/main arm64 xauth arm64 1:1.1.2-1.1 [35.4 kB]
Get:108 http://http.kali.org/kali kali-rolling/main arm64 apt arm64 2.9.29+kali1 [1,358 kB]
Get:68 http://http.kali.org/kali kali-rolling/main arm64 libapparmor1 arm64 4.1.0~beta5-3 [42.6 kB]
Get:69 http://kali.download/kali kali-rolling/main arm64 libpam-modules-bin arm64 1.7.0-3 [48.0 kB]
Get:70 http://kali.download/kali kali-rolling/main arm64 libpam-modules arm64 1.7.0-3 [170 kB]
Get:71 http://kali.download/kali kali-rolling/main arm64 libpam-runtime all 1.7.0-3 [248 kB]
Get:73 http://kali.download/kali kali-rolling/main arm64 dbus-user-session arm64 1.16.2-1 [51.5 kB]
Get:74 http://kali.download/kali kali-rolling/main arm64 libexpat1 arm64 2.6.4-1 [90.7 kB]
Get:83 http://kali.download/kali kali-rolling/main arm64 bsdutils arm64 1:2.40.4-2 [105 kB]
Get:84 http://http.kali.org/kali kali-rolling/main arm64 coreutils arm64 9.5-1+b1 [2,858 kB]
Get:111 http://kali.darklab.sh/kali kali-rolling/main arm64 base-passwd arm64 3.6.6 [52.9 kB]
Get:139 http://kali.darklab.sh/kali kali-rolling/main arm64 libnghttp2-14 arm64 1.64.0-1 [71.3 kB]
Get:162 http://kali.darklab.sh/kali kali-rolling/main arm64 openssh-client arm64 1:9.9p2-1 [906 kB]
Get:163 http://kali.darklab.sh/kali kali-rolling/main arm64 libproc2-0 arm64 2:4.0.4-7 [62.4 kB]
Get:164 http://kali.darklab.sh/kali kali-rolling/main arm64 procps arm64 2:4.0.4-7 [868 kB]
Get:86 http://kali.download/kali kali-rolling/main arm64 diffutils arm64 1:3.10-2 [378 kB]
Get:172 http://kali.darklab.sh/kali kali-rolling/main arm64 media-types all 13.0.0 [29.3 kB]
Get:174 http://kali.darklab.sh/kali kali-rolling/main arm64 libsqlite3-0 arm64 3.46.1-1 [852 kB]
Get:87 http://kali.download/kali kali-rolling/main arm64 libxxhash0 arm64 0.8.3-2 [22.3 kB]
Get:89 http://kali.download/kali kali-rolling/main arm64 liblzma5 arm64 5.6.4-1 [274 kB]
Get:90 http://kali.download/kali kali-rolling/main arm64 kali-defaults all 2025.1.1 [1,003 kB]
Get:177 http://kali.darklab.sh/kali kali-rolling/main arm64 libpython3-stdlib arm64 3.13.1-2 [9,952 B]
Get:190 http://kali.darklab.sh/kali kali-rolling/main arm64 nano arm64 8.3-1 [635 kB]
Get:94 http://kali.download/kali kali-rolling/main arm64 libudev1 arm64 257.3-1 [141 kB]
Get:199 http://http.kali.org/kali kali-rolling/main arm64 libgpm2 arm64 1.20.7-11+b2 [14.7 kB]
Get:203 http://http.kali.org/kali kali-rolling/main arm64 whiptail arm64 0.52.24-4+b1 [24.5 kB]
Get:98 http://kali.download/kali kali-rolling/main arm64 findutils arm64 4.10.0-3 [696 kB]
Get:205 http://kali.darklab.sh/kali kali-rolling/main arm64 ca-certificates all 20241223 [164 kB]
Get:209 http://kali.darklab.sh/kali kali-rolling/main arm64 abootimg arm64 0.6-2 [14.2 kB]
Get:217 http://kali.darklab.sh/kali kali-rolling/main arm64 binutils arm64 2.44-3 [262 kB]
Get:220 http://kali.darklab.sh/kali kali-rolling/main arm64 libusb-1.0-0 arm64 2:1.0.27-2 [55.4 kB]
Get:222 http://kali.darklab.sh/kali kali-rolling/main arm64 libjaylink0 arm64 0.4.0-1 [23.5 kB]
Get:238 http://kali.darklab.sh/kali kali-rolling/main arm64 libss2 arm64 1.47.2-1 [28.4 kB]
Get:246 http://kali.darklab.sh/kali kali-rolling/main arm64 nethunter-utils arm64 1.6.2 [27.7 kB]
Get:259 http://http.kali.org/kali kali-rolling/main arm64 zstd arm64 1.5.6+dfsg-2 [618 kB]
Get:100 http://kali.download/kali kali-rolling/main arm64 gzip arm64 1.13-1 [135 kB]
Get:101 http://kali.download/kali kali-rolling/main arm64 hostname arm64 3.25 [10.8 kB]
Get:103 http://http.kali.org/kali kali-rolling/main arm64 sed arm64 4.9-2+b1 [326 kB]
Get:105 http://kali.download/kali kali-rolling/main arm64 libnettle8t64 arm64 3.10.1-1 [311 kB]
Get:107 http://http.kali.org/kali kali-rolling/main arm64 sqv arm64 1.2.1-6+b1 [572 kB]
Get:109 http://http.kali.org/kali kali-rolling/main arm64 apt-utils arm64 2.9.29+kali1 [313 kB]
Get:110 http://kali.download/kali kali-rolling/main arm64 libdebconfclient0 arm64 0.277 [10.5 kB]
Get:112 http://http.kali.org/kali kali-rolling/main arm64 init-system-helpers all 1.68+kali2 [40.6 kB]
Get:113 http://http.kali.org/kali kali-rolling/main arm64 ncurses-base all 6.5+20250216-1 [273 kB]
Get:118 http://kali.download/kali kali-rolling/main arm64 logsave arm64 1.47.2-1 [23.8 kB]
Get:119 http://kali.download/kali kali-rolling/main arm64 libext2fs2t64 arm64 1.47.2-1 [204 kB]
Get:122 http://kali.download/kali kali-rolling/main arm64 klibc-utils arm64 2.0.14-1 [102 kB]
Get:124 http://kali.download/kali kali-rolling/main arm64 linux-base all 4.11 [31.2 kB]
Get:125 http://kali.download/kali kali-rolling/main arm64 login.defs all 1:4.17.3-1 [186 kB]
Get:126 http://http.kali.org/kali kali-rolling/main arm64 login arm64 1:4.16.0-2+really2.40.4-2 [86.8 kB]
Get:128 http://http.kali.org/kali kali-rolling/main arm64 init arm64 1.68+kali2 [6,752 B]
Get:130 http://kali.download/kali kali-rolling/main arm64 libunistring5 arm64 1.3-1 [449 kB]
Get:131 http://kali.download/kali kali-rolling/main arm64 libidn2-0 arm64 2.3.8-1 [107 kB]
Get:132 http://kali.download/kali kali-rolling/main arm64 libffi8 arm64 3.4.7-1 [21.2 kB]
Get:133 http://kali.download/kali kali-rolling/main arm64 libp11-kit0 arm64 0.25.5-3 [409 kB]
Get:135 http://kali.download/kali kali-rolling/main arm64 libgnutls30t64 arm64 3.8.9-2 [1,374 kB]
Get:136 http://http.kali.org/kali kali-rolling/main arm64 libsasl2-modules-db arm64 2.1.28+dfsg1-9 [20.1 kB]
Get:137 http://http.kali.org/kali kali-rolling/main arm64 libsasl2-2 arm64 2.1.28+dfsg1-9 [55.6 kB]
Get:138 http://http.kali.org/kali kali-rolling/main arm64 libldap2 arm64 2.6.9+dfsg-1 [179 kB]
Get:141 http://kali.download/kali kali-rolling/main arm64 libngtcp2-16 arm64 1.11.0-1 [121 kB]
Get:142 http://kali.download/kali kali-rolling/main arm64 libngtcp2-crypto-gnutls8 arm64 1.11.0-1 [28.2 kB]
Get:143 http://http.kali.org/kali kali-rolling/main arm64 libpsl5t64 arm64 0.21.2-1.1+b1 [57.1 kB]
Get:145 http://kali.download/kali kali-rolling/main arm64 libssh2-1t64 arm64 1.11.1-1 [235 kB]
Get:147 http://kali.download/kali kali-rolling/main arm64 liberror-perl all 0.17030-1 [26.9 kB]
Get:149 http://kali.download/kali kali-rolling/main arm64 git-man all 1:2.47.2-0.1 [2,205 kB]
Get:7 http://mirrors.jevincanders.net/kali kali-rolling/main arm64 perl-modules-5.40 all 5.40.1-2 [3,017 kB]
Get:151 http://http.kali.org/kali kali-rolling/main arm64 libmd0 arm64 1.1.0-2+b1 [33.7 kB]
Get:153 http://kali.download/kali kali-rolling/main arm64 libsemanage-common all 3.8-1 [7,720 B]
Get:154 http://kali.download/kali kali-rolling/main arm64 libsepol2 arm64 3.8-1 [265 kB]
Get:155 http://http.kali.org/kali kali-rolling/main arm64 libsemanage2 arm64 3.8-1+b1 [87.5 kB]
Get:156 http://kali.download/kali kali-rolling/main arm64 passwd arm64 1:4.17.3-1 [1,205 kB]
Get:12 http://http.kali.org/kali kali-rolling/main arm64 libtext-iconv-perl arm64 1.7-8+b4 [14.2 kB]
Get:16 http://http.kali.org/kali kali-rolling/main arm64 libdb5.3t64 arm64 5.3.28+dfsg2-9 [629 kB]
Get:158 http://kali.download/kali kali-rolling/main arm64 libcbor0.10 arm64 0.10.2-2 [27.4 kB]
Get:159 http://http.kali.org/kali kali-rolling/main arm64 libfido2-1 arm64 1.15.0-1+b1 [74.3 kB]
Get:161 http://kali.download/kali kali-rolling/main arm64 openssh-server arm64 1:9.9p2-1 [475 kB]
Get:165 http://kali.download/kali kali-rolling/main arm64 ucf all 3.0050 [42.7 kB]
Get:166 http://kali.download/kali kali-rolling/main arm64 runit-helper all 2.16.4 [7,296 B]
Get:167 http://kali.download/kali kali-rolling/main arm64 libwrap0 arm64 7.6.q-36 [55.0 kB]
Get:169 http://kali.download/kali kali-rolling/main arm64 python3.13-minimal arm64 3.13.2-1 [1,997 kB]
Get:19 http://http.kali.org/kali kali-rolling/main arm64 zlib1g arm64 1:1.3.dfsg+really1.3.1-1+b1 [85.1 kB]
Get:24 http://http.kali.org/kali kali-rolling/main arm64 libstdc++6 arm64 14.2.0-17 [637 kB]
Get:25 http://mirrors.jevincanders.net/kali kali-rolling/main arm64 openssl-provider-legacy arm64 3.4.1-1 [300 kB]
Get:170 http://kali.download/kali kali-rolling/main arm64 python3-minimal arm64 3.13.1-2 [27.0 kB]
Get:173 http://kali.download/kali kali-rolling/main arm64 tzdata all 2025a-2 [259 kB]
Get:175 http://kali.download/kali kali-rolling/main arm64 libpython3.13-stdlib arm64 3.13.2-1 [1,914 kB]
Get:27 http://http.kali.org/kali kali-rolling/main arm64 libzstd1 arm64 1.5.6+dfsg-2 [261 kB]
Get:28 http://http.kali.org/kali kali-rolling/main arm64 libacl1 arm64 2.3.2-2+b1 [32.2 kB]
Get:176 http://kali.download/kali kali-rolling/main arm64 python3.13 arm64 3.13.2-1 [745 kB]
Get:29 http://mirrors.jevincanders.net/kali kali-rolling/main arm64 libaudit-common all 1:4.0.2-2 [12.7 kB]
Get:30 http://http.kali.org/kali kali-rolling/main arm64 libcap-ng0 arm64 0.8.5-4+b1 [17.0 kB]
Get:178 http://kali.download/kali kali-rolling/main arm64 sudo arm64 1.9.16p2-1 [1,992 kB]
Get:31 http://http.kali.org/kali kali-rolling/main arm64 libaudit1 arm64 1:4.0.2-2+b2 [54.6 kB]
Get:33 http://mirrors.jevincanders.net/kali kali-rolling/main arm64 fdisk arm64 2.40.4-2 [150 kB]
Get:179 http://kali.download/kali kali-rolling/main arm64 libgpg-error0 arm64 1.51-3 [78.5 kB]
Get:180 http://kali.download/kali kali-rolling/main arm64 libgcrypt20 arm64 1.11.0-7 [742 kB]
Get:37 http://mirrors.jevincanders.net/kali kali-rolling/main arm64 util-linux arm64 2.40.4-2 [1,172 kB]
Get:182 http://kali.download/kali kali-rolling/main arm64 mawk arm64 1.3.4.20250131-1 [134 kB]
Get:184 http://kali.download/kali kali-rolling/main arm64 dmidecode arm64 3.6-2 [56.9 kB]
Get:185 http://kali.download/kali kali-rolling/main arm64 iputils-ping arm64 3:20240905-1 [49.4 kB]
Get:186 http://http.kali.org/kali kali-rolling/main arm64 less arm64 643-1+b1 [144 kB]
Get:38 http://mirrors.jevincanders.net/kali kali-rolling/main arm64 libfdisk1 arm64 2.40.4-2 [199 kB]
Get:187 http://kali.download/kali kali-rolling/main arm64 linux-sysctl-defaults all 4.11 [5,244 B]
Get:191 http://http.kali.org/kali kali-rolling/main arm64 libjansson4 arm64 2.14-2+b3 [39.2 kB]
Get:193 http://kali.download/kali kali-rolling/main arm64 nftables arm64 1.1.1-1 [74.6 kB]
Get:194 http://kali.download/kali kali-rolling/main arm64 libnftables1 arm64 1.1.1-1 [304 kB]
Get:196 http://kali.download/kali kali-rolling/main arm64 vim-common all 2:9.1.1113-1 [420 kB]
Get:197 http://kali.download/kali kali-rolling/main arm64 vim-tiny arm64 2:9.1.1113-1 [702 kB]
Get:200 http://http.kali.org/kali kali-rolling/main arm64 libsodium23 arm64 1.0.18-1+b2 [121 kB]
Get:201 http://http.kali.org/kali kali-rolling/main arm64 libslang2 arm64 2.3.3-5+b2 [506 kB]
Get:48 http://http.kali.org/kali kali-rolling/main arm64 libseccomp2 arm64 2.5.5-2+b1 [47.4 kB]
Get:202 http://http.kali.org/kali kali-rolling/main arm64 libnewt0.52 arm64 0.52.24-4+b1 [57.0 kB]
Get:206 http://http.kali.org/kali kali-rolling/main arm64 pci.ids all 0.0~2025.03.09-1 [266 kB]
Get:207 http://kali.download/kali kali-rolling/main arm64 pciutils arm64 1:3.13.0-2 [123 kB]
Get:210 http://http.kali.org/kali kali-rolling/main arm64 apt-transport-https all 2.9.29+kali1 [36.1 kB]
Get:211 http://kali.download/kali kali-rolling/main arm64 libgprofng0 arm64 2.44-3 [668 kB]
Get:212 http://kali.download/kali kali-rolling/main arm64 libctf0 arm64 2.44-3 [84.2 kB]
Get:51 http://mirrors.jevincanders.net/kali kali-rolling/main arm64 ifupdown arm64 0.8.44 [59.4 kB]
Get:214 http://kali.download/kali kali-rolling/main arm64 libsframe1 arm64 2.44-3 [77.8 kB]
Get:215 http://kali.download/kali kali-rolling/main arm64 binutils-aarch64-linux-gnu arm64 2.44-3 [820 kB]
Get:52 http://mirrors.jevincanders.net/kali kali-rolling/main arm64 libsystemd-shared arm64 257.3-1 [1,907 kB]
Get:216 http://kali.download/kali kali-rolling/main arm64 binutils-common arm64 2.44-3 [2,509 kB]
Get:223 http://kali.download/kali kali-rolling/main arm64 flashrom arm64 1.4.0-3 [178 kB]
Get:224 http://http.kali.org/kali kali-rolling/main arm64 cgpt arm64 0~R106-15054.B+dfsg-0.1 [27.2 kB]
Get:225 http://http.kali.org/kali kali-rolling/main arm64 coreboot-utils arm64 24.12+dfsg-2 [258 kB]
Get:226 http://kali.download/kali kali-rolling/main arm64 libjs-sphinxdoc all 8.1.3-5 [30.5 kB]
Get:227 http://http.kali.org/kali kali-rolling/main arm64 sphinx-rtd-theme-common all 3.0.2+dfsg-2 [1,023 kB]
Get:228 http://http.kali.org/kali kali-rolling/main arm64 coreboot-utils-doc all 24.12+dfsg-2 [7,746 kB]
Get:60 http://mirrors.jevincanders.net/kali kali-rolling/main arm64 libkrb5support0 arm64 1.21.3-4 [32.2 kB]
Get:62 http://mirrors.jevincanders.net/kali kali-rolling/main arm64 libcom-err2 arm64 1.47.2-1 [23.9 kB]
Get:79 http://mirrors.jevincanders.net/kali kali-rolling/main arm64 libdbus-1-3 arm64 1.16.2-1 [169 kB]
Get:91 http://mirrors.jevincanders.net/kali kali-rolling/main arm64 kmod arm64 34-3 [89.4 kB]
Get:95 http://http.kali.org/kali kali-rolling/main arm64 libapt-pkg6.0t64 arm64 2.9.29+kali1 [987 kB]
Get:96 http://http.kali.org/kali kali-rolling/main arm64 tar arm64 1.35+dfsg-3.1 [802 kB]
Get:229 http://http.kali.org/kali kali-rolling/main arm64 isc-dhcp-client arm64 4.4.3-P1-5+b2 [1,002 kB]
Get:99 http://http.kali.org/kali kali-rolling/main arm64 grep arm64 3.11-4+b1 [426 kB]
Get:231 http://kali.download/kali kali-rolling/main arm64 javascript-common all 12 [5,236 B]
Get:234 http://http.kali.org/kali kali-rolling/main arm64 libldap-2.5-0 arm64 2.5.19+dfsg-1 [175 kB]
Get:235 http://http.kali.org/kali kali-rolling/main arm64 libldap-common all 2.6.9+dfsg-1 [34.5 kB]
Get:236 http://http.kali.org/kali kali-rolling/main arm64 libnsl2 arm64 1.3.0-3+b3 [37.9 kB]
Get:239 http://kali.download/kali kali-rolling/main arm64 libxau6 arm64 1:1.0.11-1 [20.6 kB]
Get:240 http://kali.download/kali kali-rolling/main arm64 libxdmcp6 arm64 1:1.1.5-1 [27.8 kB]
Get:241 http://http.kali.org/kali kali-rolling/main arm64 libxcb1 arm64 1.17.0-2+b1 [143 kB]
Get:242 http://kali.download/kali kali-rolling/main arm64 libx11-data all 2:1.8.10-2 [337 kB]
Get:106 http://mirrors.jevincanders.net/kali kali-rolling/main arm64 libhogweed6t64 arm64 3.10.1-1 [332 kB]
Get:243 http://kali.download/kali kali-rolling/main arm64 libx11-6 arm64 2:1.8.10-2 [789 kB]
Get:115 http://mirrors.jevincanders.net/kali kali-rolling/main arm64 sysvinit-utils arm64 3.14-3 [33.9 kB]
Get:244 http://http.kali.org/kali kali-rolling/main arm64 libxext6 arm64 2:1.3.4-1+b3 [49.2 kB]
Get:247 http://http.kali.org/kali kali-rolling/main arm64 ntpsec-ntpdate arm64 1.2.3+dfsg1-3+b1 [30.3 kB]
Get:248 http://http.kali.org/kali kali-rolling/main arm64 ntpsec-ntpdig arm64 1.2.3+dfsg1-3+b1 [33.1 kB]
Get:249 http://http.kali.org/kali kali-rolling/main arm64 python3-ntp arm64 1.2.3+dfsg1-3+b1 [96.5 kB]
Get:251 http://kali.download/kali kali-rolling/main arm64 publicsuffix all 20250108.1153-0.1 [292 kB]
Get:129 http://http.kali.org/kali kali-rolling/main arm64 libbrotli1 arm64 1.1.0-2+b7 [308 kB]
Get:255 http://http.kali.org/kali kali-rolling/main arm64 vboot-utils arm64 0~R106-15054.B+dfsg-0.1 [71.4 kB]
Get:144 http://http.kali.org/kali kali-rolling/main arm64 librtmp1 arm64 2.4+20151223.gitfa8646d.1-2+b5 [56.8 kB]
Get:148 http://mirrors.jevincanders.net/kali kali-rolling/main arm64 git arm64 1:2.47.2-0.1 [8,756 kB]
Get:150 http://mirrors.jevincanders.net/kali kali-rolling/main arm64 libattr1 arm64 1:2.5.2-3 [22.7 kB]
Get:152 http://mirrors.jevincanders.net/kali kali-rolling/main arm64 libbsd0 arm64 0.12.2-2 [129 kB]
Get:168 http://mirrors.jevincanders.net/kali kali-rolling/main arm64 libpython3.13-minimal arm64 3.13.2-1 [853 kB]
Get:183 http://mirrors.jevincanders.net/kali kali-rolling/main arm64 cron-daemon-common all 3.0pl1-194 [17.1 kB]
Get:208 http://mirrors.jevincanders.net/kali kali-rolling/main arm64 libpci3 arm64 1:3.13.0-2 [71.8 kB]
Get:213 http://mirrors.jevincanders.net/kali kali-rolling/main arm64 libctf-nobfd0 arm64 2.44-3 [152 kB]
Get:218 http://mirrors.jevincanders.net/kali kali-rolling/main arm64 libbinutils arm64 2.44-3 [660 kB]
Get:219 http://mirrors.jevincanders.net/kali kali-rolling/main arm64 busybox arm64 1:1.37.0-4 [453 kB]
Get:221 http://http.kali.org/kali kali-rolling/main arm64 libftdi1-2 arm64 1.5-8+b1 [30.8 kB]
Get:230 http://http.kali.org/kali kali-rolling/main arm64 isc-dhcp-common arm64 4.4.3-P1-5+b2 [118 kB]
Get:232 http://mirrors.jevincanders.net/kali kali-rolling/main arm64 kbd arm64 2.7.1-2 [333 kB]
Get:252 http://mirrors.jevincanders.net/kali kali-rolling/main arm64 tree arm64 2.2.1-1 [57.9 kB]
Get:253 http://mirrors.jevincanders.net/kali kali-rolling/main arm64 usbutils arm64 1:018-1 [72.9 kB]
Get:257 http://http.kali.org/kali kali-rolling/main arm64 zsh arm64 5.9-8+b5 [845 kB]
Fetched 133 MB in 56s (2,360 kB/s)
Extracting templates from packages: 100%
Preconfiguring packages ...
dpkg: error: requested operation requires superuser privilege
Error: Sub-process /usr/bin/dpkg returned an error code (2)

┌──(/data/data/com.termux/files/kali)─(kali㉿localhost)-[~]
└─$ apt install nmap
Installing:
  nmap

Installing dependencies:
  libblas3  liblinear4  liblua5.4-0  libpcap0.8t64  nmap-common

Suggested packages:
  liblinear-tools  liblinear-dev  ncat  ndiff  zenmap

Summary:
  Upgrading: 0, Installing: 6, Removing: 0, Not Upgrading: 247
  Download size: 6,710 kB
  Space needed: 29.1 MB / 9,175 MB available

Continue? [Y/n] y
Get:1 http://mirror.math.princeton.edu/pub/kali kali-rolling/main arm64 libblas3 arm64 3.12.1-2 [104 kB]
Get:2 http://http.kali.org/kali kali-rolling/main arm64 liblinear4 arm64 2.3.0+dfsg-5+b2 [38.0 kB]
Get:3 http://http.kali.org/kali kali-rolling/main arm64 liblua5.4-0 arm64 5.4.7-1+b2 [134 kB]
Get:4 http://mirrors.ocf.berkeley.edu/kali kali-rolling/main arm64 libpcap0.8t64 arm64 1.10.5-2 [160 kB]
Get:6 http://http.kali.org/kali kali-rolling/non-free arm64 nmap arm64 7.95+dfsg-1kali1 [1,876 kB]
Get:5 http://http.kali.org/kali kali-rolling/non-free arm64 nmap-common all 7.95+dfsg-1kali1 [4,399 kB]
Fetched 6,710 kB in 4s (1,774 kB/s)
dpkg: error: requested operation requires superuser privilege
Error: Sub-process /usr/bin/dpkg returned an error code (2)

┌──(/data/data/com.termux/files/kali)─(kali㉿localhost)-[~]
└─$ nmap -sS -Pn example.com
zsh: command not found: nmap

┌──(/data/data/com.termux/files/kali)─(kali㉿localhost)-[~]
└─$ nh kex &
[1] 12645

┌──(/data/data/com.termux/files/kali)─(kali㉿localhost)-[~]
└─$ zsh: command not found: nh

[1]  + exit 127   nh kex
┌──(/data/data/com.termux/files/kali)─(kali㉿localhost)-[~]
└─$ apt install metasploit-framework
The following packages were automatically installed and are no longer required:
  libldap-2.5-0  libperl5.38t64  perl-modules-5.38
Use 'apt autoremove' to remove them.

Upgrading:
  binutils                    libbz2-1.0     libcurl3t64-gnutls      libsframe1              locales-all
  binutils-aarch64-linux-gnu  libc-bin       libgcc-s1               libssh2-1t64            openssl
  binutils-common             libc-l10n      libgmp10                libssl3t64              perl
  dpkg                        libc6          libgprofng0             libstdc++6              perl-base
  gcc-14-base                 libcrypt1      libldap-common          libtext-charwidth-perl
  gpgv                        libctf-nobfd0  liblocale-gettext-perl  libtext-iconv-perl
  libbinutils                 libctf0        liblzma5                locales

Installing:
  metasploit-framework

Installing dependencies:
  binutils-mingw-w64-i686             libc-dev-bin              make
  binutils-mingw-w64-x86-64           libc6-dev                 manpages
  build-essential                     libcc1-0                  manpages-dev
  bundler                             libcommon-sense-perl      mingw-w64-common
  bzip2                               libcrypt-dev              mingw-w64-i686-dev
  cpp                                 libdpkg-perl              mingw-w64-x86-64-dev
  cpp-14                              libfakeroot               nasm
  cpp-14-aarch64-linux-gnu            libfile-fcntllock-perl    nmap
  cpp-aarch64-linux-gnu               libgcc-14-dev             nmap-common
  curl                                libgmp-dev                openssl-provider-legacy
  dirmngr                             libgmpxx4ldbl             perl-modules-5.40
  dpkg-dev                            libgomp1                  pinentry-curses
  fakeroot                            libhwasan0                postgresql
  g++                                 libicu72                  postgresql-17
  g++-14                              libisl23                  postgresql-client-17
  g++-14-aarch64-linux-gnu            libitm1                   postgresql-client-common
  g++-aarch64-linux-gnu               libjson-perl              postgresql-common
  gcc                                 libjson-xs-perl           rake
  gcc-14                              libksba8                  rpcsvc-proto
  gcc-14-aarch64-linux-gnu            libldap2                  ruby
  gcc-aarch64-linux-gnu               liblinear4                ruby-bundler
  gcc-mingw-w64-base                  libllvm19                 ruby-dev
  gcc-mingw-w64-i686-win32            liblsan0                  ruby-did-you-mean
  gcc-mingw-w64-i686-win32-runtime    liblua5.4-0               ruby-json
  gcc-mingw-w64-x86-64-win32          libmpc3                   ruby-minitest
  gcc-mingw-w64-x86-64-win32-runtime  libmpfr6                  ruby-net-telnet
  gnupg                               libnpth0t64               ruby-power-assert
  gnupg-l10n                          libpcap0.8t64             ruby-rubygems
  gnupg-utils                         libperl5.40               ruby-sdbm
  gpg                                 libpq5                    ruby-test-unit
  gpg-agent                           libruby                   ruby-webrick
  gpg-wks-client                      libruby3.3                ruby-xmlrpc
  gpgconf                             libsensors-config         ruby3.3
  gpgsm                               libsensors5               ruby3.3-dev
  john                                libstdc++-14-dev          ruby3.3-doc
  john-data                           libtsan2                  rubygems-integration
  libalgorithm-diff-perl              libtypes-serialiser-perl  ssl-cert
  libalgorithm-diff-xs-perl           libubsan1                 sysstat
  libalgorithm-merge-perl             libxml2                   unzip
  libasan8                            libxslt1.1                wget
  libassuan9                          libyaml-0-2               xz-utils
  libatomic1                          libz3-4                   zip
  libblas3                            linux-libc-dev

Suggested packages:
  bzip2-doc        automake               scdaemon         lm-sensors            ndiff
  cpp-doc          libtool                wordlist         libstdc++-14-doc      zenmap
  gcc-14-locales   flex                   libc-devtools    make-doc              pinentry-doc
  cpp-14-doc       bison                  glibc-doc        man-browser           postgresql-doc
  pinentry-gnome3  gdb                    bzr              clamav                postgresql-doc-17
  tor              gcc-doc                gmp-doc          clamav-daemon         ri
  debian-keyring   gdb-aarch64-linux-gnu  libgmp10-doc     default-jre-headless  isag
  gcc-14-doc       gpg-wks-server         libmpfr-dev      wine
  gcc-multilib     parcimonie             liblinear-tools  wine64
  autoconf         xloadimage             liblinear-dev    ncat

Summary:
  Upgrading: 32, Installing: 129, Removing: 0, Not Upgrading: 215
  Download size: 508 MB / 557 MB
  Space needed: 2,048 MB / 9,186 MB available

Continue? [Y/n] y
Get:1 http://mirrors.ocf.berkeley.edu/kali kali-rolling/main arm64 libjson-perl all 4.10000-1 [87.5 kB]
Get:2 http://kali.download/kali kali-rolling/main arm64 postgresql-client-common all 264 [36.4 kB]
Get:3 http://kali.darklab.sh/kali kali-rolling/main arm64 ssl-cert all 1.1.3 [16.8 kB]
Get:5 http://kali.download/kali kali-rolling/main arm64 bzip2 arm64 1.0.8-6 [39.5 kB]
Get:6 http://kali.mirror.rafal.ca/kali kali-rolling/main arm64 manpages all 6.9.1-1 [1,393 kB]
Get:7 http://kali.download/kali kali-rolling/main arm64 wget arm64 1.25.0-1 [971 kB]
Get:4 http://kali.darklab.sh/kali kali-rolling/main arm64 postgresql-common all 264 [169 kB]
Get:9 http://http.kali.org/kali kali-rolling/main arm64 binutils-mingw-w64-i686 arm64 2.43.1-5+12 [2,679 kB]
Get:18 http://http.kali.org/kali kali-rolling/main arm64 libmpc3 arm64 1.3.1-1+b3 [50.5 kB]
Get:23 http://kali.darklab.sh/kali kali-rolling/main arm64 libcc1-0 arm64 14.2.0-17 [42.2 kB]
Get:27 http://kali.darklab.sh/kali kali-rolling/main arm64 libasan8 arm64 14.2.0-17 [2,580 kB]
Get:10 http://http.kali.org/kali kali-rolling/main arm64 binutils-mingw-w64-x86-64 arm64 2.43.1-5+12 [3,235 kB]
Get:38 http://http.kali.org/kali kali-rolling/main arm64 g++-14-aarch64-linux-gnu arm64 14.2.0-17 [10.1 MB]
Get:13 http://kali.mirror.rafal.ca/kali kali-rolling/main arm64 libcrypt-dev arm64 1:4.4.38-1 [123 kB]
Get:26 http://kali.mirror.rafal.ca/kali kali-rolling/main arm64 libatomic1 arm64 14.2.0-17 [10.1 kB]
Get:33 http://kali.mirror.rafal.ca/kali kali-rolling/main arm64 gcc-14-aarch64-linux-gnu arm64 14.2.0-17 [17.7 MB]
Get:11 http://kali.download/kali kali-rolling/main arm64 libc-dev-bin arm64 2.40-3 [50.9 kB]
Get:12 http://kali.download/kali kali-rolling/main arm64 linux-libc-dev all 6.12.13-1kali1 [2,515 kB]
Get:41 http://http.kali.org/kali kali-rolling/main arm64 g++ arm64 4:14.2.0-1 [1,332 B]
Get:44 http://http.kali.org/kali kali-rolling/main arm64 dpkg-dev all 1.22.15+kali2 [1,339 kB]
Get:49 http://mirror.math.princeton.edu/pub/kali kali-rolling/main arm64 ruby-minitest all 5.25.4-2 [66.2 kB]
Get:48 http://kali.darklab.sh/kali kali-rolling/main arm64 ruby-did-you-mean all 1.6.3-2 [20.9 kB]
Get:60 http://kali.darklab.sh/kali kali-rolling/main arm64 ruby-rubygems all 3.6.3-1 [406 kB]
Get:14 http://http.kali.org/kali kali-rolling/main arm64 rpcsvc-proto arm64 1.4.3-1+b1 [60.5 kB]
Get:15 http://kali.download/kali kali-rolling/main arm64 libc6-dev arm64 2.40-3 [1,591 kB]
Get:64 http://kali.darklab.sh/kali kali-rolling/main arm64 libassuan9 arm64 3.0.2-2 [59.1 kB]
Get:82 http://http.kali.org/kali kali-rolling/main arm64 gpg-agent arm64 2.2.46-1+b1 [231 kB]
Get:51 http://mirror.math.princeton.edu/pub/kali kali-rolling/main arm64 ruby-power-assert all 2.0.3-1 [11.8 kB]
Get:59 http://http.kali.org/kali kali-rolling/main arm64 ruby arm64 1:3.3+b1 [6,560 B]
Get:90 http://kali.darklab.sh/kali kali-rolling/main arm64 libalgorithm-merge-perl all 0.08-5 [11.8 kB]
Get:93 http://http.kali.org/kali kali-rolling/main arm64 libgmpxx4ldbl arm64 2:6.3.0+dfsg-3 [329 kB]
Get:96 http://kali.darklab.sh/kali kali-rolling/main arm64 libtypes-serialiser-perl all 1.01-1 [12.2 kB]
Get:106 http://kali.darklab.sh/kali kali-rolling/main arm64 nasm arm64 2.16.03-1 [396 kB]
Get:107 http://kali.darklab.sh/kali kali-rolling/main arm64 postgresql-client-17 arm64 17.4-1 [1,985 kB]
Get:16 http://kali.download/kali kali-rolling/main arm64 libisl23 arm64 0.27-1 [601 kB]
Get:17 http://http.kali.org/kali kali-rolling/main arm64 libmpfr6 arm64 4.2.1-1+b2 [680 kB]
Get:19 http://kali.download/kali kali-rolling/main arm64 cpp-14-aarch64-linux-gnu arm64 14.2.0-17 [9,169 kB]
Get:119 http://http.kali.org/kali kali-rolling/main arm64 gnupg-utils arm64 2.2.46-1+b1 [459 kB]
Get:63 http://kali.mirror.rafal.ca/kali kali-rolling/main arm64 curl arm64 8.12.1-3 [256 kB]
Get:66 http://http.kali.org/kali kali-rolling/main arm64 libksba8 arm64 1.6.7-2+b1 [125 kB]
Get:70 http://kali.mirror.rafal.ca/kali kali-rolling/main arm64 fakeroot arm64 1.37-1 [74.9 kB]
Get:94 http://http.kali.org/kali kali-rolling/main arm64 libgmp-dev arm64 2:6.3.0+dfsg-3 [621 kB]
Get:116 http://http.kali.org/kali kali-rolling/main arm64 sysstat arm64 12.7.5-2+b1 [596 kB]
Get:117 http://http.kali.org/kali kali-rolling/main arm64 unzip arm64 6.0-28+b1 [158 kB]
Get:56 http://mirrors.ocf.berkeley.edu/kali kali-rolling/main arm64 libruby3.3 arm64 3.3.7-1 [6,122 kB]
Get:20 http://kali.download/kali kali-rolling/main arm64 cpp-14 arm64 14.2.0-17 [1,280 B]
Get:21 http://kali.download/kali kali-rolling/main arm64 cpp-aarch64-linux-gnu arm64 4:14.2.0-1 [4,832 B]
Get:22 http://kali.download/kali kali-rolling/main arm64 cpp arm64 4:14.2.0-1 [1,568 B]
Get:24 http://kali.download/kali kali-rolling/main arm64 libgomp1 arm64 14.2.0-17 [124 kB]
Get:25 http://kali.download/kali kali-rolling/main arm64 libitm1 arm64 14.2.0-17 [24.2 kB]
Get:28 http://kali.download/kali kali-rolling/main arm64 liblsan0 arm64 14.2.0-17 [1,162 kB]
Get:29 http://kali.download/kali kali-rolling/main arm64 libtsan2 arm64 14.2.0-17 [2,385 kB]
Get:30 http://kali.download/kali kali-rolling/main arm64 libubsan1 arm64 14.2.0-17 [1,039 kB]
Get:31 http://kali.download/kali kali-rolling/main arm64 libhwasan0 arm64 14.2.0-17 [1,443 kB]
Get:35 http://kali.download/kali kali-rolling/main arm64 gcc-aarch64-linux-gnu arm64 4:14.2.0-1 [1,440 B]
Get:36 http://kali.download/kali kali-rolling/main arm64 gcc arm64 4:14.2.0-1 [5,136 B]
Get:37 http://http.kali.org/kali kali-rolling/main arm64 libstdc++-14-dev arm64 14.2.0-17 [2,292 kB]
Get:114 http://http.kali.org/kali kali-rolling/main arm64 ruby-sdbm arm64 1.0.0-5+b7 [14.2 kB]
Get:39 http://http.kali.org/kali kali-rolling/main arm64 g++-14 arm64 14.2.0-17 [22.1 kB]
Get:40 http://http.kali.org/kali kali-rolling/main arm64 g++-aarch64-linux-gnu arm64 4:14.2.0-1 [1,200 B]
Get:42 http://kali.download/kali kali-rolling/main arm64 make arm64 4.4.1-1 [453 kB]
Get:43 http://http.kali.org/kali kali-rolling/main arm64 libdpkg-perl all 1.22.15+kali2 [649 kB]
Get:45 http://kali.download/kali kali-rolling/main arm64 build-essential arm64 12.12 [4,624 B]
Get:46 http://kali.download/kali kali-rolling/main arm64 rubygems-integration all 1.19 [5,488 B]
Get:47 http://kali.download/kali kali-rolling/main arm64 rake all 13.2.1-1 [65.2 kB]
Get:50 http://kali.download/kali kali-rolling/main arm64 ruby-net-telnet all 0.2.0-1 [13.1 kB]
Get:52 http://kali.download/kali kali-rolling/main arm64 ruby-test-unit all 3.6.2-1 [79.1 kB]
Get:53 http://kali.download/kali kali-rolling/main arm64 ruby-webrick all 1.8.1-1 [51.4 kB]
Get:54 http://kali.download/kali kali-rolling/main arm64 ruby-xmlrpc all 0.3.3-2 [24.4 kB]
Get:55 http://kali.download/kali kali-rolling/main arm64 libyaml-0-2 arm64 0.2.5-2 [49.2 kB]
Get:57 http://kali.download/kali kali-rolling/main arm64 ruby3.3 arm64 3.3.7-1 [828 kB]
Get:58 http://http.kali.org/kali kali-rolling/main arm64 libruby arm64 1:3.3+b1 [5,436 B]
Get:61 http://kali.download/kali kali-rolling/main arm64 ruby-bundler all 2.6.3-1 [427 kB]
Get:67 http://kali.download/kali kali-rolling/main arm64 libnpth0t64 arm64 1.8-2 [22.8 kB]
Get:68 http://http.kali.org/kali kali-rolling/main arm64 dirmngr arm64 2.2.46-1+b1 [344 kB]
Get:69 http://kali.download/kali kali-rolling/main arm64 libfakeroot arm64 1.37-1 [29.5 kB]
Get:71 http://http.kali.org/kali kali-rolling/main arm64 gcc-mingw-w64-base arm64 14.2.0-17+27 [194 kB]
Get:72 http://kali.download/kali kali-rolling/main arm64 mingw-w64-common all 12.0.0-5 [5,792 kB]
Get:8 http://mirrors.jevincanders.net/kali kali-rolling/main arm64 xz-utils arm64 5.6.4-1 [553 kB]
Get:32 http://mirrors.jevincanders.net/kali kali-rolling/main arm64 libgcc-14-dev arm64 14.2.0-17 [2,362 kB]
Get:73 http://kali.download/kali kali-rolling/main arm64 mingw-w64-i686-dev all 12.0.0-5 [4,180 kB]
Get:75 http://http.kali.org/kali kali-rolling/main arm64 gcc-mingw-w64-i686-win32 arm64 14.2.0-17+27 [34.1 MB]
Get:34 http://mirrors.jevincanders.net/kali kali-rolling/main arm64 gcc-14 arm64 14.2.0-17 [527 kB]
Get:62 http://mirrors.jevincanders.net/kali kali-rolling/main arm64 bundler all 2.6.3-1 [88.2 kB]
Get:65 http://http.kali.org/kali kali-rolling/main arm64 gpgconf arm64 2.2.46-1+b1 [115 kB]
Get:74 http://http.kali.org/kali kali-rolling/main arm64 gcc-mingw-w64-i686-win32-runtime arm64 14.2.0-17+27 [12.4 MB]
Get:76 http://mirrors.jevincanders.net/kali kali-rolling/main arm64 mingw-w64-x86-64-dev all 12.0.0-5 [4,872 kB]
Get:89 http://http.kali.org/kali kali-rolling/main arm64 libalgorithm-diff-xs-perl arm64 0.04-8+b4 [11.2 kB]
Get:91 http://http.kali.org/kali kali-rolling/main arm64 libcommon-sense-perl arm64 3.75-3+b5 [22.9 kB]
Get:97 http://http.kali.org/kali kali-rolling/main arm64 libjson-xs-perl arm64 4.030-2+b4 [89.5 kB]
Get:104 http://http.kali.org/kali kali-rolling/main arm64 libxslt1.1 arm64 1.1.35-1.1+b1 [222 kB]
Get:110 http://http.kali.org/kali kali-rolling/main arm64 ruby-json arm64 2.9.1+dfsg-1+b1 [60.2 kB]
Get:77 http://http.kali.org/kali kali-rolling/main arm64 gcc-mingw-w64-x86-64-win32-runtime arm64 14.2.0-17+27 [13.2 MB]
Get:78 http://http.kali.org/kali kali-rolling/main arm64 gcc-mingw-w64-x86-64-win32 arm64 14.2.0-17+27 [34.3 MB]
Get:79 http://kali.download/kali kali-rolling/main arm64 gnupg-l10n all 2.2.46-1 [702 kB]
Get:80 http://http.kali.org/kali kali-rolling/main arm64 gpg arm64 2.2.46-1+b1 [481 kB]
Get:81 http://kali.download/kali kali-rolling/main arm64 pinentry-curses arm64 1.3.1-2 [83.5 kB]
Get:83 http://http.kali.org/kali kali-rolling/main arm64 gpgsm arm64 2.2.46-1+b1 [232 kB]
Get:84 http://kali.download/kali kali-rolling/main arm64 gnupg all 2.2.46-1 [376 kB]
Get:85 http://http.kali.org/kali kali-rolling/main arm64 gpg-wks-client arm64 2.2.46-1+b1 [95.1 kB]
Get:86 http://http.kali.org/kali kali-rolling/main arm64 john-data all 1.9.0-Jumbo-1+git20211102-0kali9 [22.8 MB]
Get:87 http://http.kali.org/kali kali-rolling/main arm64 john arm64 1.9.0-Jumbo-1+git20211102-0kali9 [3,950 kB]
Get:88 http://kali.download/kali kali-rolling/main arm64 libalgorithm-diff-perl all 1.201-1 [43.3 kB]
Get:92 http://http.kali.org/kali kali-rolling/main arm64 libfile-fcntllock-perl arm64 0.22-4+b4 [34.6 kB]
Get:95 http://kali.download/kali kali-rolling/main arm64 libicu72 arm64 72.1-6 [9,239 kB]
Get:98 http://http.kali.org/kali kali-rolling/main arm64 libxml2 arm64 2.12.7+dfsg+really2.9.14-0.2+b2 [630 kB]
Get:99 http://kali.download/kali kali-rolling/main arm64 libz3-4 arm64 4.13.3-1 [7,507 kB]
Get:100 http://http.kali.org/kali kali-rolling/main arm64 libllvm19 arm64 1:19.1.7-1+b1 [23.3 MB]
Get:101 http://kali.download/kali kali-rolling/main arm64 libpq5 arm64 17.4-1 [219 kB]
Get:102 http://kali.download/kali kali-rolling/main arm64 libsensors-config all 1:3.6.0-10 [14.6 kB]
Get:103 http://http.kali.org/kali kali-rolling/main arm64 libsensors5 arm64 1:3.6.0-10+b1 [34.3 kB]
Get:105 http://kali.download/kali kali-rolling/main arm64 manpages-dev all 6.9.1-1 [2,122 kB]
Get:108 http://kali.download/kali kali-rolling/main arm64 postgresql-17 arm64 17.4-1 [16.0 MB]
Get:109 http://http.kali.org/kali kali-rolling/main arm64 postgresql all 17+264 [12.2 kB]
Get:111 http://kali.download/kali kali-rolling/main arm64 metasploit-framework arm64 6.4.50-0kali1 [225 MB]
Get:112 http://kali.download/kali kali-rolling/main arm64 ruby3.3-dev arm64 3.3.7-1 [1,038 kB]
Get:113 http://http.kali.org/kali kali-rolling/main arm64 ruby-dev arm64 1:3.3+b1 [5,572 B]
Get:115 http://kali.download/kali kali-rolling/main arm64 ruby3.3-doc all 3.3.7-1 [2,958 kB]
Get:118 http://http.kali.org/kali kali-rolling/main arm64 zip arm64 3.0-14+b1 [227 kB]
Fetched 508 MB in 3min 35s (2,366 kB/s)
Extracting templates from packages: 100%
Preconfiguring packages ...
dpkg: error: requested operation requires superuser privilege
Error: Sub-process /usr/bin/dpkg returned an error code (2)

┌──(/data/data/com.termux/files/kali)─(kali㉿localhost)-[~]
└─$ readthedocs.io
zsh: command not found: readthedocs.io

┌──(/data/data/com.termux/files/kali)─(kali㉿localhost)-[~]
└─$ man {command}
zsh: command not found: man

┌──(/data/data/com.termux/files/kali)─(kali㉿localhost)-[~]
└─$ info {command}
zsh: command not found: info

┌──(/data/data/com.termux/files/kali)─(kali㉿localhost)-[~]
└─$ https://github.com/{owner}/{repo}/wiki
zsh: no such file or directory: https://github.com/{owner}/{repo}/wiki

┌──(/data/data/com.termux/files/kali)─(kali㉿localhost)-[~]
└─$ git init
hint: Using 'master' as the name for the initial branch. This default branch name
hint: is subject to change. To configure the initial branch name to use in all
hint: of your new repositories, which will suppress this warning, call:
hint:
hint:   git config --global init.defaultBranch <name>
hint:
hint: Names commonly chosen instead of 'master' are 'main', 'trunk' and
hint: 'development'. The just-created branch can be renamed via this command:
hint:
hint:   git branch -m <name>
Initialized empty Git repository in /home/kali/.git/

┌──(/data/data/com.termux/files/kali)─(kali㉿localhost)-[~]
└─$ git add .

┌──(/data/data/com.termux/files/kali)─(kali㉿localhost)-[~]
└─$ git commit -m "Add NetHunter findings"
Author identity unknown

*** Please tell me who you are.

Run

  git config --global user.email "you@example.com"
  git config --global user.name "Your Name"

to set your account's default identity.
Omit --global to set the identity only in this repository.

fatal: empty ident name (for <kali@localhost.localdomain>) not allowed

┌──(/data/data/com.termux/files/kali)─(kali㉿localhost)-[~]
└─$ git remote add origin https://github.com/yourusername/your-repo.git

┌──(/data/data/com.termux/files/kali)─(kali㉿localhost)-[~]
└─$ git push -u origin mastergit config --global user standonyourground78@proton.me
error: unknown option `global'
usage: git push [<options>] [<repository> [<refspec>...]]

    -v, --[no-]verbose    be more verbose
    -q, --[no-]quiet      be more quiet
    --[no-]repo <repository>
                          repository
    --[no-]all            push all branches
    --[no-]branches       alias of --all
    --[no-]mirror         mirror all refs
    -d, --[no-]delete     delete refs
    --[no-]tags           push tags (can't be used with --all or --branches or --mirror)
    -n, --[no-]dry-run    dry run
    --[no-]porcelain      machine-readable output
    -f, --[no-]force      force updates
    --[no-]force-with-lease[=<refname>:<expect>]
                          require old value of ref to be at this value
    --[no-]force-if-includes
                          require remote updates to be 
                          locally
    --[no-]recurse-submodules (check|on-demand|no)
                          control recursive pushing of submodules
    --[no-]thin           use thin pack
    --[no-]receive-pack <receive-pack>
                          receive pack program
    --[no-]exec <receive-pack>
                          receive pack program
    -u, --[no-]set-upstream
                          set upstream for git pull/status
    --[no-]progress       force progress reporting
    --[no-]prune          prune locally removed refs
    --no-verify           bypass pre-push hook
    --verify              opposite of --no-verify
    --[no-]follow-tags    push missing but relevant tags
    --[no-]signed[=(yes|no|if-asked)]
                          GPG sign the push
    --[no-]atomic         request atomic transaction on remote side
    -o, --[no-]push-option <server-specific>
                          option to transmit
    -4, --ipv4            use IPv4 addresses only
    -6, --ipv6            use IPv6 addresses only


┌──(/data/data/com.termux/files/kali)─(kali㉿localhost)-[~]
└─$ --[no-]porcelain      machine-readable output
zsh: command not found: --[no-]porcelain

┌──(/data/data/com.termux/files/kali)─(kali㉿localhost)-[~]
└─$ git push --[no-]porcelain      machine-readable output
error: unknown option `[no-]porcelain'
usage: git push [<options>] [<repository> [<refspec>...]]

    -v, --[no-]verbose    be more verbose
    -q, --[no-]quiet      be more quiet
    --[no-]repo <repository>
                          repository
    --[no-]all            push all branches
    --[no-]branches       alias of --all
    --[no-]mirror         mirror all refs
    -d, --[no-]delete     delete refs
    --[no-]tags           push tags (can't be used with --all or --branches or --mirror)
    -n, --[no-]dry-run    dry run
    --[no-]porcelain      machine-readable output
    -f, --[no-]force      force updates
    --[no-]force-with-lease[=<refname>:<expect>]
                          require old value of ref to be at this value
    --[no-]force-if-includes
                          require remote updates to be integrated locally
    --[no-]recurse-submodules (check|on-demand|no)
                          control recursive pushing of submodules
    --[no-]thin           use thin pack
    --[no-]receive-pack <receive-pack>
                          receive pack program
    --[no-]exec <receive-pack>
                          receive pack program
    -u, --[no-]set-upstream
                          set upstream for git pull/status
    --[no-]progress       force progress reporting
    --[no-]prune          prune locally removed refs
    --no-verify           bypass pre-push hook
    --verify              opposite of --no-verify
    --[no-]follow-tags    push missing but relevant tags
    --[no-]signed[=(yes|no|if-asked)]
                          GPG sign the push
    --[no-]atomic         request atomic transaction on remote side
    -o, --[no-]push-option <server-specific>
                          option to transmit
    -4, --ipv4            use IPv4 addresses only
    -6, --ipv6            use IPv6 addresses only


┌──(/data/data/com.termux/files/kali)─(kali㉿localhost)-[~]
└─$ machine-readable output
zsh: command not found: machine-readable

┌──(/data/data/com.termux/files/kali)─(kali㉿localhost)-[~]
└─$# Net
