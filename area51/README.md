# Alienware 14 (area51)

Configs for Alienware 14, hostname area51

lspci
```
00:00.0 Host bridge: Intel Corporation Xeon E3-1200 v3/4th Gen Core Processor DRAM Controller (rev 06)
00:01.0 PCI bridge: Intel Corporation Xeon E3-1200 v3/4th Gen Core Processor PCI Express x16 Controller (rev 06)
00:02.0 VGA compatible controller: Intel Corporation 4th Gen Core Processor Integrated Graphics Controller (rev 06)
00:03.0 Audio device: Intel Corporation Xeon E3-1200 v3/4th Gen Core Processor HD Audio Controller (rev 06)
00:14.0 USB controller: Intel Corporation 8 Series/C220 Series Chipset Family USB xHCI (rev 04)
00:16.0 Communication controller: Intel Corporation 8 Series/C220 Series Chipset Family MEI Controller #1 (rev 04)
00:1a.0 USB controller: Intel Corporation 8 Series/C220 Series Chipset Family USB EHCI #2 (rev 04)
00:1b.0 Audio device: Intel Corporation 8 Series/C220 Series Chipset High Definition Audio Controller (rev 04)
00:1c.0 PCI bridge: Intel Corporation 8 Series/C220 Series Chipset Family PCI Express Root Port #1 (rev d4)
00:1c.2 PCI bridge: Intel Corporation 8 Series/C220 Series Chipset Family PCI Express Root Port #3 (rev d4)
00:1c.3 PCI bridge: Intel Corporation 8 Series/C220 Series Chipset Family PCI Express Root Port #4 (rev d4)
00:1c.4 PCI bridge: Intel Corporation 8 Series/C220 Series Chipset Family PCI Express Root Port #5 (rev d4)
00:1d.0 USB controller: Intel Corporation 8 Series/C220 Series Chipset Family USB EHCI #1 (rev 04)
00:1f.0 ISA bridge: Intel Corporation HM87 Express LPC Controller (rev 04)
00:1f.2 RAID bus controller: Intel Corporation 82801 Mobile SATA Controller [RAID mode] (rev 04)
00:1f.3 SMBus: Intel Corporation 8 Series/C220 Series Chipset Family SMBus Controller (rev 04)
01:00.0 VGA compatible controller: NVIDIA Corporation GK107M [GeForce GT 750M] (rev a1)
01:00.1 Audio device: NVIDIA Corporation GK107 HDMI Audio Controller (rev a1)
08:00.0 Ethernet controller: Qualcomm Atheros Killer E220x Gigabit Ethernet Controller (rev 10)
09:00.0 Unassigned class [ff00]: Realtek Semiconductor Co., Ltd. RTS5209 PCI Express Card Reader (rev 01)
09:00.1 SD Host controller: Realtek Semiconductor Co., Ltd. RTS5209 PCI Express Card Reader (rev 01)
0a:00.0 Network controller: Qualcomm Atheros AR9462 Wireless Network Adapter (rev 01)
```

lscpu
```
Architecture:                    x86_64
CPU op-mode(s):                  32-bit, 64-bit
Byte Order:                      Little Endian
Address sizes:                   39 bits physical, 48 bits virtual
CPU(s):                          8
On-line CPU(s) list:             0-7
Thread(s) per core:              2
Core(s) per socket:              4
Socket(s):                       1
NUMA node(s):                    1
Vendor ID:                       GenuineIntel
CPU family:                      6
Model:                           60
Model name:                      Intel(R) Core(TM) i7-4700MQ CPU @ 2.40GHz
Stepping:                        3
CPU MHz:                         2624.515
CPU max MHz:                     3400.0000
CPU min MHz:                     800.0000
BogoMIPS:                        4790.41
Virtualization:                  VT-x
L1d cache:                       128 KiB
L1i cache:                       128 KiB
L2 cache:                        1 MiB
L3 cache:                        6 MiB
NUMA node0 CPU(s):               0-7
Vulnerability Itlb multihit:     KVM: Mitigation: VMX disabled
Vulnerability L1tf:              Mitigation; PTE Inversion; VMX conditional cache flushes, SMT vulnerable
Vulnerability Mds:               Mitigation; Clear CPU buffers; SMT vulnerable
Vulnerability Meltdown:          Mitigation; PTI
Vulnerability Spec store bypass: Mitigation; Speculative Store Bypass disabled via prctl and seccomp
Vulnerability Spectre v1:        Mitigation; usercopy/swapgs barriers and __user pointer sanitization
Vulnerability Spectre v2:        Mitigation; Full generic retpoline, IBPB conditional, IBRS_FW, STIBP conditional, RSB filling
Vulnerability Srbds:             Vulnerable: No microcode
Vulnerability Tsx async abort:   Not affected
Flags:                           fpu vme de pse tsc msr pae mce cx8 apic sep mtrr pge mca cmov pat pse36 clflush dts acpi mmx fxsr sse sse2 ss ht tm pbe syscall nx pdp
                                 e1gb rdtscp lm constant_tsc arch_perfmon pebs bts rep_good nopl xtopology nonstop_tsc cpuid aperfmperf pni pclmulqdq dtes64 monitor ds
                                 _cpl vmx est tm2 ssse3 sdbg fma cx16 xtpr pdcm pcid sse4_1 sse4_2 movbe popcnt tsc_deadline_timer aes xsave avx f16c rdrand lahf_lm ab
                                 m cpuid_fault epb invpcid_single pti ssbd ibrs ibpb stibp tpr_shadow vnmi flexpriority ept vpid ept_ad fsgsbase tsc_adjust bmi1 avx2 s
                                 mep bmi2 erms invpcid xsaveopt dtherm ida arat pln pts md_clear flush_l1d
```

