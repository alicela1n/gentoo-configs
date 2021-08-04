# Inspiron 3537 (violet-matrix)

Configs for the Dell Inspiron 3537, hostname violet-matrix.

lspci -v
```
00:00.0 Host bridge: Intel Corporation Haswell-ULT DRAM Controller (rev 09)
00:02.0 VGA compatible controller: Intel Corporation Haswell-ULT Integrated Graphics Controller (rev 09)
00:03.0 Audio device: Intel Corporation Haswell-ULT HD Audio Controller (rev 09)
00:14.0 USB controller: Intel Corporation 8 Series USB xHCI HC (rev 04)
00:16.0 Communication controller: Intel Corporation 8 Series HECI #0 (rev 04)
00:1b.0 Audio device: Intel Corporation 8 Series HD Audio Controller (rev 04)
00:1c.0 PCI bridge: Intel Corporation 8 Series PCI Express Root Port 3 (rev e4)
00:1c.3 PCI bridge: Intel Corporation 8 Series PCI Express Root Port 4 (rev e4)
00:1d.0 USB controller: Intel Corporation 8 Series USB EHCI #1 (rev 04)
00:1f.0 ISA bridge: Intel Corporation 8 Series LPC Controller (rev 04)
00:1f.2 SATA controller: Intel Corporation 8 Series SATA Controller 1 [AHCI mode] (rev 04)
00:1f.3 SMBus: Intel Corporation 8 Series SMBus Controller (rev 04)
01:00.0 Ethernet controller: Realtek Semiconductor Co., Ltd. RTL810xE PCI Express Fast Ethernet controller (rev 07)
02:00.0 Network controller: Qualcomm Atheros AR9485 Wireless Network Adapter (rev 01)
```

lscpu
```
Architecture:                    x86_64
CPU op-mode(s):                  32-bit, 64-bit
Byte Order:                      Little Endian
Address sizes:                   39 bits physical, 48 bits virtual
CPU(s):                          4
On-line CPU(s) list:             0-3
Thread(s) per core:              2
Core(s) per socket:              2
Socket(s):                       1
NUMA node(s):                    1
Vendor ID:                       GenuineIntel
CPU family:                      6
Model:                           69
Model name:                      Intel(R) Core(TM) i3-4010U CPU @ 1.70GHz
Stepping:                        1
CPU MHz:                         1696.166
CPU max MHz:                     1700.0000
CPU min MHz:                     800.0000
BogoMIPS:                        3393.68
Virtualization:                  VT-x
L1d cache:                       64 KiB
L1i cache:                       64 KiB
L2 cache:                        512 KiB
L3 cache:                        3 MiB
NUMA node0 CPU(s):               0-3
Vulnerability Itlb multihit:     KVM: Mitigation: VMX disabled
Vulnerability L1tf:              Mitigation; PTE Inversion; VMX conditional cache flushes, SMT vulnerable
Vulnerability Mds:               Mitigation; Clear CPU buffers; SMT vulnerable
Vulnerability Meltdown:          Mitigation; PTI
Vulnerability Spec store bypass: Mitigation; Speculative Store Bypass disabled via prctl and seccomp
Vulnerability Spectre v1:        Mitigation; usercopy/swapgs barriers and __user pointer sanitization
Vulnerability Spectre v2:        Mitigation; Full generic retpoline, IBPB conditional, IBRS_FW, STIBP conditional, RSB filling
Vulnerability Srbds:             Mitigation; Microcode
Vulnerability Tsx async abort:   Not affected
Flags:                           fpu vme de pse tsc msr pae mce cx8 apic sep mtrr pge mca cmov pat pse36 clflush dts acpi mmx fxsr sse sse2 ss ht tm
                                  pbe syscall nx pdpe1gb rdtscp lm constant_tsc arch_perfmon pebs bts rep_good nopl xtopology nonstop_tsc cpuid aper
                                 fmperf pni pclmulqdq dtes64 monitor ds_cpl vmx est tm2 ssse3 sdbg fma cx16 xtpr pdcm pcid sse4_1 sse4_2 x2apic movb
                                 e popcnt tsc_deadline_timer aes xsave avx f16c rdrand lahf_lm abm cpuid_fault epb invpcid_single pti ssbd ibrs ibpb
                                  stibp tpr_shadow vnmi flexpriority ept vpid ept_ad fsgsbase tsc_adjust bmi1 avx2 smep bmi2 erms invpcid xsaveopt d
                                 therm ida arat pln pts md_clear flush_l1d
```

