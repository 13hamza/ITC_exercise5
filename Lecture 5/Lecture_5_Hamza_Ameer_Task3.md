# Lecture 5 - Task 3

```bash
sed "s/root/ROOT/g" processes.log
```
```
USER         PID %CPU %MEM    VSZ   RSS TTY      STAT START   TIME COMMAND
ROOT           1  0.1  0.9  25224 16480 ?        Ss   09:19   0:03 /usr/lib/systemd/systemd --system --deserialize=92
ROOT           2  0.0  0.0      0     0 ?        S    09:19   0:00 [kthreadd]
ROOT           3  0.0  0.0      0     0 ?        S    09:19   0:00 [pool_workqueue_release]
ROOT           4  0.0  0.0      0     0 ?        I<   09:19   0:00 [kworker/R-rcu_gp]
ROOT           5  0.0  0.0      0     0 ?        I<   09:19   0:00 [kworker/R-sync_wq]
ROOT           6  0.0  0.0      0     0 ?        I<   09:19   0:00 [kworker/R-kvfree_rcu_reclaim]
ROOT           7  0.0  0.0      0     0 ?        I<   09:19   0:00 [kworker/R-slub_flushwq]
ROOT           8  0.0  0.0      0     0 ?        I<   09:19   0:00 [kworker/R-netns]
ROOT          10  0.0  0.0      0     0 ?        I<   09:19   0:00 [kworker/0:0H-kblockd]
ROOT          12  0.0  0.0      0     0 ?        I    09:19   0:00 [kworker/u4:0-ext4-rsv-conversion]
ROOT          13  0.0  0.0      0     0 ?        I<   09:19   0:00 [kworker/R-mm_percpu_wq]
ROOT          14  0.0  0.0      0     0 ?        S    09:19   0:02 [ksoftirqd/0]
ROOT          15  0.0  0.0      0     0 ?        I    09:19   0:00 [rcu_preempt]
ROOT          16  0.0  0.0      0     0 ?        S    09:19   0:00 [rcu_exp_par_gp_kthread_worker/0]
ROOT          17  0.0  0.0      0     0 ?        S    09:19   0:00 [rcu_exp_gp_kthread_worker]
ROOT          18  0.0  0.0      0     0 ?        S    09:19   0:00 [migration/0]
ROOT          19  0.0  0.0      0     0 ?        S    09:19   0:00 [kprobe-optimizer]
ROOT          20  0.0  0.0      0     0 ?        S    09:19   0:00 [idle_inject/0]
ROOT          21  0.0  0.0      0     0 ?        S    09:19   0:00 [cpuhp/0]
ROOT          22  0.0  0.0      0     0 ?        S    09:19   0:00 [kdevtmpfs]
ROOT          23  0.0  0.0      0     0 ?        I<   09:19   0:00 [kworker/R-inet_frag_wq]
ROOT          24  0.0  0.0      0     0 ?        I    09:19   0:00 [rcu_tasks_kthread]
ROOT          25  0.0  0.0      0     0 ?        I    09:19   0:00 [rcu_tasks_rude_kthread]
ROOT          26  0.0  0.0      0     0 ?        S    09:19   0:00 [kauditd]
ROOT          27  0.0  0.0      0     0 ?        S    09:19   0:00 [khungtaskd]
ROOT          28  0.0  0.0      0     0 ?        S    09:19   0:00 [oom_reaper]
ROOT          31  0.0  0.0      0     0 ?        I<   09:19   0:00 [kworker/R-writeback]
ROOT          32  0.0  0.0      0     0 ?        S    09:19   0:00 [kcompactd0]
ROOT          33  0.0  0.0      0     0 ?        SN   09:19   0:00 [ksmd]
ROOT          34  0.0  0.0      0     0 ?        SN   09:19   0:00 [khugepaged]
ROOT          35  0.0  0.0      0     0 ?        I<   09:19   0:00 [kworker/R-kblockd]
ROOT          36  0.0  0.0      0     0 ?        I<   09:19   0:00 [kworker/R-blkcg_punt_bio]
ROOT          37  0.0  0.0      0     0 ?        I<   09:19   0:00 [kworker/R-kintegrityd]
ROOT          38  0.0  0.0      0     0 ?        S    09:19   0:00 [irq/9-acpi]
ROOT          39  0.0  0.0      0     0 ?        I<   09:19   0:00 [kworker/R-tpm_dev_wq]
ROOT          40  0.0  0.0      0     0 ?        I<   09:19   0:00 [kworker/R-ata_sff]
ROOT          41  0.0  0.0      0     0 ?        I<   09:19   0:00 [kworker/R-md_bitmap]
ROOT          42  0.0  0.0      0     0 ?        I<   09:19   0:00 [kworker/R-md_llbitmap_io]
ROOT          43  0.0  0.0      0     0 ?        I<   09:19   0:00 [kworker/R-md_llbitmap_unplug]
ROOT          44  0.0  0.0      0     0 ?        I<   09:19   0:00 [kworker/R-edac-poller]
ROOT          45  0.0  0.0      0     0 ?        I<   09:19   0:00 [kworker/R-devfreq_wq]
ROOT          46  0.0  0.0      0     0 ?        S    09:19   0:00 [watchdogd]
ROOT          47  0.0  0.0      0     0 ?        I<   09:19   0:00 [kworker/R-quota_events_unbound]
ROOT          48  0.0  0.0      0     0 ?        S    09:19   0:00 [kswapd0]
ROOT          49  0.0  0.0      0     0 ?        S    09:19   0:00 [ecryptfs-kthread]
ROOT          50  0.0  0.0      0     0 ?        I<   09:19   0:00 [kworker/R-kthrotld]
ROOT          51  0.0  0.0      0     0 ?        I<   09:19   0:00 [kworker/R-acpi_thermal_pm]
ROOT          52  0.0  0.0      0     0 ?        S    09:19   0:00 [scsi_eh_0]
ROOT          53  0.0  0.0      0     0 ?        I<   09:19   0:00 [kworker/R-scsi_tmf_0]
ROOT          54  0.0  0.0      0     0 ?        S    09:19   0:00 [scsi_eh_1]
ROOT          55  0.0  0.0      0     0 ?        I<   09:19   0:00 [kworker/R-scsi_tmf_1]
ROOT          58  0.0  0.0      0     0 ?        I    09:19   0:00 [kworker/u4:5-writeback]
ROOT          59  0.0  0.0      0     0 ?        I<   09:19   0:00 [kworker/R-mld]
ROOT          61  0.0  0.0      0     0 ?        I<   09:19   0:00 [kworker/R-ipv6_addrconf]
ROOT          62  0.0  0.0      0     0 ?        I<   09:19   0:00 [kworker/R-kstrp]
ROOT          65  0.0  0.0      0     0 ?        I<   09:19   0:00 [kworker/u5:0]
ROOT          76  0.0  0.0      0     0 ?        I<   09:19   0:00 [kworker/R-charger_manager]
ROOT         278  0.0  0.0      0     0 ?        S    09:19   0:00 [scsi_eh_2]
ROOT         279  0.0  0.0      0     0 ?        I<   09:19   0:00 [kworker/R-scsi_tmf_2]
ROOT         311  0.0  0.0      0     0 ?        S    09:19   0:00 [jbd2/sda2-8]
ROOT         312  0.0  0.0      0     0 ?        I<   09:19   0:00 [kworker/R-ext4-rsv-conversion]
ROOT         442  0.0  0.0      0     0 ?        I<   09:19   0:00 [kworker/R-kmpathd]
ROOT         447  0.0  0.0      0     0 ?        I<   09:19   0:00 [kworker/R-kmpath_handlerd]
ROOT         774  0.0  0.0      0     0 ?        I<   09:19   0:00 [kworker/R-cfg80211]
ROOT         804  0.0  0.0      0     0 ?        S    09:19   0:00 [irq/18-vmwgfx]
ROOT         808  0.0  0.1   2888  2016 ?        Ss   09:19   0:00 /bin/sh /usr/lib/systemd/scripts/chronyd-starter.sh -n -F 1
ROOT         809  0.0  0.0      0     0 ?        I<   09:19   0:00 [kworker/R-ttm]
message+     810  0.0  0.3   9168  5820 ?        Ss   09:19   0:00 @dbus-daemon --system --address=systemd: --nofork --nopidfile --systemd-activation --syslog-only
ROOT         817  0.0  1.7  46844 30252 ?        Ss   09:19   0:00 /usr/bin/python3 /usr/bin/networkd-dispatcher --run-startup-triggers
ROOT         823  0.0  2.5 1878004 42524 ?       Ssl  09:19   0:00 /usr/lib/snapd/snapd
ROOT         827  0.0  0.5  18572  9748 ?        Ss   09:19   0:00 /usr/lib/systemd/systemd-logind
_chrony      900  0.0  0.3  20556  6384 ?        S    09:19   0:00 /usr/sbin/chronyd -n -F 1
ROOT         902  0.0  1.9 126116 33048 ?        Ssl  09:19   0:00 /usr/bin/python3 /usr/share/unattended-upgrades/unattended-upgrade-shutdown --wait-for-signal
_chrony      923  0.0  0.1  12096  2460 ?        S    09:19   0:00 /usr/sbin/chronyd -n -F 1
ROOT         942  0.0  0.3   8760  5544 ?        Ss   09:19   0:00 login -- hamza
hamza       1178  0.0  0.7  21608 12608 ?        Ss   09:19   0:00 /usr/lib/systemd/systemd --user --deserialize=10
hamza       1185  0.0  0.2  23012  4096 ?        S    09:19   0:00 (sd-pam)
hamza       1209  0.0  0.3   8856  6072 tty1     Ss   09:19   0:00 -bash
ROOT        1627  0.0  0.0      0     0 ?        I    09:40   0:00 [kworker/0:0-cgroup_release]
ROOT        1634  0.3  0.0      0     0 ?        I    09:50   0:02 [kworker/0:1-events]
ROOT        1729  0.0  0.0      0     0 ?        I    09:50   0:00 [kworker/u4:2-events_unbound]
ROOT       11393  0.2  0.0      0     0 ?        I<   09:52   0:01 [kworker/0:1H-kblockd]
ROOT       18003  0.0  0.2   7060  3404 ?        Ss   09:53   0:00 /usr/sbin/cron -f -P
ROOT       18009  0.0  0.5 214212  9768 ?        SLsl 09:53   0:00 /usr/sbin/multipathd -d -s
polkitd    18539  0.0  0.5 306448  8416 ?        Ssl  09:53   0:00 /usr/lib/polkit-1/polkitd --no-debug --log-level=notice
ROOT       18547  0.0  0.9 543364 15184 ?        Ssl  09:53   0:00 /usr/libexec/udisks2/udisksd
systemd+   18553  0.0  0.8  22432 14612 ?        Ss   09:53   0:00 /usr/lib/systemd/systemd-resolved
ROOT       18554  0.0  0.7  34116 13216 ?        S<s  09:53   0:00 /usr/lib/systemd/systemd-journald
ROOT       18559  0.0  0.6 318672 11520 ?        Ssl  09:53   0:00 /usr/libexec/upowerd
ROOT       18561  0.0  2.7 365856 46032 ?        Ssl  09:53   0:00 /usr/libexec/fwupd/fwupd
ROOT       18573  0.0  0.4  10744  7748 ?        Ss   09:53   0:00 sshd: /usr/sbin/sshd -D [listener] 0 of 10-100 startups
ROOT       18588  0.0  0.7  37976 12412 ?        Ss   09:53   0:00 /usr/lib/systemd/systemd-udevd
ROOT       18603  0.0  0.8 391608 14128 ?        Ssl  09:53   0:00 /usr/sbin/ModemManager
systemd+   18617  0.0  0.7  21204 12144 ?        Ss   09:53   0:00 /usr/lib/systemd/systemd-networkd
ROOT       18618  0.0  0.0      0     0 ?        S    09:53   0:00 [psimon]
syslog     18620  0.0  0.3 220548  5312 ?        Ssl  09:53   0:00 /usr/sbin/rsyslogd -n -iNONE
ROOT       18889  0.0  0.0      0     0 ?        S    09:53   0:00 [psimon]
ROOT       19598  0.0  0.0      0     0 ?        I    09:59   0:00 [kworker/u4:1-events_unbound]
ROOT       19599  0.0  0.0      0     0 ?        I    09:59   0:00 [kworker/0:2-events]
hamza      19631  0.0  0.2   9764  4732 tty1     R+   10:01   0:00 ps aux
100 processes are running
```

