# IdeaPad FLEX 15IWL (magenta-matrix)

Configs for the Lenovo IdeaPad FLEX 15IWL, hostname magenta-matrix.

lspci
```
00:00.0 Host bridge: Intel Corporation Coffee Lake HOST and DRAM Controller (rev 0c)
00:02.0 VGA compatible controller: Intel Corporation UHD Graphics 620 (Whiskey Lake) (rev 02)
00:04.0 Signal processing controller: Intel Corporation Xeon E3-1200 v5/E3-1500 v5/6th Gen Core Processor Thermal Subsystem (rev 0c)
00:08.0 System peripheral: Intel Corporation Xeon E3-1200 v5/v6 / E3-1500 v5 / 6th/7th/8th Gen Core Processor Gaussian Mixture Model
00:12.0 Signal processing controller: Intel Corporation Cannon Point-LP Thermal Controller (rev 30)
00:14.0 USB controller: Intel Corporation Cannon Point-LP USB 3.1 xHCI Controller (rev 30)
00:14.2 RAM memory: Intel Corporation Cannon Point-LP Shared SRAM (rev 30)
00:14.3 Network controller: Intel Corporation Cannon Point-LP CNVi [Wireless-AC] (rev 30)
00:15.0 Serial bus controller [0c80]: Intel Corporation Cannon Point-LP Serial IO I2C Controller #0 (rev 30)
00:15.1 Serial bus controller [0c80]: Intel Corporation Cannon Point-LP Serial IO I2C Controller #1 (rev 30)
00:15.2 Serial bus controller [0c80]: Intel Corporation Device 9dea (rev 30)
00:16.0 Communication controller: Intel Corporation Cannon Point-LP MEI Controller #1 (rev 30)
00:17.0 SATA controller: Intel Corporation Cannon Point-LP SATA Controller [AHCI Mode] (rev 30)
00:1d.0 PCI bridge: Intel Corporation Cannon Point-LP PCI Express Root Port #9 (rev f0)
00:1d.4 PCI bridge: Intel Corporation Cannon Point-LP PCI Express Root Port #13 (rev f0)
00:1f.0 ISA bridge: Intel Corporation Cannon Point-LP LPC Controller (rev 30)
00:1f.3 Audio device: Intel Corporation Cannon Point-LP High Definition Audio Controller (rev 30)
00:1f.4 SMBus: Intel Corporation Cannon Point-LP SMBus Controller (rev 30)
00:1f.5 Serial bus controller [0c80]: Intel Corporation Cannon Point-LP SPI Controller (rev 30)
01:00.0 Unassigned class [ff00]: Realtek Semiconductor Co., Ltd. RTS522A PCI Express Card Reader (rev 01)
02:00.0 Non-Volatile memory controller: Samsung Electronics Co Ltd NVMe SSD Controller SM981/PM981/PM983
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
Model:                           142
Model name:                      Intel(R) Core(TM) i5-8265U CPU @ 1.60GHz
Stepping:                        12
Frequency boost:                 enabled
CPU MHz:                         1514.096
CPU max MHz:                     1801.0000
CPU min MHz:                     400.0000
BogoMIPS:                        3600.00
Virtualization:                  VT-x
L1d cache:                       128 KiB
L1i cache:                       128 KiB
L2 cache:                        1 MiB
L3 cache:                        6 MiB
NUMA node0 CPU(s):               0-7
Vulnerability Itlb multihit:     KVM: Mitigation: Split huge pages
Vulnerability L1tf:              Not affected
Vulnerability Mds:               Not affected
Vulnerability Meltdown:          Not affected
Vulnerability Spec store bypass: Mitigation; Speculative Store Bypass disabled via prctl and seccomp
Vulnerability Spectre v1:        Mitigation; usercopy/swapgs barriers and __user pointer sanitization
Vulnerability Spectre v2:        Mitigation; Enhanced IBRS, IBPB conditional, RSB filling
Vulnerability Srbds:             Mitigation; TSX disabled
Vulnerability Tsx async abort:   Not affected
Flags:                           fpu vme de pse tsc msr pae mce cx8 apic sep mtrr pge mca cmov pat pse36 clflush dts acpi mmx fxsr sse sse2 ss ht tm pbe syscall nx pdpe1gb rdtscp lm constan
                                 t_tsc art arch_perfmon pebs bts rep_good nopl xtopology nonstop_tsc cpuid aperfmperf pni pclmulqdq dtes64 monitor ds_cpl vmx est tm2 ssse3 sdbg fma cx16 xtp
                                 r pdcm pcid sse4_1 sse4_2 x2apic movbe popcnt tsc_deadline_timer aes xsave avx f16c rdrand lahf_lm abm 3dnowprefetch cpuid_fault epb invpcid_single ssbd ibr
                                 s ibpb stibp ibrs_enhanced tpr_shadow vnmi flexpriority ept vpid ept_ad fsgsbase tsc_adjust bmi1 avx2 smep bmi2 erms invpcid mpx rdseed adx smap clflushopt 
                                 intel_pt xsaveopt xsavec xgetbv1 xsaves dtherm ida arat pln pts hwp hwp_notify hwp_act_window hwp_epp md_clear flush_l1d arch_capabilities
```

