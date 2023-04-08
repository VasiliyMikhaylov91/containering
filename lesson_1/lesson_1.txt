chelchik@gb-linux:~$ sudo unshare --net --pid --fork --mount-proc /bin/bash
root@gb-linux:/home/chelchik# ps -aux
USER         PID %CPU %MEM    VSZ   RSS TTY      STAT START   TIME COMMAND
root           1  0.0  0.2  18888  4204 pts/1    S    11:09   0:00 /bin/bash
root           8  0.0  0.1  21620  3772 pts/1    R+   11:10   0:00 ps -aux
root@gb-linux:/home/chelchik# exit
exit
chelchik@gb-linux:~$ ps -aux
USER         PID %CPU %MEM    VSZ   RSS TTY      STAT START   TIME COMMAND
root           1  0.3  0.6 168264 12876 ?        Ss   10:59   0:02 /sbin/init splash
root           2  0.0  0.0      0     0 ?        S    10:59   0:00 [kthreadd]
root           3  0.0  0.0      0     0 ?        I<   10:59   0:00 [rcu_gp]
root           4  0.0  0.0      0     0 ?        I<   10:59   0:00 [rcu_par_gp]
root           5  0.0  0.0      0     0 ?        I<   10:59   0:00 [slub_flushwq]
root           6  0.0  0.0      0     0 ?        I<   10:59   0:00 [netns]
root           7  0.0  0.0      0     0 ?        I    10:59   0:00 [kworker/0:0-events]
root           8  0.0  0.0      0     0 ?        I<   10:59   0:00 [kworker/0:0H-events_highpri]
root           9  0.0  0.0      0     0 ?        I    10:59   0:00 [kworker/u8:0-flush-8:0]
root          10  0.0  0.0      0     0 ?        I<   10:59   0:00 [mm_percpu_wq]
root          11  0.0  0.0      0     0 ?        I    10:59   0:00 [rcu_tasks_kthread]
root          12  0.0  0.0      0     0 ?        I    10:59   0:00 [rcu_tasks_rude_kthread]
root          13  0.0  0.0      0     0 ?        I    10:59   0:00 [rcu_tasks_trace_kthread]
root          14  0.0  0.0      0     0 ?        S    10:59   0:00 [ksoftirqd/0]
root          15  0.0  0.0      0     0 ?        I    10:59   0:00 [rcu_preempt]
root          16  0.0  0.0      0     0 ?        S    10:59   0:00 [migration/0]
root          17  0.0  0.0      0     0 ?        S    10:59   0:00 [idle_inject/0]
root          19  0.0  0.0      0     0 ?        S    10:59   0:00 [cpuhp/0]
root          20  0.0  0.0      0     0 ?        S    10:59   0:00 [cpuhp/1]
root          21  0.0  0.0      0     0 ?        S    10:59   0:00 [idle_inject/1]
root          22  0.0  0.0      0     0 ?        S    10:59   0:00 [migration/1]
root          23  0.0  0.0      0     0 ?        S    10:59   0:00 [ksoftirqd/1]
root          25  0.0  0.0      0     0 ?        I<   10:59   0:00 [kworker/1:0H]
root          26  0.0  0.0      0     0 ?        S    10:59   0:00 [cpuhp/2]
root          27  0.0  0.0      0     0 ?        S    10:59   0:00 [idle_inject/2]
root          28  0.0  0.0      0     0 ?        S    10:59   0:00 [migration/2]
root          29  0.0  0.0      0     0 ?        S    10:59   0:00 [ksoftirqd/2]
root          31  0.0  0.0      0     0 ?        I<   10:59   0:00 [kworker/2:0H-events_highpri]
root          32  0.0  0.0      0     0 ?        S    10:59   0:00 [cpuhp/3]
root          33  0.0  0.0      0     0 ?        S    10:59   0:00 [idle_inject/3]
root          34  0.0  0.0      0     0 ?        S    10:59   0:00 [migration/3]
root          35  0.0  0.0      0     0 ?        S    10:59   0:00 [ksoftirqd/3]
root          36  0.0  0.0      0     0 ?        I    10:59   0:00 [kworker/3:0-mm_percpu_wq]
root          37  0.0  0.0      0     0 ?        I<   10:59   0:00 [kworker/3:0H-kblockd]
root          38  0.0  0.0      0     0 ?        S    10:59   0:00 [kdevtmpfs]
root          39  0.0  0.0      0     0 ?        I<   10:59   0:00 [inet_frag_wq]
root          40  0.0  0.0      0     0 ?        S    10:59   0:00 [kauditd]
root          41  0.0  0.0      0     0 ?        S    10:59   0:00 [khungtaskd]
root          43  0.0  0.0      0     0 ?        S    10:59   0:00 [oom_reaper]
root          45  0.0  0.0      0     0 ?        I<   10:59   0:00 [writeback]
root          46  0.0  0.0      0     0 ?        S    10:59   0:00 [kcompactd0]
root          47  0.0  0.0      0     0 ?        SN   10:59   0:00 [ksmd]
root          48  0.0  0.0      0     0 ?        SN   10:59   0:00 [khugepaged]
root          49  0.0  0.0      0     0 ?        I<   10:59   0:00 [kintegrityd]
root          50  0.0  0.0      0     0 ?        I<   10:59   0:00 [kblockd]
root          51  0.0  0.0      0     0 ?        I<   10:59   0:00 [blkcg_punt_bio]
root          52  0.0  0.0      0     0 ?        I<   10:59   0:00 [tpm_dev_wq]
root          53  0.0  0.0      0     0 ?        I<   10:59   0:00 [ata_sff]
root          54  0.0  0.0      0     0 ?        I<   10:59   0:00 [md]
root          55  0.0  0.0      0     0 ?        I<   10:59   0:00 [edac-poller]
root          56  0.0  0.0      0     0 ?        I<   10:59   0:00 [devfreq_wq]
root          57  0.0  0.0      0     0 ?        S    10:59   0:00 [watchdogd]
root          59  0.0  0.0      0     0 ?        I<   10:59   0:00 [kworker/0:1H-kblockd]
root          60  0.1  0.0      0     0 ?        S    10:59   0:01 [kswapd0]
root          61  0.0  0.0      0     0 ?        S    10:59   0:00 [ecryptfs-kthread]
root          67  0.0  0.0      0     0 ?        I<   10:59   0:00 [kthrotld]
root          72  0.0  0.0      0     0 ?        I<   10:59   0:00 [acpi_thermal_pm]
root          73  0.0  0.0      0     0 ?        S    10:59   0:00 [xenbus_probe]
root          74  0.0  0.0      0     0 ?        S    10:59   0:00 [scsi_eh_0]
root          75  0.0  0.0      0     0 ?        I<   10:59   0:00 [scsi_tmf_0]
root          76  0.0  0.0      0     0 ?        S    10:59   0:00 [scsi_eh_1]
root          77  0.0  0.0      0     0 ?        I<   10:59   0:00 [scsi_tmf_1]
root          78  0.0  0.0      0     0 ?        I<   10:59   0:00 [vfio-irqfd-clea]
root          80  0.0  0.0      0     0 ?        I    10:59   0:00 [kworker/u8:3-flush-8:0]
root          81  0.0  0.0      0     0 ?        I<   10:59   0:00 [kworker/3:1H-kblockd]
root          82  0.0  0.0      0     0 ?        I<   10:59   0:00 [mld]
root          83  0.0  0.0      0     0 ?        I<   10:59   0:00 [ipv6_addrconf]
root          88  0.0  0.0      0     0 ?        I<   10:59   0:00 [kstrp]
root          95  0.0  0.0      0     0 ?        I<   10:59   0:00 [zswap-shrink]
root          96  0.0  0.0      0     0 ?        I<   10:59   0:00 [kworker/u9:0]
root         142  0.0  0.0      0     0 ?        I<   10:59   0:00 [charger_manager]
root         143  0.0  0.0      0     0 ?        I    10:59   0:00 [kworker/2:2-mm_percpu_wq]
root         182  0.0  0.0      0     0 ?        I<   10:59   0:00 [kworker/2:1H-kblockd]
root         184  0.0  0.0      0     0 ?        S    10:59   0:00 [scsi_eh_2]
root         185  0.0  0.0      0     0 ?        I<   10:59   0:00 [scsi_tmf_2]
root         191  0.0  0.0      0     0 ?        I<   10:59   0:00 [kworker/1:1H-kblockd]
root         212  0.0  0.0      0     0 ?        S    10:59   0:00 [jbd2/sda3-8]
root         213  0.0  0.0      0     0 ?        I<   10:59   0:00 [ext4-rsv-conver]
root         252  0.0  1.8  97240 36708 ?        S<s  10:59   0:00 /lib/systemd/systemd-journald
root         287  0.0  0.0      0     0 ?        I<   10:59   0:00 [ipmi-msghandler]
root         298  0.0  0.0      0     0 ?        I    10:59   0:00 [kworker/2:3-events]
root         304  0.0  0.2  26792  5728 ?        Ss   10:59   0:00 /lib/systemd/systemd-udevd
root         305  0.0  0.0      0     0 ?        S    10:59   0:00 [irq/18-vmwgfx]
root         306  0.0  0.0      0     0 ?        S    10:59   0:00 [card0-crtc0]
root         307  0.0  0.0      0     0 ?        S    10:59   0:00 [card0-crtc1]
root         308  0.0  0.0      0     0 ?        S    10:59   0:00 [card0-crtc2]
root         309  0.0  0.0      0     0 ?        S    10:59   0:00 [card0-crtc3]
root         310  0.0  0.0      0     0 ?        S    10:59   0:00 [card0-crtc4]
root         311  0.0  0.0      0     0 ?        S    10:59   0:00 [card0-crtc5]
root         312  0.0  0.0      0     0 ?        S    10:59   0:00 [card0-crtc6]
root         313  0.0  0.0      0     0 ?        S    10:59   0:00 [card0-crtc7]
root         366  0.0  0.0      0     0 ?        I    10:59   0:00 [kworker/u8:7-events_unbound]
root         380  0.0  0.0      0     0 ?        I<   10:59   0:00 [cryptd]
root         475  0.0  0.0      0     0 ?        I    10:59   0:00 [kworker/1:3-events]
systemd+     487  0.0  0.2  14828  5916 ?        Ss   10:59   0:00 /lib/systemd/systemd-oomd
systemd+     490  0.0  0.5  25260 11668 ?        Ss   10:59   0:00 /lib/systemd/systemd-resolved
root         644  0.0  0.4 249168  8100 ?        Ssl  10:59   0:00 /usr/libexec/accounts-daemon
root         645  0.0  0.0   2812  1136 ?        Ss   10:59   0:00 /usr/sbin/acpid
avahi        648  0.0  0.1   7624  3196 ?        Ss   10:59   0:00 avahi-daemon: running [gb-linux.local]
root         649  0.0  0.1  18148  2960 ?        Ss   10:59   0:00 /usr/sbin/cron -f -P
message+     650  0.0  0.2  10068  5872 ?        Ss   10:59   0:00 @dbus-daemon --system --address=systemd: --nofork --n
root         652  0.0  0.7 344532 15528 ?        Ssl  10:59   0:00 /usr/sbin/NetworkManager --no-daemon
root         659  0.0  0.1  82764  3820 ?        Ssl  10:59   0:00 /usr/sbin/irqbalance --foreground
root         660  0.0  0.8  49712 16600 ?        Ss   10:59   0:00 /usr/bin/python3 /usr/bin/networkd-dispatcher --run-s
root         664  0.0  0.4 236908  9580 ?        Ssl  10:59   0:00 /usr/libexec/polkitd --no-debug
root         665  0.0  0.3 249080  6572 ?        Ssl  10:59   0:00 /usr/libexec/power-profiles-daemon
syslog       667  0.0  0.2 222400  4556 ?        Ssl  10:59   0:00 /usr/sbin/rsyslogd -n -iNONE
root         670  0.0  0.3 245200  6608 ?        Ssl  10:59   0:00 /usr/libexec/switcheroo-control
root         673  0.0  0.3  23644  7780 ?        Ss   10:59   0:00 /lib/systemd/systemd-logind
root         674  0.0  0.5 393060 11372 ?        Ssl  10:59   0:00 /usr/libexec/udisks2/udisksd
root         678  0.0  0.2  16496  4492 ?        Ss   10:59   0:00 /sbin/wpa_supplicant -u -s -O /run/wpa_supplicant
avahi        683  0.0  0.0   7440   272 ?        S    10:59   0:00 avahi-daemon: chroot helper
root         726  0.0  0.0      0     0 ?        I    10:59   0:00 [kworker/0:3-events]
root         752  0.0  0.5 213944 11080 ?        Ss   10:59   0:00 php-fpm: master process (/etc/php/8.1/fpm/php-fpm.con
root         766  0.0  0.4 317008  8976 ?        Ssl  10:59   0:00 /usr/sbin/ModemManager
root         775  0.1  0.6 1413372 12944 ?       Ssl  10:59   0:00 /usr/bin/containerd
root         779  0.0  0.3  15424  6412 ?        Ss   10:59   0:00 sshd: /usr/sbin/sshd -D [listener] 0 of 10-100 startu
root         817  0.0  0.9 126804 18528 ?        Ssl  10:59   0:00 /usr/bin/python3 /usr/share/unattended-upgrades/unatt
root         835  0.0  0.0  55204   432 ?        Ss   10:59   0:00 nginx: master process /usr/sbin/nginx -g daemon on; m
www-data     836  0.0  0.1  55876  2964 ?        S    10:59   0:00 nginx: worker process
www-data     837  0.0  0.1  55876  2964 ?        S    10:59   0:00 nginx: worker process
www-data     838  0.0  0.1  55876  2964 ?        S    10:59   0:00 nginx: worker process
www-data     840  0.0  0.1  55876  2964 ?        S    10:59   0:00 nginx: worker process
www-data     885  0.0  0.1 214420  3628 ?        S    10:59   0:00 php-fpm: pool www
www-data     886  0.0  0.1 214420  3648 ?        S    10:59   0:00 php-fpm: pool www
root         903  0.0  0.5 214124 10808 ?        Ss   10:59   0:00 /usr/sbin/apache2 -k start
www-data     930  0.0  0.2 214616  4176 ?        S    10:59   0:00 /usr/sbin/apache2 -k start
www-data     931  0.0  0.2 214616  4180 ?        S    10:59   0:00 /usr/sbin/apache2 -k start
www-data     932  0.0  0.2 214616  4180 ?        S    10:59   0:00 /usr/sbin/apache2 -k start
www-data     933  0.0  0.2 214616  4176 ?        S    10:59   0:00 /usr/sbin/apache2 -k start
www-data     934  0.0  0.2 214616  4168 ?        S    10:59   0:00 /usr/sbin/apache2 -k start
root         949  0.0  0.5  81256 10168 ?        Ss   10:59   0:00 /usr/sbin/cupsd -l
mysql        964  0.5 12.6 2250380 255200 ?      Ssl  10:59   0:04 /usr/sbin/mysqld
root        1401  0.0  0.4 172612  9860 ?        Ssl  10:59   0:00 /usr/sbin/cups-browsed
root        1404  0.0  1.5 1749388 30764 ?       Ssl  10:59   0:00 /usr/bin/dockerd -H fd:// --containerd=/run/container
kernoops    1420  0.0  0.0  13080   132 ?        Ss   10:59   0:00 /usr/sbin/kerneloops --test
kernoops    1425  0.0  0.0  13080   456 ?        Ss   10:59   0:00 /usr/sbin/kerneloops
root        2142  0.0  0.1 710900  2048 ?        Sl   10:59   0:00 /usr/bin/containerd-shim-runc-v2 -namespace moby -id
root        2167  0.0  0.0 710900  1916 ?        Sl   10:59   0:00 /usr/bin/containerd-shim-runc-v2 -namespace moby -id
vboxadd     2184  0.5 12.2 2370092 247436 ?      Ssl  10:59   0:03 mysqld --default-authentication-plugin=mysql_native_p
root        2192  0.0  0.3 158872  6580 ?        Ss   10:59   0:00 php-fpm: master process (/usr/local/etc/php-fpm.conf)
82          2529  0.0  0.1 158884  2652 ?        S    10:59   0:00 php-fpm: pool www
82          2530  0.0  0.1 158884  2652 ?        S    10:59   0:00 php-fpm: pool www
root        2610  0.0  0.1 305268  2876 ?        Sl   10:59   0:00 /usr/sbin/VBoxService --pidfile /var/run/vboxadd-serv
root        2621  0.0  0.4 250056  8652 ?        Ssl  10:59   0:00 /usr/sbin/gdm3
root        2626  0.0  0.4 179088  9496 ?        Sl   10:59   0:00 gdm-session-worker [pam/gdm-launch-environment]
gdm         2631  0.0  0.5  19148 11472 ?        Ss   10:59   0:00 /lib/systemd/systemd --user
gdm         2632  0.0  0.0 169924  1648 ?        S    10:59   0:00 (sd-pam)
gdm         2638  0.0  0.2  48084  5952 ?        S<sl 10:59   0:00 /usr/bin/pipewire
gdm         2639  0.0  0.2  32108  5756 ?        Ssl  10:59   0:00 /usr/bin/pipewire-media-session
gdm         2640  0.0  1.0 906968 21036 ?        S<sl 10:59   0:00 /usr/bin/pulseaudio --daemonize=no --log-target=journ
gdm         2643  0.0  0.2 171256  5808 tty1     Ssl+ 10:59   0:00 /usr/libexec/gdm-wayland-session dbus-run-session --
gdm         2645  0.0  0.2   8568  4480 ?        Ss   10:59   0:00 /usr/bin/dbus-daemon --session --address=systemd: --n
rtkit       2646  0.0  0.0 154000  1536 ?        SNsl 10:59   0:00 /usr/libexec/rtkit-daemon
gdm         2656  0.0  0.0   6492  1300 tty1     S+   10:59   0:00 dbus-run-session -- gnome-session --autostart /usr/sh
gdm         2657  0.0  0.2   8836  4652 tty1     S+   10:59   0:00 dbus-daemon --nofork --print-address 4 --session
gdm         2660  0.0  0.6 864392 12388 tty1     Sl+  10:59   0:00 /usr/libexec/gnome-session-binary --autostart /usr/sh
gdm         2661  0.0  0.3 249552  7884 ?        Ssl  10:59   0:00 /usr/libexec/gvfsd
gdm         2668  0.0  0.3 380884  6200 ?        Sl   10:59   0:00 /usr/libexec/gvfsd-fuse /run/user/127/gvfs -f
gdm         2683  0.2  6.3 4402740 128420 tty1   Sl+  10:59   0:01 /usr/bin/gnome-shell
gdm         2693  0.0  1.2 642232 24848 ?        SNsl 10:59   0:00 /usr/libexec/tracker-miner-fs-3
gdm         2703  0.0  0.3 472208  7656 ?        Ssl  10:59   0:00 /usr/libexec/xdg-document-portal
gdm         2708  0.0  0.2 244976  5548 ?        Ssl  10:59   0:00 /usr/libexec/xdg-permission-store
root        2715  0.0  0.0   2792  1012 ?        Ss   10:59   0:00 fusermount3 -o rw,nosuid,nodev,fsname=portal,auto_unm
gdm         2724  0.0  0.4 325096  9364 ?        Ssl  10:59   0:00 /usr/libexec/gvfs-udisks2-volume-monitor
gdm         2729  0.0  0.3 245332  6736 ?        Ssl  10:59   0:00 /usr/libexec/gvfs-mtp-volume-monitor
gdm         2741  0.0  0.3 245536  6636 ?        Ssl  10:59   0:00 /usr/libexec/gvfs-goa-volume-monitor
gdm         2746  0.0  1.3 573528 27872 ?        Sl   10:59   0:00 /usr/libexec/goa-daemon
gdm         2753  0.0  0.6 347456 12552 ?        Sl   10:59   0:00 /usr/libexec/goa-identity-service
gdm         2755  0.0  0.3 246288  6936 ?        Ssl  10:59   0:00 /usr/libexec/gvfs-gphoto2-volume-monitor
gdm         2761  0.0  0.4 324108  8236 ?        Ssl  10:59   0:00 /usr/libexec/gvfs-afc-volume-monitor
root        2768  0.0  0.4 251168  8760 ?        Ssl  10:59   0:00 /usr/libexec/upowerd
gdm         2793  0.0  0.3 309740  7580 tty1     Sl+  10:59   0:00 /usr/libexec/at-spi-bus-launcher
gdm         2798  0.0  0.1   8296  3988 tty1     S+   10:59   0:00 /usr/bin/dbus-daemon --config-file=/usr/share/default
gdm         2805  0.0  1.3 183212 27188 tty1     S+   10:59   0:00 /usr/bin/Xwayland :1024 -rootless -noreset -accessx -
gdm         2808  0.0  0.2 245188  5464 tty1     Sl+  10:59   0:00 /usr/libexec/xdg-permission-store
root        2814  0.0  0.8 307256 18072 ?        Ssl  10:59   0:00 /usr/libexec/packagekitd
gdm         2819  0.0  1.1 2669876 23340 tty1    Sl+  10:59   0:00 /usr/bin/gjs /usr/share/gnome-shell/org.gnome.Shell.N
gdm         2822  0.0  0.3 162676  7172 tty1     Sl+  10:59   0:00 /usr/libexec/at-spi2-registryd --use-gnome-session
gdm         2825  0.0  0.4 475192  9648 tty1     Sl+  10:59   0:00 /usr/libexec/gsd-sharing
gdm         2828  0.0  0.8 424096 17396 tty1     Sl+  10:59   0:00 /usr/libexec/gsd-wacom
gdm         2832  0.0  0.9 534508 18908 tty1     Sl+  10:59   0:00 /usr/libexec/gsd-color
gdm         2834  0.0  0.8 349812 17004 tty1     Sl+  10:59   0:00 /usr/libexec/gsd-keyboard
gdm         2839  0.0  0.5 258792 10448 tty1     Sl+  10:59   0:00 /usr/libexec/gsd-print-notifications
gdm         2846  0.0  0.3 466796  6488 tty1     Sl+  10:59   0:00 /usr/libexec/gsd-rfkill
gdm         2851  0.0  0.3 395300  8024 tty1     Sl+  10:59   0:00 /usr/libexec/gsd-smartcard
gdm         2853  0.0  0.6 384708 12600 tty1     Sl+  10:59   0:00 /usr/libexec/gsd-datetime
gdm         2864  0.0  1.0 873912 20564 tty1     Sl+  10:59   0:00 /usr/libexec/gsd-media-keys
gdm         2868  0.0  0.3 245228  6432 tty1     Sl+  10:59   0:00 /usr/libexec/gsd-screensaver-proxy
gdm         2872  0.0  0.4 328608  9088 tty1     Sl+  10:59   0:00 /usr/libexec/gsd-sound
gdm         2873  0.0  0.3 319684  6712 tty1     Sl+  10:59   0:00 /usr/libexec/gsd-a11y-settings
gdm         2876  0.0  0.3 321184  6912 tty1     Sl+  10:59   0:00 /usr/libexec/gsd-housekeeping
gdm         2883  0.0  0.9 533984 19388 tty1     Sl+  10:59   0:00 /usr/libexec/gsd-power
gdm         2927  0.0  0.5 351300 11540 tty1     Sl+  10:59   0:00 /usr/libexec/gsd-printer
colord      2955  0.0  0.5 254316 11716 ?        Ssl  10:59   0:00 /usr/libexec/colord
gdm         2971  0.0  1.1 2678204 23716 tty1    Sl+  10:59   0:00 /usr/bin/gjs /usr/share/gnome-shell/org.gnome.ScreenS
root        3008  0.0  0.5  17424 10564 ?        Ss   11:00   0:00 sshd: chelchik [priv]
chelchik    3012  0.1  0.5  19112 11476 ?        Ss   11:00   0:00 /lib/systemd/systemd --user
chelchik    3013  0.0  0.1 170204  2624 ?        S    11:00   0:00 (sd-pam)
chelchik    3019  0.0  0.3  48284  6376 ?        Ssl  11:00   0:00 /usr/bin/pipewire
chelchik    3020  0.0  0.3  32308  6432 ?        Ssl  11:00   0:00 /usr/bin/pipewire-media-session
chelchik    3021  0.0  0.9 306280 20132 ?        Ssl  11:00   0:00 /usr/bin/pulseaudio --daemonize=no --log-target=journ
chelchik    3034  0.0  0.2   8568  4652 ?        Ss   11:00   0:00 /usr/bin/dbus-daemon --session --address=systemd: --n
chelchik    3048  0.0  0.4 249552  8140 ?        Ssl  11:00   0:00 /usr/libexec/gvfsd
chelchik    3060  0.0  0.3 380884  6372 ?        Sl   11:00   0:00 /usr/libexec/gvfsd-fuse /run/user/1000/gvfs -f
chelchik    3126  0.0  0.3  17556  7620 ?        R    11:00   0:00 sshd: chelchik@pts/0
chelchik    3128  0.0  0.2  20044  5172 pts/0    Ss   11:00   0:00 -bash
chelchik    3133  0.0  1.1 642244 23656 ?        SNsl 11:00   0:00 /usr/libexec/tracker-miner-fs-3
chelchik    3144  0.0  0.4 325088  9520 ?        Ssl  11:00   0:00 /usr/libexec/gvfs-udisks2-volume-monitor
chelchik    3149  0.0  0.3 245332  6760 ?        Ssl  11:00   0:00 /usr/libexec/gvfs-mtp-volume-monitor
chelchik    3153  0.0  0.3 245536  6768 ?        Ssl  11:00   0:00 /usr/libexec/gvfs-goa-volume-monitor
chelchik    3158  0.0  1.4 573528 30288 ?        Sl   11:00   0:00 /usr/libexec/goa-daemon
chelchik    3170  0.0  0.6 347456 12700 ?        Sl   11:00   0:00 /usr/libexec/goa-identity-service
chelchik    3172  0.0  0.3 246288  6876 ?        Ssl  11:00   0:00 /usr/libexec/gvfs-gphoto2-volume-monitor
chelchik    3179  0.0  0.4 324108  8392 ?        Ssl  11:00   0:00 /usr/libexec/gvfs-afc-volume-monitor
chelchik    3197  0.0  0.3 472208  7680 ?        Ssl  11:00   0:00 /usr/libexec/xdg-document-portal
chelchik    3200  0.0  0.2 244976  5320 ?        Ssl  11:00   0:00 /usr/libexec/xdg-permission-store
root        3206  0.0  0.0   2792  1008 ?        Ss   11:00   0:00 fusermount3 -o rw,nosuid,nodev,fsname=portal,auto_unm
root       11935  0.0  0.0      0     0 ?        I    11:04   0:00 [kworker/1:0-cgroup_destroy]
root       12564  0.0  0.0      0     0 ?        I    11:05   0:00 [kworker/3:3-mm_percpu_wq]
root       12913  0.0  0.0      0     0 ?        I    11:05   0:00 [kworker/2:0-cgroup_destroy]
root       13191  0.0  0.0      0     0 ?        I    11:05   0:00 [kworker/0:1-cgroup_destroy]
root       15486  0.0  0.0      0     0 ?        I    11:06   0:00 [kworker/u8:1-events_unbound]
root       19589  0.0  0.0      0     0 ?        I    11:09   0:00 [kworker/0:2-cgroup_destroy]
root       21363  0.0  0.0      0     0 ?        I    11:09   0:00 [kworker/u8:2-flush-8:0]
root       21364  0.0  0.0      0     0 ?        I    11:09   0:00 [kworker/u8:4-flush-8:0]
root       21623 12.3  2.1 1244424 44348 ?       Ssl  11:10   0:06 /usr/lib/snapd/snapd
root       21745  0.1  0.3  14692  6292 ?        Ss   11:10   0:00 /lib/systemd/systemd-timedated
root       21799  0.0  0.0      0     0 ?        I    11:10   0:00 [kworker/1:1-mm_percpu_wq]
root       22020  0.0  0.0      0     0 ?        I    11:10   0:00 [kworker/u8:5-flush-8:0]
root       22047  0.0  0.0      0     0 ?        I    11:10   0:00 [kworker/2:1-cgroup_destroy]
root       23351  0.0  0.0      0     0 ?        I    11:10   0:00 [kworker/3:1-events]
root       23352  0.0  0.0      0     0 ?        I    11:10   0:00 [kworker/3:2]
root       23449  0.0  0.0      0     0 ?        I    11:10   0:00 [kworker/u8:6-writeback]
root       23541  0.0  0.0   2888   960 ?        Ss   11:10   0:00 /bin/sh /usr/lib/apt/apt.systemd.daily update
root       23545  0.0  0.0   2888  1812 ?        S    11:10   0:00 /bin/sh /usr/lib/apt/apt.systemd.daily lock_is_held u
chelchik   23548  1.1  1.3 940072 26448 ?        Ssl  11:10   0:00 /usr/bin/snap userd --agent
gdm        23549  1.1  1.2 941480 25864 ?        Ssl  11:10   0:00 /usr/bin/snap userd --agent
root       23613  0.7  0.5  29488 11220 ?        S    11:10   0:00 apt-get -qq -y update
_apt       23616  0.1  0.4  33296  9732 ?        S    11:10   0:00 /usr/lib/apt/methods/http
_apt       23617  0.1  0.4  33296  9676 ?        S    11:10   0:00 /usr/lib/apt/methods/http
_apt       23630  0.0  0.3  26312  6916 ?        S    11:10   0:00 /usr/lib/apt/methods/gpgv
_apt       23941  9.0  0.3  26268  7632 ?        S    11:10   0:00 /usr/lib/apt/methods/store
chelchik   23942  0.0  0.1  21780  3736 pts/0    R+   11:10   0:00 ps -aux
chelchik@gb-linux:~$