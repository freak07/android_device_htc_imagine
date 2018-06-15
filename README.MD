Device files for building TWRP for HTC Imagine

DEVICE INFORMATION FOLLOWS
--------------------------
htc_imedugl:/ $ cat /proc/partitions
major minor  #blocks  name

   1        0       8192 ram0
   1        1       8192 ram1
   1        2       8192 ram2
   1        3       8192 ram3
   1        4       8192 ram4
   1        5       8192 ram5
   1        6       8192 ram6
   1        7       8192 ram7
   1        8       8192 ram8
   1        9       8192 ram9
   1       10       8192 ram10
   1       11       8192 ram11
   1       12       8192 ram12
   1       13       8192 ram13
   1       14       8192 ram14
   1       15       8192 ram15
   7        0      65536 loop0
 254        0    2911396 zram0
   8       16       4096 sdb
   8       17       3924 sdb1
   8       18        128 sdb2
   8        0   59662336 sda
   8        1        104 sda1
   8        2          8 sda2
   8        3      32768 sda3
   8        4      24256 sda4
   8        5       4096 sda5
   8        6       1024 sda6
   8        7       1024 sda7
   8        8      10240 sda8
   8        9      10240 sda9
   8       10      30720 sda10
   8       11      20480 sda11
   8       12        128 sda12
   8       13         32 sda13
   8       14        512 sda14
   8       15       1284 sda15
 259        0      46080 sda16
 259        1      61440 sda17
 259        2    3846144 sda18
 259        3    3846144 sda19
 259        4   51724288 sda20
 259        5       1280 sda21
   8       32       4096 sdc
   8       33       3924 sdc1
   8       34        128 sdc2
   8       48       4096 sdd
   8       49        104 sdd1
   8       50        128 sdd2
   8       51       3820 sdd3
   8       64    2805760 sde
   8       65        512 sde1
   8       66       2048 sde2
   8       67        512 sde3
   8       68        512 sde4
   8       69     112640 sde5
   8       70       1024 sde6
   8       71       4096 sde7
   8       72      32768 sde8
   8       73       1024 sde9
   8       74      32768 sde10
   8       75        512 sde11
   8       76        512 sde12
   8       77      65536 sde13
   8       78      32768 sde14
   8       79        512 sde15
 259        6        512 sde16
 259        7        128 sde17
 259        8         64 sde18
 259        9    1048576 sde19
 259       10         64 sde20
 259       11       8192 sde21
 259       12        512 sde22
 259       13       2048 sde23
 259       14        512 sde24
 259       15        512 sde25
 259       16     112640 sde26
 259       17       1024 sde27
 259       18       4096 sde28
 259       19      32768 sde29
 259       20       1024 sde30
 259       21      32768 sde31
 259       22        512 sde32
 259       23        512 sde33
 259       24      65536 sde34
 259       25      32768 sde35
 259       26        512 sde36
 259       27        512 sde37
 259       28        128 sde38
 259       29         64 sde39
 259       30    1048576 sde40
 259       31         64 sde41
 259       32       8192 sde42
 259       33         16 sde43
 259       34          4 sde44
 259       35       1024 sde45
 259       36        256 sde46
 259       37        256 sde47
 259       38          4 sde48
 259       39      33424 sde49
 259       40          4 sde50
 259       41       1024 sde51
 259       42       8192 sde52
 259       43       2048 sde53
 259       44      65536 sde54
 259       45        128 sde55
 259       46         16 sde56
 259       47       3224 sde57
   8       80       8192 sdf
   8       81         16 sdf1
   8       82        256 sdf2
   8       83       2048 sdf3
   8       84       1024 sdf4
   8       85       2048 sdf5
   8       86       2048 sdf6
   8       87        708 sdf7
 179        0  192251904 mmcblk0
 179        1  192219136 mmcblk0p1
 253        0   51724288 dm-0
 
htc_imedugl:/ $ cat /proc/filesystems                                          
nodev	sysfs
nodev	rootfs
nodev	ramfs
nodev	bdev
nodev	proc
nodev	cpuset
nodev	cgroup
nodev	cgroup2
nodev	tmpfs
nodev	configfs
nodev	debugfs
nodev	tracefs
nodev	sockfs
nodev	bpf
nodev	pipefs
nodev	devpts
	ext3
	ext4
	ext2
	vfat
	msdos
nodev	ecryptfs
nodev	sdcardfs
	fuseblk
nodev	fuse
nodev	fusectl
nodev	pstore
nodev	selinuxfs
nodev	functionfs
	texfat

