# Inspiron 3670 (sakura)

Configs for the Inspiron 3670, hostname sakura.

lspci
```
00:00.0 Host bridge: Intel Corporation 8th Gen Core Processor Host Bridge/DRAM Registers (rev 07)
00:02.0 VGA compatible controller: Intel Corporation UHD Graphics 630 (Desktop)
00:08.0 System peripheral: Intel Corporation Xeon E3-1200 v5/v6 / E3-1500 v5 / 6th/7th/8th Gen Core Processor Gaussian Mixture Model
00:12.0 Signal processing controller: Intel Corporation Cannon Lake PCH Thermal Controller (rev 10)
00:14.0 USB controller: Intel Corporation Cannon Lake PCH USB 3.1 xHCI Host Controller (rev 10)
00:14.2 RAM memory: Intel Corporation Cannon Lake PCH Shared SRAM (rev 10)
00:16.0 Communication controller: Intel Corporation Cannon Lake PCH HECI Controller (rev 10)
00:17.0 SATA controller: Intel Corporation Cannon Lake PCH SATA AHCI Controller (rev 10)
00:1b.0 PCI bridge: Intel Corporation Cannon Lake PCH PCI Express Root Port #21 (rev f0)
00:1c.0 PCI bridge: Intel Corporation Cannon Lake PCH PCI Express Root Port #5 (rev f0)
00:1c.7 PCI bridge: Intel Corporation Cannon Lake PCH PCI Express Root Port #8 (rev f0)
00:1f.0 ISA bridge: Intel Corporation Device a308 (rev 10)
00:1f.3 Audio device: Intel Corporation Cannon Lake PCH cAVS (rev 10)
00:1f.4 SMBus: Intel Corporation Cannon Lake PCH SMBus Controller (rev 10)
00:1f.5 Serial bus controller [0c80]: Intel Corporation Cannon Lake PCH SPI Controller (rev 10)
01:00.0 Non-Volatile memory controller: Sandisk Corp PC SN520 NVMe SSD (rev 01)
02:00.0 Ethernet controller: Realtek Semiconductor Co., Ltd. RTL8111/8168/8411 PCI Express Gigabit Ethernet Controller (rev 15)
03:00.0 Network controller: Qualcomm Atheros QCA9565 / AR9565 Wireless Network Adapter (rev 01)
```

lscpu
```
Architecture:                    x86_64
CPU op-mode(s):                  32-bit, 64-bit
Byte Order:                      Little Endian
Address sizes:                   39 bits physical, 48 bits virtual
CPU(s):                          6
On-line CPU(s) list:             0-5
Thread(s) per core:              1
Core(s) per socket:              6
Socket(s):                       1
NUMA node(s):                    1
Vendor ID:                       GenuineIntel
CPU family:                      6
Model:                           158
Model name:                      Intel(R) Core(TM) i5-8400 CPU @ 2.80GHz
Stepping:                        10
CPU MHz:                         2789.483
CPU max MHz:                     4000.0000
CPU min MHz:                     800.0000
BogoMIPS:                        5599.85
Virtualization:                  VT-x
L1d cache:                       192 KiB
L1i cache:                       192 KiB
L2 cache:                        1.5 MiB
L3 cache:                        9 MiB
NUMA node0 CPU(s):               0-5
Vulnerability Itlb multihit:     KVM: Mitigation: Split huge pages
Vulnerability L1tf:              Mitigation; PTE Inversion; VMX conditional cache flushes, SMT disabled
Vulnerability Mds:               Mitigation; Clear CPU buffers; SMT disabled
Vulnerability Meltdown:          Mitigation; PTI
Vulnerability Spec store bypass: Mitigation; Speculative Store Bypass disabled via prctl and seccomp
Vulnerability Spectre v1:        Mitigation; usercopy/swapgs barriers and __user pointer sanitization
Vulnerability Spectre v2:        Mitigation; Full generic retpoline, IBPB conditional, IBRS_FW, STIBP d
                                 isabled, RSB filling
Vulnerability Srbds:             Mitigation; Microcode
Vulnerability Tsx async abort:   Not affected
Flags:                           fpu vme de pse tsc msr pae mce cx8 apic sep mtrr pge mca cmov pat pse3
                                 6 clflush dts acpi mmx fxsr sse sse2 ss ht tm pbe syscall nx pdpe1gb r
                                 dtscp lm constant_tsc art arch_perfmon pebs bts rep_good nopl xtopolog
                                 y nonstop_tsc cpuid aperfmperf pni pclmulqdq dtes64 monitor ds_cpl vmx
                                  est tm2 ssse3 sdbg fma cx16 xtpr pdcm pcid sse4_1 sse4_2 x2apic movbe
                                  popcnt tsc_deadline_timer aes xsave avx f16c rdrand lahf_lm abm 3dnow
                                 prefetch cpuid_fault epb invpcid_single pti ssbd ibrs ibpb stibp tpr_s
                                 hadow vnmi flexpriority ept vpid ept_ad fsgsbase tsc_adjust bmi1 avx2 
                                 smep bmi2 erms invpcid mpx rdseed adx smap clflushopt intel_pt xsaveop
                                 t xsavec xgetbv1 xsaves dtherm ida arat pln pts hwp hwp_notify hwp_act
                                 _window hwp_epp md_clear flush_l1d
```