```bash
cat users.txt
```
```
root:x:0:0:root:/root:/bin/bash
sync:x:4:65534:sync:/bin:/bin/sync
dhcpcd:x:997:997:DHCP Client Daemon:/usr/lib/dhcpcd:/bin/false
hamza:x:1000:1000:hamza:/home/hamza:/bin/bash
```

```bash
awk -F: "{print \"User \" \$1 \" has UID \" \$3 \" and GID \" \$4}" /etc/passwd
```
```
User root has UID 0 and GID 0
User daemon has UID 1 and GID 1
User bin has UID 2 and GID 2
User sys has UID 3 and GID 3
User sync has UID 4 and GID 65534
User games has UID 5 and GID 60
User man has UID 6 and GID 12
User lp has UID 7 and GID 7
User mail has UID 8 and GID 8
User news has UID 9 and GID 9
User uucp has UID 10 and GID 10
User proxy has UID 13 and GID 13
User www-data has UID 33 and GID 33
User backup has UID 34 and GID 34
User list has UID 38 and GID 38
User irc has UID 39 and GID 39
User _apt has UID 42 and GID 65534
User nobody has UID 65534 and GID 65534
User systemd-network has UID 998 and GID 998
User dhcpcd has UID 997 and GID 997
User messagebus has UID 996 and GID 996
User systemd-resolve has UID 990 and GID 990
User _chrony has UID 989 and GID 989
User usbmux has UID 100 and GID 46
User polkitd has UID 988 and GID 988
User syslog has UID 101 and GID 103
User uuidd has UID 102 and GID 104
User tcpdump has UID 986 and GID 986
User tss has UID 985 and GID 985
User landscape has UID 103 and GID 106
User fwupd-refresh has UID 984 and GID 984
User hamza has UID 1000 and GID 1000
User sshd has UID 983 and GID 65534
```