emerge --info
```
Portage 3.0.20 (python 3.9.6-final-0, default/linux/amd64/17.1/desktop/plasma/systemd, gcc-10.3.1, glibc-2.33-r1, 5.10.52-gentoo-x86_64 x86_64)
=================================================================
System uname: Linux-5.10.52-gentoo-x86_64-x86_64-Intel-R-_Core-TM-_i5-8265U_CPU_@_1.60GHz-with-glibc2.33
KiB Mem:     7858588 total,   1054204 free
KiB Swap:   23437496 total,  23422528 free
Timestamp of repository gentoo: Sat, 31 Jul 2021 00:45:02 +0000
Head commit of repository gentoo: ab8b0d3c153afeb3447963dcc4807fc41a288df6
Head commit of repository alicela1ns-overlay: 9c13622a6ff1ca13e95f74809a7e9942144fd811

Timestamp of repository powerman: Sat, 17 Jul 2021 08:07:08 +0000
Head commit of repository powerman: 6351e44ac2519488e7e503b5aa1ce4f131f565da

Timestamp of repository vifino-overlay: Fri, 16 Jul 2021 22:52:35 +0000
Head commit of repository vifino-overlay: 9ecb0d6bf1d9d88ba55dbc993617646d421760c4

sh bash 5.1_p8
ld GNU ld (Gentoo 2.35.2 p1) 2.35.2
distcc 3.4 x86_64-pc-linux-gnu [disabled]
ccache version 4.3 [disabled]
app-shells/bash:          5.1_p8::gentoo
dev-java/java-config:     2.3.1::gentoo
dev-lang/perl:            5.34.0::gentoo
dev-lang/python:          2.7.18_p11::gentoo, 3.9.6::gentoo
dev-lang/rust-bin:        1.53.0::gentoo
dev-util/ccache:          4.3-r2::gentoo
dev-util/cmake:           3.18.5::gentoo
dev-util/pkgconfig:       0.29.2::gentoo
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
    sync-rsync-extra-opts: 
    sync-rsync-verify-metamanifest: yes
    sync-rsync-verify-max-age: 24
    sync-rsync-verify-jobs: 1

alicela1ns-overlay
    location: /var/db/repos/alicela1ns-overlay
    sync-type: git
    sync-uri: git@github.com:alicela1n/alicela1n-gentoo-overlay.git
    masters: gentoo

localrepo
    location: /var/db/repos/localrepo
    masters: gentoo

powerman
    location: /var/db/repos/powerman
    sync-type: git
    sync-uri: https://github.com/gentoo-mirror/powerman.git
    masters: gentoo

vifino-overlay
    location: /var/db/repos/vifino-overlay
    sync-type: git
    sync-uri: https://github.com/gentoo-mirror/vifino-overlay.git
    masters: gentoo

crossdev
    location: /var/db/repos/localrepo-crossdev
    masters: gentoo
    priority: 10

ACCEPT_KEYWORDS="amd64"
ACCEPT_LICENSE="* -@EULA"
CBUILD="x86_64-pc-linux-gnu"
CFLAGS="-march=skylake -O2 -pipe"
CHOST="x86_64-pc-linux-gnu"
CONFIG_PROTECT="/etc /usr/share/config /usr/share/gnupg/qualified.txt"
CONFIG_PROTECT_MASK="/etc/ca-certificates.conf /etc/dconf /etc/env.d /etc/fonts/fonts.conf /etc/gconf /etc/gentoo-release /etc/php/apache2-php7.4/ext-active/ /etc/php/cgi-php7.4/ext-active/ /etc/php/cli-php7.4/ext-active/ /etc/revdep-rebuild /etc/sandbox.d /etc/terminfo /etc/texmf/language.dat.d /etc/texmf/language.def.d /etc/texmf/updmap.d /etc/texmf/web2c"
CXXFLAGS="-march=skylake -O2 -pipe"
DISTDIR="/var/cache/distfiles"
EMERGE_DEFAULT_OPTS=" --jobs 4 --usepkg-exclude 'sys-kernel/gentoo-sources virtual/*'"
ENV_UNSET="CARGO_HOME DBUS_SESSION_BUS_ADDRESS DISPLAY GOBIN GOPATH PERL5LIB PERL5OPT PERLPREFIX PERL_CORE PERL_MB_OPT PERL_MM_OPT XAUTHORITY XDG_CACHE_HOME XDG_CONFIG_HOME XDG_DATA_HOME XDG_RUNTIME_DIR"
FCFLAGS="-march=skylake -O2 -pipe"
FEATURES="assume-digests binpkg-docompress binpkg-dostrip binpkg-logs buildpkg config-protect-if-modified distlocks ebuild-locks fixlafiles ipc-sandbox merge-sync multilib-strict network-sandbox news parallel-fetch pid-sandbox preserve-libs protect-owned qa-unresolved-soname-deps sandbox sfperms strict unknown-features-warn unmerge-logs unmerge-orphans userfetch userpriv usersandbox usersync xattr"
FFLAGS="-march=skylake -O2 -pipe"
GENTOO_MIRRORS="https://mirrors.advancedhosters.com/gentoo/ http://gentoo.mirrors.easynews.com/linux/gentoo/ http://mirrors.rit.edu/gentoo/ http://www.gtlib.gatech.edu/pub/gentoo"
LANG="en_US.UTF-8"
LDFLAGS="-Wl,-O1 -Wl,--as-needed"
MAKEOPTS="-j7"
PKGDIR="/var/cache/binpkgs"
PORTAGE_CONFIGROOT="/"
PORTAGE_RSYNC_OPTS="--recursive --links --safe-links --perms --times --omit-dir-times --compress --force --whole-file --delete --stats --human-readable --timeout=180 --exclude=/distfiles --exclude=/local --exclude=/packages --exclude=/.git"
PORTAGE_TMPDIR="/var/tmp"
USE="X Xvaapi a52 aac acl acpi activities alsa amd64 avahi bluetooth branding bzip2 cairo cdda cdr cli crypt cups dbus declarative dri dts dvd dvdr emboss encode exif flac fortran gdbm gif gphoto2 gpm gtk gui iconv icu ios ipv6 jpeg kde kipi kwallet lcms libglvnd libnotify libtirpc mad mng mp3 mp4 mpeg multilib ncurses networkmanager nls nptl ogg opengl openmp pam pango pcre pdf phonon plasma png policykit ppds pulseaudio qml qt5 readline sdl seccomp semantic-desktop sound spell split-usr ssl startup-notification svg systemd tcpd tiff truetype udev udisks unicode upower usb vim-syntax vorbis wayland widgets wxwidgets x264 xattr xcb xinerama xml xv xvid zlib zsh-completion" ABI_X86="64" ADA_TARGET="gnat_2021" ALSA_CARDS="ali5451 als4000 atiixp atiixp-modem bt87x ca0106 cmipci emu10k1x ens1370 ens1371 es1938 es1968 fm801 hda-intel intel8x0 intel8x0m maestro3 trident usb-audio via82xx via82xx-modem ymfpci" APACHE2_MODULES="authn_core authz_core socache_shmcb unixd actions alias auth_basic authn_alias authn_anon authn_dbm authn_default authn_file authz_dbm authz_default authz_groupfile authz_host authz_owner authz_user autoindex cache cgi cgid dav dav_fs dav_lock deflate dir disk_cache env expires ext_filter file_cache filter headers include info log_config logio mem_cache mime mime_magic negotiation rewrite setenvif speling status unique_id userdir usertrack vhost_alias" CALLIGRA_FEATURES="karbon sheets words" COLLECTD_PLUGINS="df interface irq load memory rrdtool swap syslog" CPU_FLAGS_X86="aes avx avx2 f16c fma3 mmx mmxext pclmul popcnt rdrand sse sse2 sse3 sse4_1 sse4_2 ssse3" ELIBC="glibc" GPSD_PROTOCOLS="ashtech aivdm earthmate evermore fv18 garmin garmintxt gpsclock greis isync itrax mtk3301 nmea ntrip navcom oceanserver oldstyle oncore rtcm104v2 rtcm104v3 sirf skytraq superstar2 timing tsip tripmate tnt ublox ubx" GRUB_PLATFORMS="efi-64 pc" INPUT_DEVICES="wacom libinput" KERNEL="linux" L10N="en en-US" LCD_DEVICES="bayrad cfontz cfontz633 glk hd44780 lb216 lcdm001 mtxorb ncurses text" LIBREOFFICE_EXTENSIONS="presenter-console presenter-minimizer" LUA_SINGLE_TARGET="lua5-1" LUA_TARGETS="lua5-1" OFFICE_IMPLEMENTATION="libreoffice" PHP_TARGETS="php7-3 php7-4" POSTGRES_TARGETS="postgres10 postgres11" PYTHON_SINGLE_TARGET="python3_9" PYTHON_TARGETS="python3_9" QEMU_SOFTMMU_TARGETS="arm aarch64 alpha i386 x86_64 sparc sparc64 ppc ppc64 riscv32 riscv64 mipsel mips64el mips mips64" QEMU_USER_TARGETS="x86_64 i386 aarch64 arm" RUBY_TARGETS="ruby26" USERLAND="GNU" VIDEO_CARDS="intel i965 iris" XTABLES_ADDONS="quota2 psd pknock lscan length2 ipv4options ipset ipp2p iface geoip fuzzy condition tee tarpit sysrq proto steal rawnat logmark ipmark dhcpmac delude chaos account"
Unset:  CC, CPPFLAGS, CTARGET, CXX, INSTALL_MASK, LC_ALL, LINGUAS, PORTAGE_BINHOST, PORTAGE_BUNZIP2_COMMAND, PORTAGE_COMPRESS, PORTAGE_COMPRESS_FLAGS, PORTAGE_RSYNC_EXTRA_OPTS, RUSTFLAGS

```