emerge --info
```
Portage 3.0.20 (python 3.9.6-final-0, default/linux/amd64/17.1/desktop/plasma/systemd, gcc-10.3.1, glibc-2.33-r1, 5.10.52-gentoo-x86_64 x86_64)
=================================================================
System uname: Linux-5.10.52-gentoo-x86_64-x86_64-Intel-R-_Core-TM-_i5-8400_CPU_@_2.80GHz-with-glibc2.33
KiB Mem:    11931136 total,   1478756 free
KiB Swap:   10534204 total,   9595196 free
Timestamp of repository gentoo: Fri, 27 Aug 2021 03:00:01 +0000
Head commit of repository gentoo: 39b92753f99a1d6f24c11757cd67e39b8c5e02d8
Head commit of repository alicela1ns-overlay: 4b8c26b1989858f0a774f976558de7c3c47a0c9f

Timestamp of repository powerman: Thu, 26 Aug 2021 17:36:43 +0000
Head commit of repository powerman: 01167319dd595898f951c29498048399a870ea1f

Timestamp of repository vifino-overlay: Thu, 26 Aug 2021 17:36:48 +0000
Head commit of repository vifino-overlay: a17179e7ce02bc4462f11e96b4206a59a978c8ea

sh bash 5.1_p8
ld GNU ld (Gentoo 2.36.1 p5) 2.36.1
distcc 3.4 x86_64-pc-linux-gnu [disabled]
ccache version 4.3 [disabled]
app-shells/bash:          5.1_p8::gentoo
dev-java/java-config:     2.3.1::gentoo
dev-lang/perl:            5.34.0::gentoo
dev-lang/python:          2.7.18_p11::gentoo, 3.9.6_p1::gentoo
dev-lang/rust-bin:        1.53.0::gentoo
dev-util/ccache:          4.3-r2::gentoo
dev-util/cmake:           3.20.5::gentoo
sys-apps/baselayout:      2.7::gentoo
sys-apps/sandbox:         2.24::gentoo
sys-devel/autoconf:       2.13-r1::gentoo, 2.69-r5::gentoo
sys-devel/automake:       1.16.3-r1::gentoo
sys-devel/binutils:       2.36.1-r2::gentoo
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
    sync-rsync-verify-jobs: 1
    sync-rsync-extra-opts: 
    sync-rsync-verify-max-age: 24

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
USE="X Xvaapi a52 aac acl acpi activities alsa amd64 avahi bluetooth branding bzip2 cairo cdda cdr cli crypt cups dbus declarative dri dts dvd dvdr emboss encode exif flac fortran gdbm gif gphoto2 gpm gtk gui iconv icu ios ipv6 jpeg kde kipi kwallet lcms libglvnd libnotify libtirpc mad mng mp3 mp4 mpeg multilib ncurses networkmanager nls nptl ogg opengl openmp pam pango pcre pdf plasma png policykit ppds pulseaudio qml qt5 readline sdl seccomp semantic-desktop sound spell split-usr ssl startup-notification svg systemd tcpd tiff truetype udev udisks unicode upower usb vim-syntax vorbis wayland widgets wxwidgets x264 xattr xcb xinerama xml xv xvid zlib zsh-completion" ABI_X86="64" ADA_TARGET="gnat_2021" ALSA_CARDS="ali5451 als4000 atiixp atiixp-modem bt87x ca0106 cmipci emu10k1x ens1370 ens1371 es1938 es1968 fm801 hda-intel intel8x0 intel8x0m maestro3 trident usb-audio via82xx via82xx-modem ymfpci" APACHE2_MODULES="authn_core authz_core socache_shmcb unixd actions alias auth_basic authn_alias authn_anon authn_dbm authn_default authn_file authz_dbm authz_default authz_groupfile authz_host authz_owner authz_user autoindex cache cgi cgid dav dav_fs dav_lock deflate dir disk_cache env expires ext_filter file_cache filter headers include info log_config logio mem_cache mime mime_magic negotiation rewrite setenvif speling status unique_id userdir usertrack vhost_alias" CALLIGRA_FEATURES="karbon sheets words" COLLECTD_PLUGINS="df interface irq load memory rrdtool swap syslog" CPU_FLAGS_X86="aes avx avx2 f16c fma3 mmx mmxext pclmul popcnt rdrand sse sse2 sse3 sse4_1 sse4_2 ssse3" ELIBC="glibc" GPSD_PROTOCOLS="ashtech aivdm earthmate evermore fv18 garmin garmintxt gpsclock greis isync itrax mtk3301 nmea ntrip navcom oceanserver oldstyle oncore rtcm104v2 rtcm104v3 sirf skytraq superstar2 timing tsip tripmate tnt ublox ubx" GRUB_PLATFORMS="efi-64 pc" INPUT_DEVICES="wacom libinput" KERNEL="linux" L10N="en en-US" LCD_DEVICES="bayrad cfontz cfontz633 glk hd44780 lb216 lcdm001 mtxorb ncurses text" LIBREOFFICE_EXTENSIONS="presenter-console presenter-minimizer" LUA_SINGLE_TARGET="lua5-1" LUA_TARGETS="lua5-1" OFFICE_IMPLEMENTATION="libreoffice" PHP_TARGETS="php7-3 php7-4" POSTGRES_TARGETS="postgres12 postgres13" PYTHON_SINGLE_TARGET="python3_9" PYTHON_TARGETS="python3_9" QEMU_SOFTMMU_TARGETS="arm aarch64 alpha i386 x86_64 sparc sparc64 ppc ppc64 riscv32 riscv64 mipsel mips64el mips mips64" QEMU_USER_TARGETS="x86_64 i386 aarch64 arm" RUBY_TARGETS="ruby26" USERLAND="GNU" VIDEO_CARDS="intel i965 iris" XTABLES_ADDONS="quota2 psd pknock lscan length2 ipv4options ipset ipp2p iface geoip fuzzy condition tee tarpit sysrq proto steal rawnat logmark ipmark dhcpmac delude chaos account"
Unset:  CC, CPPFLAGS, CTARGET, CXX, INSTALL_MASK, LC_ALL, LINGUAS, PORTAGE_BINHOST, PORTAGE_BUNZIP2_COMMAND, PORTAGE_COMPRESS, PORTAGE_COMPRESS_FLAGS, PORTAGE_RSYNC_EXTRA_OPTS, RUSTFLAGS
```