emerge --info
```
Portage 3.0.20 (python 3.9.6-final-0, default/linux/amd64/17.1/desktop/plasma/systemd, gcc-10.3.1, glibc-2.33-r1, 5.10.52-gentoo-dist x86_64)
=================================================================
System uname: Linux-5.10.52-gentoo-dist-x86_64-Intel-R-_Core-TM-_i7-4700MQ_CPU_@_2.40GHz-with-glibc2.33
KiB Mem:     8026904 total,   5478748 free
KiB Swap:   19531244 total,  19531244 free
Timestamp of repository gentoo: Sat, 14 Aug 2021 06:00:01 +0000
Head commit of repository gentoo: baa4781e4a30a955ef9ba8f5d24493cbddd3c517
Head commit of repository alicela1ns-overlay: b67f5d7db85b3ab6804df6acd893825e063c7f75

sh bash 5.1_p8
ld GNU ld (Gentoo 2.35.2 p1) 2.35.2
distcc 3.4 x86_64-pc-linux-gnu [disabled]
ccache version 4.3 [disabled]
app-shells/bash:          5.1_p8::gentoo
dev-java/java-config:     2.3.1::gentoo
dev-lang/perl:            5.34.0::gentoo
dev-lang/python:          2.7.18_p11::gentoo, 3.9.6_p1::gentoo
dev-lang/rust:            1.53.0::gentoo
dev-util/ccache:          4.3-r2::gentoo
dev-util/cmake:           3.20.5::gentoo
sys-apps/baselayout:      2.7::gentoo
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
    sync-rsync-verify-metamanifest: yes
    sync-rsync-verify-max-age: 24
    sync-rsync-extra-opts:
    sync-rsync-verify-jobs: 1

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
CFLAGS="-O2 -march=haswell -pipe"
CHOST="x86_64-pc-linux-gnu"
CONFIG_PROTECT="/etc /usr/share/config /usr/share/gnupg/qualified.txt"
CONFIG_PROTECT_MASK="/etc/ca-certificates.conf /etc/dconf /etc/env.d /etc/fonts/fonts.conf /etc/gconf /etc/gentoo-release /etc/php/apache2-php7.4/ext-active/ /etc/php/cgi-php7.4/ext-active/ /etc/php/cli-php7.4/ext-active/ /etc/revdep-rebuild /etc/sandbox.d /etc/terminfo /etc/texmf/language.dat.d /etc/texmf/language.def.d /etc/texmf/updmap.d /etc/texmf/web2c"
CXXFLAGS="-O2 -march=haswell -pipe"
DISTDIR="/var/cache/distfiles"
EMERGE_DEFAULT_OPTS=" --jobs 4"
ENV_UNSET="CARGO_HOME DBUS_SESSION_BUS_ADDRESS DISPLAY GOBIN GOPATH PERL5LIB PERL5OPT PERLPREFIX PERL_CORE PERL_MB_OPT PERL_MM_OPT XAUTHORITY XDG_CACHE_HOME XDG_CONFIG_HOME XDG_DATA_HOME XDG_RUNTIME_DIR"
FCFLAGS="-O2 -march=haswell -pipe"
FEATURES="assume-digests binpkg-docompress binpkg-dostrip binpkg-logs config-protect-if-modified distlocks ebuild-locks fixlafiles ipc-sandbox merge-sync multilib-strict network-sandbox news parallel-fetch pid-sandbox preserve-libs protect-owned qa-unresolved-soname-deps sandbox sfperms strict unknown-features-warn unmerge-logs unmerge-orphans userfetch userpriv usersandbox usersync xattr"
FFLAGS="-O2 -march=haswell -pipe"
GENTOO_MIRRORS="http://distfiles.gentoo.org"
LANG="en_US.UTF-8"
LDFLAGS="-Wl,-O1 -Wl,--as-needed"
MAKEOPTS="-j5"
PKGDIR="/var/cache/binpkgs"
PORTAGE_CONFIGROOT="/"
PORTAGE_RSYNC_OPTS="--recursive --links --safe-links --perms --times --omit-dir-times --compress --force --whole-file --delete --stats --human-readable --timeout=180 --exclude=/distfiles --exclude=/local --exclude=/packages --exclude=/.git"
PORTAGE_TMPDIR="/var/tmp"
USE="X Xvaapi a52 aac acl acpi activities alsa amd64 avahi bluetooth branding bzip2 cairo cdda cdr cli crypt cups dbus declarative dri dts dvd dvdr emboss encode exif flac fortran gdbm gif gphoto2 gpm gtk gui iconv icu ios ipv6 jpeg kde kipi kwallet lcms libglvnd libnotify libtirpc mad mng mp3 mp4 mpeg multilib ncurses networkmanager nls nptl ogg opengl openmp pam pango pcre pdf phonon plasma png policykit ppds pulseaudio qml qt5 readline sdl seccomp semantic-desktop sound spell split-usr ssl startup-notification svg systemd tcpd tiff truetype udev udisks unicode upower usb vim-syntax vorbis widgets wxwidgets x264 xattr xcb xinerama xml xv xvid zlib zsh-completion" ABI_X86="32 64" ADA_TARGET="gnat_2018" ALSA_CARDS="ali5451 als4000 atiixp atiixp-modem bt87x ca0106 cmipci emu10k1x ens1370 ens1371 es1938 es1968 fm801 hda-intel intel8x0 intel8x0m maestro3 trident usb-audio via82xx via82xx-modem ymfpci" APACHE2_MODULES="authn_core authz_core socache_shmcb unixd actions alias auth_basic authn_alias authn_anon authn_dbm authn_default authn_file authz_dbm authz_default authz_groupfile authz_host authz_owner authz_user autoindex cache cgi cgid dav dav_fs dav_lock deflate dir disk_cache env expires ext_filter file_cache filter headers include info log_config logio mem_cache mime mime_magic negotiation rewrite setenvif speling status unique_id userdir usertrack vhost_alias" CALLIGRA_FEATURES="karbon sheets words" COLLECTD_PLUGINS="df interface irq load memory rrdtool swap syslog" CPU_FLAGS_X86="aes avx avx2 f16c fma3 mmx mmxext pclmul popcnt rdrand sse sse2 sse3 sse4_1 sse4_2 ssse3" ELIBC="glibc" GPSD_PROTOCOLS="ashtech aivdm earthmate evermore fv18 garmin garmintxt gpsclock greis isync itrax mtk3301 nmea ntrip navcom oceanserver oldstyle oncore rtcm104v2 rtcm104v3 sirf skytraq superstar2 timing tsip tripmate tnt ublox ubx" INPUT_DEVICES="evdev libinput" KERNEL="linux" LCD_DEVICES="bayrad cfontz cfontz633 glk hd44780 lb216 lcdm001 mtxorb ncurses text" LIBREOFFICE_EXTENSIONS="presenter-console presenter-minimizer" LUA_SINGLE_TARGET="lua5-1" LUA_TARGETS="lua5-1" OFFICE_IMPLEMENTATION="libreoffice" PHP_TARGETS="php7-3 php7-4" POSTGRES_TARGETS="postgres12 postgres13" PYTHON_SINGLE_TARGET="python3_9" PYTHON_TARGETS="python3_9" QEMU_SOFTMMU_TARGETS="arm aarch64 alpha i386 x86_64 sparc sparc64 ppc ppc64 riscv32 riscv64 mipsel mips64el mips mips64" QEMU_USER_TARGETS="x86_64 i386 aarch64 arm" RUBY_TARGETS="ruby26" USERLAND="GNU" VIDEO_CARDS="intel i965 nvidia" XTABLES_ADDONS="quota2 psd pknock lscan length2 ipv4options ipset ipp2p iface geoip fuzzy condition tee tarpit sysrq proto steal rawnat logmark ipmark dhcpmac delude chaos account"
Unset:  CC, CPPFLAGS, CTARGET, CXX, INSTALL_MASK, LC_ALL, LINGUAS, PORTAGE_BINHOST, PORTAGE_BUNZIP2_COMMAND, PORTAGE_COMPRESS, PORTAGE_COMPRESS_FLAGS, PORTAGE_RSYNC_EXTRA_OPTS, RUSTFLAGS
```