```bash
awk "NR>1 {print \$1, \$11}" processes.log
```
```
root /usr/lib/systemd/systemd
root [kthreadd]
root [pool_workqueue_release]
root [kworker/R-rcu_gp]
root [kworker/R-sync_wq]
root [kworker/R-kvfree_rcu_reclaim]
root [kworker/R-slub_flushwq]
root [kworker/R-netns]
root [kworker/0:0H-kblockd]
root [kworker/u4:0-ext4-rsv-conversion]
root [kworker/R-mm_percpu_wq]
root [ksoftirqd/0]
root [rcu_preempt]
root [rcu_exp_par_gp_kthread_worker/0]
root [rcu_exp_gp_kthread_worker]
root [migration/0]
root [kprobe-optimizer]
root [idle_inject/0]
root [cpuhp/0]
root [kdevtmpfs]
root [kworker/R-inet_frag_wq]
root [rcu_tasks_kthread]
root [rcu_tasks_rude_kthread]
root [kauditd]
root [khungtaskd]
root [oom_reaper]
root [kworker/R-writeback]
root [kcompactd0]
root [ksmd]
root [khugepaged]
root [kworker/R-kblockd]
root [kworker/R-blkcg_punt_bio]
root [kworker/R-kintegrityd]
root [irq/9-acpi]
root [kworker/R-tpm_dev_wq]
root [kworker/R-ata_sff]
root [kworker/R-md_bitmap]
root [kworker/R-md_llbitmap_io]
root [kworker/R-md_llbitmap_unplug]
root [kworker/R-edac-poller]
root [kworker/R-devfreq_wq]
root [watchdogd]
root [kworker/R-quota_events_unbound]
root [kswapd0]
root [ecryptfs-kthread]
root [kworker/R-kthrotld]
root [kworker/R-acpi_thermal_pm]
root [scsi_eh_0]
root [kworker/R-scsi_tmf_0]
root [scsi_eh_1]
root [kworker/R-scsi_tmf_1]
root [kworker/u4:5-writeback]
root [kworker/R-mld]
root [kworker/R-ipv6_addrconf]
root [kworker/R-kstrp]
root [kworker/u5:0]
root [kworker/R-charger_manager]
root [scsi_eh_2]
root [kworker/R-scsi_tmf_2]
root [jbd2/sda2-8]
root [kworker/R-ext4-rsv-conversion]
root [kworker/R-kmpathd]
root [kworker/R-kmpath_handlerd]
root [kworker/R-cfg80211]
root [irq/18-vmwgfx]
root /bin/sh
root [kworker/R-ttm]
message+ @dbus-daemon
root /usr/bin/python3
root /usr/lib/snapd/snapd
root /usr/lib/systemd/systemd-logind
_chrony /usr/sbin/chronyd
root /usr/bin/python3
_chrony /usr/sbin/chronyd
root login
hamza /usr/lib/systemd/systemd
hamza (sd-pam)
hamza -bash
root [kworker/0:0-cgroup_release]
root [kworker/0:1-events]
root [kworker/u4:2-events_unbound]
root [kworker/0:1H-kblockd]
root /usr/sbin/cron
root /usr/sbin/multipathd
polkitd /usr/lib/polkit-1/polkitd
root /usr/libexec/udisks2/udisksd
systemd+ /usr/lib/systemd/systemd-resolved
root /usr/lib/systemd/systemd-journald
root /usr/libexec/upowerd
root /usr/libexec/fwupd/fwupd
root sshd:
root /usr/lib/systemd/systemd-udevd
root /usr/sbin/ModemManager
systemd+ /usr/lib/systemd/systemd-networkd
root [psimon]
syslog /usr/sbin/rsyslogd
root [psimon]
root [kworker/u4:1-events_unbound]
root [kworker/0:2-events]
hamza ps
100 
```

```bash
awk "NR>1 {sum += \$3} END {print \"Total CPU usage:  \" sum \"%\"}" processes.log
```
```
Total CPU usage:  0.6%
```