inxi -F
```
System:    Host: sakura Kernel: 5.10.52-gentoo-x86_64 x86_64 bits: 64 Desktop: KDE Plasma 5.21.5 
           Distro: Gentoo Base System release 2.7 
Machine:   Type: Desktop System: Dell product: Inspiron 3670 v: N/A 
           serial: <superuser/root required> 
           Mobo: Dell model: 0H4VK7 v: A01 serial: <superuser/root required> UEFI: Dell v: 2.15.0 
           date: 02/21/2020 
CPU:       Info: 6-Core model: Intel Core i5-8400 bits: 64 type: MCP L2 cache: 9216 KiB 
           Speed: 2450 MHz min/max: 800/4000 MHz Core speeds (MHz): 1: 900 2: 900 3: 900 4: 900 
           5: 900 6: 900 
Graphics:  Device-1: Intel UHD Graphics 630 driver: i915 v: kernel 
           Display: x11 server: X.Org 1.20.13 driver: modesetting resolution: 1920x1080~60Hz 
           OpenGL: renderer: Mesa Intel UHD Graphics 630 (CFL GT2) v: 4.6 Mesa 21.1.7 
Audio:     Device-1: Intel Cannon Lake PCH cAVS driver: snd_hda_intel 
           Sound Server: ALSA v: k5.10.52-gentoo-x86_64 
Network:   Device-1: Realtek RTL8111/8168/8411 PCI Express Gigabit Ethernet driver: r8169 
           IF: enp2s0 state: down mac: <redacted> 
           Device-2: Qualcomm Atheros QCA9565 / AR9565 Wireless Network Adapter driver: ath9k 
           IF: wlp3s0 state: up mac: <redacted> 
           Device-3: Qualcomm Atheros type: USB driver: btusb 
           IF-ID-1: dummy0 state: down mac: 3e:7a:ce:30:c5:1f 
           IF-ID-2: ipddp0 state: down mac: 00:00:00:00:00:00 
           IF-ID-3: sit0 state: down mac: 00:00:00:00 
           IF-ID-4: teql0 state: down mac: N/A 
           IF-ID-5: virbr0 state: down mac: 52:54:00:73:43:1c 
Drives:    Local Storage: total: 4.66 TiB used: 2.71 TiB (58.0%) 
           ID-1: /dev/nvme0n1 model: PC SN520 NVMe WDC 128GB size: 119.24 GiB 
           ID-2: /dev/sda vendor: Seagate model: ST1000DM010-2EP102 size: 931.51 GiB 
           ID-3: /dev/sdb type: USB vendor: Western Digital model: WD My Book 25EE size: 3.64 TiB 
Partition: ID-1: / size: 114.98 GiB used: 83.01 GiB (72.2%) fs: btrfs dev: /dev/dm-0 
           ID-2: /boot size: 196.9 MiB used: 188.1 MiB (95.5%) fs: vfat dev: /dev/nvme0n1p1 
           ID-3: /home size: 931.51 GiB used: 844.16 GiB (90.6%) fs: btrfs dev: /dev/dm-1 
           ID-4: /var/tmp size: 931.51 GiB used: 844.16 GiB (90.6%) fs: btrfs dev: /dev/dm-1 
Swap:      ID-1: swap-1 type: partition size: 4.05 GiB used: 0 KiB (0.0%) dev: /dev/nvme0n1p3 
           ID-2: swap-2 type: zram size: 6.00 GiB used: 916.5 MiB (14.9%) dev: /dev/zram0 
Sensors:   System Temperatures: cpu: 56.0 C mobo: N/A 
           Fan Speeds (RPM): N/A 
Info:      Processes: 384 Uptime: 1d 10h 17m Memory: 11.38 GiB used: 7.78 GiB (68.4%) Shell: Zsh 
           inxi: 3.1.06 
```

/proc/cmdline
```
initrd=\23e9b4ede725b48fe6559b4d5fcaf390\5.10.52-x86_64\initrd rd.luks.uuid=3fb4681c-aa9e-489b-9ac9-64eeff8fe85b rootflags=subvol=@gentoo root=UUID=703d8553-eba1-4903-8e5e-93a63a5314a3 rootfstype=btrfs ro root_trim=yes i915.enable_gvt=1 kvm.ignore_msrs=1 intel_pstate=disable resume=UUID=703d8553-eba1-4903-8e5e-93a63a5314a3 resume_offset=22549760 snd_hda_intel.single_cmd=1 snd_hda_intel.probe_mask=1
```