inxi -F
```
System:    Host: area51 Kernel: 5.10.52-gentoo-dist x86_64 bits: 64 Desktop: KDE Plasma 5.21.5
           Distro: Gentoo Base System release 2.7
Machine:   Type: Portable System: Alienware product: Alienware 14 v: A12 serial: <superuser/root required>
           Mobo: Alienware model: 07MJ2Y v: A00 serial: <superuser/root required> UEFI: Alienware v: A12 date: 07/22/2019
Battery:   ID-1: BAT1 charge: 42.7 Wh condition: 44.0/71.0 Wh (62%)
CPU:       Info: Quad Core model: Intel Core i7-4700MQ bits: 64 type: MT MCP L2 cache: 6144 KiB
           Speed: 798 MHz min/max: 800/3400 MHz Core speeds (MHz): 1: 798 2: 798 3: 798 4: 798 5: 798 6: 798 7: 798 8: 799
Graphics:  Device-1: Intel 4th Gen Core Processor Integrated Graphics driver: i915 v: kernel
           Device-2: NVIDIA GK107M [GeForce GT 750M] driver: nvidia v: 460.91.03
           Device-3: Sunplus Innovation Laptop Integrated Webcam FHD type: USB driver: uvcvideo
           Display: x11 server: X.org 1.20.13 driver: modesetting,nvidia resolution: <xdpyinfo missing>
           OpenGL: renderer: GeForce GT 750M/PCIe/SSE2 v: 4.6.0 NVIDIA 460.91.03
Audio:     Device-1: Intel Xeon E3-1200 v3/4th Gen Core Processor HD Audio driver: snd_hda_intel
           Device-2: Intel 8 Series/C220 Series High Definition Audio driver: snd_hda_intel
           Device-3: NVIDIA GK107 HDMI Audio driver: snd_hda_intel
           Sound Server: ALSA v: k5.10.52-gentoo-dist
Network:   Device-1: Qualcomm Atheros Killer E220x Gigabit Ethernet driver: alx
           IF: enp8s0 state: down mac: <redacted>
           Device-2: Qualcomm Atheros AR9462 Wireless Network Adapter driver: ath9k
           IF: wlp10s0 state: up mac: <redacted>
           Device-3: Qualcomm Atheros AR3012 Bluetooth 4.0 type: USB driver: btusb
Drives:    Local Storage: total: 698.64 GiB used: 69.23 GiB (9.9%)
           ID-1: /dev/sda vendor: Western Digital model: WD7500BPKT-75PK4T0 size: 698.64 GiB
RAID:      Hardware-1: Intel 82801 Mobile SATA Controller [RAID mode] driver: ahci
Partition: ID-1: / size: 697.69 GiB used: 69.23 GiB (9.9%) fs: btrfs dev: /dev/dm-0
           ID-2: /home size: 697.69 GiB used: 69.23 GiB (9.9%) fs: btrfs dev: /dev/dm-0
Swap:      ID-1: swap-1 type: file size: 18.63 GiB used: 0 KiB (0.0%) file: /swapfile
Sensors:   System Temperatures: cpu: 58.0 C mobo: N/A gpu: nvidia temp: 54 C
           Fan Speeds (RPM): N/A
Info:      Processes: 217 Uptime: 8m Memory: 7.66 GiB used: 1.18 GiB (15.4%) Shell: Zsh inxi: 3.1.06
```

Notes:
* needs special config for NVIDIA optimus
* no kernel config because I'm using `sys-kernel/gentoo-kernel-bin`