inxi -F
```
System:    Host: magenta-matrix Kernel: 5.10.52-gentoo-x86_64 x86_64 bits: 64 Desktop: KDE Plasma 5.21.5 
           Distro: Gentoo Base System release 2.7 
Machine:   Type: Convertible System: LENOVO product: 81SR v: Lenovo IdeaPad FLEX-15IWL serial: <superuser/root required> 
           Mobo: LENOVO model: LNVNB161216 v: SDK0J40700 WIN serial: <superuser/root required> UEFI: LENOVO v: ALCN28WW(V2.05) 
           date: 11/25/2019 
Battery:   ID-1: BAT1 charge: 53.0 Wh condition: 53.0/52.5 Wh (101%) 
CPU:       Info: Quad Core model: Intel Core i5-8265U bits: 64 type: MT MCP L2 cache: 6144 KiB 
           Speed: 1800 MHz min/max: 400/1801 MHz Core speeds (MHz): 1: 1800 2: 1800 3: 1800 4: 1800 5: 1800 6: 1800 7: 1800 
           8: 1800 
Graphics:  Device-1: Intel UHD Graphics 620 driver: i915 v: kernel 
           Device-2: Syntek Integrated Camera type: USB driver: uvcvideo 
           Display: x11 server: X.org 1.20.11 driver: modesetting resolution: <xdpyinfo missing> 
           OpenGL: renderer: Mesa Intel UHD Graphics 620 (WHL GT2) v: 4.6 Mesa 21.1.4 
Audio:     Device-1: Intel Cannon Point-LP High Definition Audio driver: snd_hda_intel 
           Sound Server: ALSA v: k5.10.52-gentoo-x86_64 
Network:   Device-1: Intel Cannon Point-LP CNVi [Wireless-AC] driver: iwlwifi 
           IF: wlp0s20f3 state: up mac: <redacted> 
           IF-ID-1: sit0 state: down mac: 00:00:00:00 
           IF-ID-2: virbr0 state: down mac: 52:54:00:73:43:1c 
Drives:    Local Storage: total: 1.60 TiB used: 859.72 GiB (52.6%) 
           ID-1: /dev/nvme0n1 vendor: Samsung model: MZVLB256HAHQ-000L2 size: 238.47 GiB 
           ID-2: /dev/sda vendor: Western Digital model: WDBNCE0010PNC size: 931.51 GiB 
           ID-3: /dev/sdb type: USB model: ATA WDC WD5000LPCX-7 size: 465.76 GiB 
Partition: ID-1: / size: 229.48 GiB used: 72.45 GiB (31.6%) fs: btrfs dev: /dev/dm-0 
           ID-2: /boot size: 952.1 MiB used: 248.5 MiB (26.1%) fs: vfat dev: /dev/nvme0n1p1 
           ID-3: /home size: 931.51 GiB used: 777.91 GiB (83.5%) fs: btrfs dev: /dev/dm-1 
Swap:      ID-1: swap-1 type: file size: 22.35 GiB used: 14.6 MiB (0.1%) file: /swap/swapfile 
Sensors:   System Temperatures: cpu: 54.0 C mobo: N/A 
           Fan Speeds (RPM): N/A 
Info:      Processes: 317 Uptime: 2h 06m Memory: 7.49 GiB used: 4.99 GiB (66.6%) Shell: Zsh inxi: 3.1.06 
```