emerge --info
```
Portage 3.0.20 (python 3.9.6-final-0, default/linux/amd64/17.1/desktop/plasma, gcc-10.3.0, glibc-2.33-r1, 5.10.52-gentoo-x86_64 x86_64)
=================================================================
System uname: Linux-5.10.52-gentoo-x86_64-x86_64-Intel-R-_Core-TM-_i3-4010U_CPU_@_1.70GHz-with-glibc2.33
KiB Mem:     8026364 total,   2203532 free
KiB Swap:    7812496 total,   7799164 free
Timestamp of repository gentoo: Wed, 04 Aug 2021 03:30:01 +0000
Head commit of repository gentoo: 6e17560f8922f9b12c3184946b691cb016e58667
Head commit of repository alicela1ns-overlay: 9c13622a6ff1ca13e95f74809a7e9942144fd811

sh bash 5.1_p8
ld GNU ld (Gentoo 2.35.2 p1) 2.35.2
distcc 3.4 x86_64-pc-linux-gnu [disabled]
ccache version 4.3 [disabled]
app-shells/bash:          5.1_p8::gentoo
dev-lang/perl:            5.34.0::gentoo
dev-lang/python:          3.8.11::gentoo, 3.9.6::gentoo
dev-lang/rust:            1.53.0::gentoo
dev-util/ccache:          4.3-r2::gentoo
dev-util/cmake:           3.18.5::gentoo
sys-apps/baselayout:      2.7::gentoo
sys-apps/openrc:          0.42.1-r1::gentoo
sys-apps/sandbox:         2.24::gentoo
sys-devel/autoconf:       2.13-r1::gentoo, 2.69-r5::gentoo
sys-devel/automake:       1.16.3-r1::gentoo
sys-devel/binutils:       2.35.2::gentoo
sys-devel/gcc:            10.3.0-r2::gentoo
sys-devel/gcc-config:     2.4::gentoo
sys-devel/libtool:        2.4.6-r6::gentoo
sys-devel/make:           4.3::gentoo
sys-kernel/linux-headers: 5.10::gentoo (virtual/os-headers)
sys-libs/glibc:           2.33-r1::gentoo
Repositories:

gentoo
    location: /var/db/repos/gentoo
    sync-type: rsync
    sync-uri: rsync://rsync.gentoo.org/gentoo-portage
    priority: -1000
    sync-rsync-verify-max-age: 24
    sync-rsync-verify-jobs: 1
    sync-rsync-verify-metamanifest: yes
    sync-rsync-extra-opts:

alicela1ns-overlay
    location: /var/db/repos/alicela1ns-overlay
    sync-type: git
    sync-uri: https://github.com/alicela1n/alicela1n-gentoo-overlay.git
    masters: gentoo

localrepo
    location: /var/db/repos/localrepo
    masters: gentoo

ACCEPT_KEYWORDS="amd64"
ACCEPT_LICENSE="* -@EULA"
CBUILD="x86_64-pc-linux-gnu"
CFLAGS="-march=haswell -O2 -pipe"
CHOST="x86_64-pc-linux-gnu"
CONFIG_PROTECT="/etc /usr/share/config /usr/share/gnupg/qualified.txt"
CONFIG_PROTECT_MASK="/etc/ca-certificates.conf /etc/dconf /etc/env.d /etc/fonts/fonts.conf /etc/gconf /etc/gentoo-release /etc/revdep-rebuild /etc/sandbox.d /etc/terminfo /etc/texmf/language.dat.d /etc/texmf/language.def.d /etc/texmf/updmap.d /etc/texmf/web2c"
CXXFLAGS="-march=haswell -O2 -pipe"
DISTDIR="/var/cache/distfiles"
EMERGE_DEFAULT_OPTS=" --jobs 4 --usepkg-exclude 'sys-kernel/gentoo-sources virtual/*'"
ENV_UNSET="CARGO_HOME DBUS_SESSION_BUS_ADDRESS DISPLAY GOBIN GOPATH PERL5LIB PERL5OPT PERLPREFIX PERL_CORE PERL_MB_OPT PERL_MM_OPT XAUTHORITY XDG_CACHE_HOME XDG_CONFIG_HOME XDG_DATA_HOME XDG_RUNTIME_DIR"
FCFLAGS="-march=haswell -O2 -pipe"
FEATURES="assume-digests binpkg-docompress binpkg-dostrip binpkg-logs config-protect-if-modified distlocks ebuild-locks fixlafiles ipc-sandbox merge-sync multilib-strict network-sandbox news parallel-fetch pid-sandbox preserve-libs protect-owned qa-unresolved-soname-deps sandbox sfperms strict unknown-features-warn unmerge-logs unmerge-orphans userfetch userpriv usersandbox usersync xattr"
FFLAGS="-march=haswell -O2 -pipe"
GENTOO_MIRRORS="https://mirrors.advancedhosters.com/gentoo/ http://gentoo.mirrors.easynews.com/linux/gentoo/ http://mirrors.rit.edu/gentoo/ http://www.gtlib.gatech.edu/pub/gentoo"
LANG="en_US.UTF-8"
LDFLAGS="-Wl,-O1 -Wl,--as-needed"
MAKEOPTS="-j3"
PKGDIR="/var/cache/binpkgs"
PORTAGE_CONFIGROOT="/"
PORTAGE_RSYNC_OPTS="--recursive --links --safe-links --perms --times --omit-dir-times --compress --force --whole-file --delete --stats --human-readable --timeout=180 --exclude=/distfiles --exclude=/local --exclude=/packages --exclude=/.git"
PORTAGE_TMPDIR="/var/tmp"
USE="X Xvaapi a52 aac acl acpi activities alsa amd64 avahi bluetooth branding bzip2 cairo cdda cdr cli crypt cups dbus declarative dri dts dvd dvdr elogind emboss encode exif flac fortran gdbm gif gphoto2 gpm gtk gui iconv icu ios ipv6 jpeg kde kipi kwallet lcms libglvnd libnotify libtirpc mad mng mp3 mp4 mpeg multilib ncurses networkmanager nls nptl ogg opengl openmp pam pango pcre pdf phonon plasma png policykit ppds pulseaudio qml qt5 readline sdl seccomp semantic-desktop sound spell split-usr ssl startup-notification svg tcpd tiff truetype udev udisks unicode upower usb vim-syntax vorbis widgets wxwidgets x264 xattr xcb xinerama xml xv xvid zlib zsh-completion" ABI_X86="64" ADA_TARGET="gnat_2021" ALSA_CARDS="ali5451 als4000 atiixp atiixp-modem bt87x ca0106 cmipci emu10k1x ens1370 ens1371 es1938 es1968 fm801 hda-intel intel8x0 intel8x0m maestro3 trident usb-audio via82xx via82xx-modem ymfpci" APACHE2_MODULES="authn_core authz_core socache_shmcb unixd actions alias auth_basic authn_alias authn_anon authn_dbm authn_default authn_file authz_dbm authz_default authz_groupfile authz_host authz_owner authz_user autoindex cache cgi cgid dav dav_fs dav_lock deflate dir disk_cache env expires ext_filter file_cache filter headers include info log_config logio mem_cache mime mime_magic negotiation rewrite setenvif speling status unique_id userdir usertrack vhost_alias" CALLIGRA_FEATURES="karbon sheets words" COLLECTD_PLUGINS="df interface irq load memory rrdtool swap syslog" CPU_FLAGS_X86="aes avx avx2 f16c fma3 mmx mmxext pclmul popcnt rdrand sse sse2 sse3 sse4_1 sse4_2 ssse3" ELIBC="glibc" GPSD_PROTOCOLS="ashtech aivdm earthmate evermore fv18 garmin garmintxt gpsclock greis isync itrax mtk3301 nmea ntrip navcom oceanserver oldstyle oncore rtcm104v2 rtcm104v3 sirf skytraq superstar2 timing tsip tripmate tnt ublox ubx" GRUB_PLATFORMS="efi-64 pc" INPUT_DEVICES="synaptics libinput" KERNEL="linux" L10N="en en-US" LCD_DEVICES="bayrad cfontz cfontz633 glk hd44780 lb216 lcdm001 mtxorb ncurses text" LIBREOFFICE_EXTENSIONS="presenter-console presenter-minimizer" LUA_SINGLE_TARGET="lua5-1" LUA_TARGETS="lua5-1" OFFICE_IMPLEMENTATION="libreoffice" PHP_TARGETS="php7-3 php7-4" POSTGRES_TARGETS="postgres12 postgres13" PYTHON_SINGLE_TARGET="python3_9" PYTHON_TARGETS="python3_9" QEMU_SOFTMMU_TARGETS="arm aarch64 alpha i386 x86_64 sparc sparc64 ppc ppc64 riscv32 riscv64 mipsel mips64el mips mips64" QEMU_USER_TARGETS="x86_64 i386 aarch64 arm" RUBY_TARGETS="ruby26" USERLAND="GNU" VIDEO_CARDS="intel" XTABLES_ADDONS="quota2 psd pknock lscan length2 ipv4options ipset ipp2p iface geoip fuzzy condition tee tarpit sysrq proto steal rawnat logmark ipmark dhcpmac delude chaos account"
Unset:  CC, CPPFLAGS, CTARGET, CXX, INSTALL_MASK, LC_ALL, LINGUAS, PORTAGE_BINHOST, PORTAGE_BUNZIP2_COMMAND, PORTAGE_COMPRESS, PORTAGE_COMPRESS_FLAGS, PORTAGE_RSYNC_EXTRA_OPTS, RUSTFLAGS
```