htc_imedugl:/dev/block/platform/soc/1d84000.ufshc/by-name # ls -al
total 0
drwxr-xr-x 2 root root 1880 1970-02-05 04:16 .
drwxr-xr-x 4 root root 2040 1970-02-05 04:16 ..
lrwxrwxrwx 1 root root   15 1970-02-05 04:16 abl_a -> /dev/block/sde9
lrwxrwxrwx 1 root root   16 1970-02-05 04:16 abl_b -> /dev/block/sde30
lrwxrwxrwx 1 root root   15 1970-02-05 04:16 aop_a -> /dev/block/sde1
lrwxrwxrwx 1 root root   16 1970-02-05 04:16 aop_b -> /dev/block/sde22
lrwxrwxrwx 1 root root   16 1970-02-05 04:16 apdp -> /dev/block/sde46
lrwxrwxrwx 1 root root   16 1970-02-05 04:16 avb_rec -> /dev/block/sde56
lrwxrwxrwx 1 root root   15 1970-02-05 04:16 bluetooth_a -> /dev/block/sde6
lrwxrwxrwx 1 root root   16 1970-02-05 04:16 bluetooth_b -> /dev/block/sde27
lrwxrwxrwx 1 root root   15 1970-02-05 04:16 board_info -> /dev/block/sdf1
lrwxrwxrwx 1 root root   16 1970-02-05 04:16 boot_a -> /dev/block/sde13
lrwxrwxrwx 1 root root   16 1970-02-05 04:16 boot_b -> /dev/block/sde34
lrwxrwxrwx 1 root root   16 1970-02-05 04:16 carrier -> /dev/block/sda16
lrwxrwxrwx 1 root root   15 1970-02-05 04:16 cdt -> /dev/block/sdd2
lrwxrwxrwx 1 root root   16 1970-02-05 04:16 cmnlib64_a -> /dev/block/sde16
lrwxrwxrwx 1 root root   16 1970-02-05 04:16 cmnlib64_b -> /dev/block/sde37
lrwxrwxrwx 1 root root   16 1970-02-05 04:16 cmnlib_a -> /dev/block/sde15
lrwxrwxrwx 1 root root   16 1970-02-05 04:16 cmnlib_b -> /dev/block/sde36
lrwxrwxrwx 1 root root   16 1970-02-05 04:16 control -> /dev/block/sda13
lrwxrwxrwx 1 root root   16 1970-02-05 04:16 cota -> /dev/block/sda17
lrwxrwxrwx 1 root root   15 1970-02-05 04:16 ddr -> /dev/block/sdd3
lrwxrwxrwx 1 root root   16 1970-02-05 04:16 devcfg_a -> /dev/block/sde17
lrwxrwxrwx 1 root root   16 1970-02-05 04:16 devcfg_b -> /dev/block/sde38
lrwxrwxrwx 1 root root   16 1970-02-05 04:16 devinfo -> /dev/block/sde44
lrwxrwxrwx 1 root root   16 1970-02-05 04:16 devlog -> /dev/block/sda10
lrwxrwxrwx 1 root root   16 1970-02-05 04:16 dip -> /dev/block/sde45
lrwxrwxrwx 1 root root   16 1970-02-05 04:16 dpo -> /dev/block/sde48
lrwxrwxrwx 1 root root   16 1970-02-05 04:16 dsp_a -> /dev/block/sde10
lrwxrwxrwx 1 root root   16 1970-02-05 04:16 dsp_b -> /dev/block/sde31
lrwxrwxrwx 1 root root   16 1970-02-05 04:16 dtbo_a -> /dev/block/sde21
lrwxrwxrwx 1 root root   16 1970-02-05 04:16 dtbo_b -> /dev/block/sde42
lrwxrwxrwx 1 root root   16 1970-02-05 04:16 extra -> /dev/block/sda12
lrwxrwxrwx 1 root root   16 1970-02-05 04:16 fataldevlog -> /dev/block/sda11
lrwxrwxrwx 1 root root   16 1970-02-05 04:16 frp -> /dev/block/sda14
lrwxrwxrwx 1 root root   15 1970-02-05 04:16 fsc -> /dev/block/sdf4
lrwxrwxrwx 1 root root   15 1970-02-05 04:16 fsg -> /dev/block/sdf3
lrwxrwxrwx 1 root root   16 1970-02-05 04:16 hosd_a -> /dev/block/sde14
lrwxrwxrwx 1 root root   16 1970-02-05 04:16 hosd_b -> /dev/block/sde35
lrwxrwxrwx 1 root root   15 1970-02-05 04:16 hvbmeta -> /dev/block/sda4
lrwxrwxrwx 1 root root   15 1970-02-05 04:16 hyp_a -> /dev/block/sde3
lrwxrwxrwx 1 root root   16 1970-02-05 04:16 hyp_b -> /dev/block/sde24
lrwxrwxrwx 1 root root   16 1970-02-05 04:16 keymaster_a -> /dev/block/sde11
lrwxrwxrwx 1 root root   16 1970-02-05 04:16 keymaster_b -> /dev/block/sde32
lrwxrwxrwx 1 root root   16 1970-02-05 04:16 limits -> /dev/block/sde50
lrwxrwxrwx 1 root root   16 1970-02-05 04:16 local -> /dev/block/sda15
lrwxrwxrwx 1 root root   16 1970-02-05 04:16 lockbooter_a -> /dev/block/sde12
lrwxrwxrwx 1 root root   16 1970-02-05 04:16 lockbooter_b -> /dev/block/sde33
lrwxrwxrwx 1 root root   16 1970-02-05 04:16 logdump -> /dev/block/sde54
lrwxrwxrwx 1 root root   16 1970-02-05 04:16 logfs -> /dev/block/sde52
lrwxrwxrwx 1 root root   15 1970-02-05 04:16 mdtp_a -> /dev/block/sde8
lrwxrwxrwx 1 root root   16 1970-02-05 04:16 mdtp_b -> /dev/block/sde29
lrwxrwxrwx 1 root root   15 1970-02-05 04:16 mdtpsecapp_a -> /dev/block/sde7
lrwxrwxrwx 1 root root   16 1970-02-05 04:16 mdtpsecapp_b -> /dev/block/sde28
lrwxrwxrwx 1 root root   15 1970-02-05 04:16 mfg -> /dev/block/sdf2
lrwxrwxrwx 1 root root   15 1970-02-05 04:16 misc -> /dev/block/sda6
lrwxrwxrwx 1 root root   15 1970-02-05 04:16 modemst1 -> /dev/block/sdf5
lrwxrwxrwx 1 root root   15 1970-02-05 04:16 modemst2 -> /dev/block/sdf6
lrwxrwxrwx 1 root root   16 1970-02-05 04:16 msadp -> /dev/block/sde47
lrwxrwxrwx 1 root root   15 1970-02-05 04:16 oem_misc -> /dev/block/sda7
lrwxrwxrwx 1 root root   15 1970-02-05 04:16 padding0 -> /dev/block/sda1
lrwxrwxrwx 1 root root   15 1970-02-05 04:16 padding3 -> /dev/block/sdd1
lrwxrwxrwx 1 root root   15 1970-02-05 04:16 persist -> /dev/block/sda3
lrwxrwxrwx 1 root root   15 1970-02-05 04:16 pg1fs -> /dev/block/sda5
lrwxrwxrwx 1 root root   15 1970-02-05 04:16 pmic_a -> /dev/block/sde4
lrwxrwxrwx 1 root root   16 1970-02-05 04:16 pmic_b -> /dev/block/sde25
lrwxrwxrwx 1 root root   16 1970-02-05 04:16 qupfw_a -> /dev/block/sde18
lrwxrwxrwx 1 root root   16 1970-02-05 04:16 qupfw_b -> /dev/block/sde39
lrwxrwxrwx 1 root root   15 1970-02-05 04:16 radio_a -> /dev/block/sde5
lrwxrwxrwx 1 root root   16 1970-02-05 04:16 radio_b -> /dev/block/sde26
lrwxrwxrwx 1 root root   15 1970-02-05 04:16 ramdump -> /dev/block/sda8
lrwxrwxrwx 1 root root   16 1970-02-05 04:16 reserve0 -> /dev/block/sda21
lrwxrwxrwx 1 root root   16 1970-02-05 04:16 reserve4 -> /dev/block/sde57
lrwxrwxrwx 1 root root   15 1970-02-05 04:16 reserve5 -> /dev/block/sdf7
lrwxrwxrwx 1 root root   16 1970-02-05 04:16 sec -> /dev/block/sde43
lrwxrwxrwx 1 root root   16 1970-02-05 04:16 sp1 -> /dev/block/sde49
lrwxrwxrwx 1 root root   15 1970-02-05 04:16 ssd -> /dev/block/sda2
lrwxrwxrwx 1 root root   16 1970-02-05 04:16 sti -> /dev/block/sde53
lrwxrwxrwx 1 root root   16 1970-02-05 04:16 storsec -> /dev/block/sde55
lrwxrwxrwx 1 root root   16 1970-02-05 04:16 system_a -> /dev/block/sda18
lrwxrwxrwx 1 root root   16 1970-02-05 04:16 system_b -> /dev/block/sda19
lrwxrwxrwx 1 root root   15 1970-02-05 04:16 tool_diag -> /dev/block/sda9
lrwxrwxrwx 1 root root   16 1970-02-05 04:16 toolsfv -> /dev/block/sde51
lrwxrwxrwx 1 root root   15 1970-02-05 04:16 tz_a -> /dev/block/sde2
lrwxrwxrwx 1 root root   16 1970-02-05 04:16 tz_b -> /dev/block/sde23
lrwxrwxrwx 1 root root   16 1970-02-05 04:16 userdata -> /dev/block/sda20
lrwxrwxrwx 1 root root   16 1970-02-05 04:16 vbmeta_a -> /dev/block/sde20
lrwxrwxrwx 1 root root   16 1970-02-05 04:16 vbmeta_b -> /dev/block/sde41
lrwxrwxrwx 1 root root   16 1970-02-05 04:16 vendor_a -> /dev/block/sde19
lrwxrwxrwx 1 root root   16 1970-02-05 04:16 vendor_b -> /dev/block/sde40
lrwxrwxrwx 1 root root   15 1970-02-05 04:16 xbl_a -> /dev/block/sdb1
lrwxrwxrwx 1 root root   15 1970-02-05 04:16 xbl_b -> /dev/block/sdc1
lrwxrwxrwx 1 root root   15 1970-02-05 04:16 xbl_config_a -> /dev/block/sdb2
lrwxrwxrwx 1 root root   15 1970-02-05 04:16 xbl_config_b -> /dev/block/sdc2