inxi -F
```
System:    Host: violet-matrix Kernel: 5.10.52-gentoo-x86_64 x86_64 bits: 64 Desktop: KDE Plasma 5.21.5 
           Distro: Gentoo Base System release 2.7 
Machine:   Type: Portable System: Dell product: Inspiron 3537 v: A11 serial: <superuser/root required> 
           Mobo: Dell model: 0MJNYC v: A00 serial: <superuser/root required> UEFI: Dell v: A11 date: 07/30/2018 
Battery:   ID-1: BAT1 charge: 14.3 Wh condition: 31.1/41.4 Wh (75%) 
CPU:       Info: Dual Core model: Intel Core i3-4010U bits: 64 type: MT MCP L2 cache: 3072 KiB 
           Speed: 1696 MHz min/max: 800/1700 MHz Core speeds (MHz): 1: 1696 2: 1696 3: 1696 4: 1697 
Graphics:  Device-1: Intel Haswell-ULT Integrated Graphics driver: i915 v: kernel 
           Device-2: Microdia Dell Laptop Integrated Webcam HD type: USB driver: uvcvideo 
           Display: x11 server: X.org 1.20.11 driver: intel unloaded: modesetting resolution: <xdpyinfo missing> 
           OpenGL: renderer: Mesa DRI Intel HD Graphics 4400 (HSW GT2) v: 4.5 Mesa 21.1.4 
Audio:     Device-1: Intel Haswell-ULT HD Audio driver: snd_hda_intel 
           Device-2: Intel 8 Series HD Audio driver: snd_hda_intel 
           Sound Server: ALSA v: k5.10.52-gentoo-x86_64 
Network:   Device-1: Realtek RTL810xE PCI Express Fast Ethernet driver: r8169 
           IF: enp1s0 state: down mac: <redacted> 
           Device-2: Qualcomm Atheros AR9485 Wireless Network Adapter driver: ath9k 
           IF: wlp2s0 state: up mac: <redacted>
Drives:    Local Storage: total: 232.89 GiB used: 58.74 GiB (25.2%) 
           ID-1: /dev/sda vendor: Western Digital model: WDBNCE2500PNC size: 232.89 GiB 
Partition: ID-1: / size: 227.67 GiB used: 58.63 GiB (25.8%) fs: ext4 dev: /dev/dm-0 
           ID-2: /boot size: 499.0 MiB used: 113.5 MiB (22.8%) fs: vfat dev: /dev/sda1 
Swap:      ID-1: swap-1 type: file size: 7.45 GiB used: 13.0 MiB (0.2%) file: /swapfile 
Sensors:   Missing: Required tool sensors not installed. Check --recommends 
Info:      Processes: 207 Uptime: 2d 2h 12m Memory: 7.65 GiB used: 2.67 GiB (34.9%) Shell: Zsh inxi: 3.1.06
```
