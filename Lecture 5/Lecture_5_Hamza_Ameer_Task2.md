# Lecture 5 - Task 2

```bash
ps aux | grep hamza
```
```
root         851  0.0  0.3   8760  5680 ?        Ss   06:19   0:00 login -- hamza
hamza       1253  0.0  0.7  22200 12972 ?        Ss   06:19   0:00 /usr/lib/systemd/systemd --user
hamza       1260  0.0  0.2  23012  4136 ?        S    06:19   0:00 (sd-pam)
hamza       1287  0.0  0.3   8856  5872 tty1     Ss   06:19   0:00 -bash
hamza       1820  0.0  0.2   9764  4672 tty1     R+   06:45   0:00 ps aux
hamza       1821  0.0  0.1   6716  2644 tty1     S+   06:45   0:00 grep --color=auto hamza
```

```bash
ps aux | grep -E "^hamza\b"
```
```
hamza       1253  0.0  0.7  22200 12972 ?        Ss   06:19   0:00 /usr/lib/systemd/systemd --user
hamza       1260  0.0  0.2  23012  4136 ?        S    06:19   0:00 (sd-pam)
hamza       1287  0.0  0.3   8856  5872 tty1     Ss   06:19   0:00 -bash
hamza       1831  0.0  0.2   9764  4676 tty1     R+   06:46   0:00 ps aux
hamza       1832  0.0  0.1   6716  2684 tty1     S+   06:46   0:00 grep --color=auto -E ^hamza\b
```

```bash
ps aux | grep -v "^root"
```
```
USER         PID %CPU %MEM    VSZ   RSS TTY      STAT START   TIME COMMAND
systemd+     467  0.0  0.8  22632 14640 ?        Ss   06:18   0:00 /usr/lib/systemd/systemd-resolved
systemd+     606  0.0  0.7  21464 12316 ?        Ss   06:18   0:00 /usr/lib/systemd/systemd-networkd
message+     770  0.0  0.3   9132  5736 ?        Ss   06:19   0:00 @dbus-daemon --system --address=systemd: --nofork --nopidfile --systemd-activation --syslog-only
polkitd      782  0.0  0.4 306448  8292 ?        Ssl  06:19   0:00 /usr/lib/polkit-1/polkitd --no-debug --log-level=notice
_chrony      859  0.0  0.3  20556  6464 ?        S    06:19   0:00 /usr/sbin/chronyd -n -F 1
syslog       866  0.0  0.3 220548  6212 ?        Ssl  06:19   0:00 /usr/sbin/rsyslogd -n -iNONE
_chrony      881  0.0  0.1  12096  2408 ?        S    06:19   0:00 /usr/sbin/chronyd -n -F 1
hamza       1253  0.0  0.7  22200 12972 ?        Ss   06:19   0:00 /usr/lib/systemd/systemd --user
hamza       1260  0.0  0.2  23012  4136 ?        S    06:19   0:00 (sd-pam)
hamza       1287  0.0  0.3   8856  5872 tty1     Ss   06:19   0:00 -bash
hamza       1842  0.0  0.2   9764  4672 tty1     R+   06:46   0:00 ps aux
hamza       1843  0.0  0.1   6716  2648 tty1     S+   06:46   0:00 grep --color=auto -v ^root
```

```bash
ps aux | grep -vE "kworker|irq"
```
```
USER         PID %CPU %MEM    VSZ   RSS TTY      STAT START   TIME COMMAND
root           1  0.2  0.9  24700 16148 ?        Ss   06:18   0:03 /usr/lib/systemd/systemd --switched-root --system --deserialize=53
root           2  0.0  0.0      0     0 ?        S    06:18   0:00 [kthreadd]
root           3  0.0  0.0      0     0 ?        S    06:18   0:00 [pool_workqueue_release]
root          15  0.0  0.0      0     0 ?        I    06:18   0:00 [rcu_preempt]
root          16  0.0  0.0      0     0 ?        S    06:18   0:00 [rcu_exp_par_gp_kthread_worker/0]
root          17  0.0  0.0      0     0 ?        S    06:18   0:00 [rcu_exp_gp_kthread_worker]
root          18  0.0  0.0      0     0 ?        S    06:18   0:00 [migration/0]
root          19  0.0  0.0      0     0 ?        S    06:18   0:00 [kprobe-optimizer]
root          20  0.0  0.0      0     0 ?        S    06:18   0:00 [idle_inject/0]
root          21  0.0  0.0      0     0 ?        S    06:18   0:00 [cpuhp/0]
root          22  0.0  0.0      0     0 ?        S    06:18   0:00 [kdevtmpfs]
root          24  0.0  0.0      0     0 ?        I    06:18   0:00 [rcu_tasks_kthread]
root          25  0.0  0.0      0     0 ?        I    06:18   0:00 [rcu_tasks_rude_kthread]
root          26  0.0  0.0      0     0 ?        S    06:18   0:00 [kauditd]
root          27  0.0  0.0      0     0 ?        S    06:18   0:00 [khungtaskd]
root          28  0.0  0.0      0     0 ?        S    06:18   0:00 [oom_reaper]
root          32  0.0  0.0      0     0 ?        S    06:18   0:00 [kcompactd0]
root          33  0.0  0.0      0     0 ?        SN   06:18   0:00 [ksmd]
root          34  0.0  0.0      0     0 ?        SN   06:18   0:00 [khugepaged]
root          46  0.0  0.0      0     0 ?        S    06:18   0:00 [watchdogd]
root          48  0.0  0.0      0     0 ?        S    06:18   0:00 [kswapd0]
root          49  0.0  0.0      0     0 ?        S    06:18   0:00 [ecryptfs-kthread]
root          52  0.0  0.0      0     0 ?        S    06:18   0:00 [scsi_eh_0]
root          54  0.0  0.0      0     0 ?        S    06:18   0:00 [scsi_eh_1]
root         278  0.0  0.0      0     0 ?        S    06:18   0:00 [scsi_eh_2]
root         309  0.0  0.0      0     0 ?        S    06:18   0:00 [jbd2/sda2-8]
root         404  0.0  0.0      0     0 ?        S    06:18   0:00 [psimon]
root         411  0.0  1.0  50396 17140 ?        S<s  06:18   0:00 /usr/lib/systemd/systemd-journald
root         451  0.0  0.5 279492  9644 ?        SLsl 06:18   0:00 /usr/sbin/multipathd -d -s
systemd+     467  0.0  0.8  22632 14640 ?        Ss   06:18   0:00 /usr/lib/systemd/systemd-resolved
root         471  0.0  0.9  41228 15428 ?        Ss   06:18   0:00 /usr/lib/systemd/systemd-udevd
root         532  0.0  0.0      0     0 ?        S    06:18   0:00 [psimon]
systemd+     606  0.0  0.7  21464 12316 ?        Ss   06:18   0:00 /usr/lib/systemd/systemd-networkd
root         769  0.0  0.1   2888  2012 ?        Ss   06:19   0:00 /bin/sh /usr/lib/systemd/scripts/chronyd-starter.sh -n -F 1
message+     770  0.0  0.3   9132  5736 ?        Ss   06:19   0:00 @dbus-daemon --system --address=systemd: --nofork --nopidfile --systemd-activation --syslog-only
root         776  0.0  1.7  46844 30220 ?        Ss   06:19   0:00 /usr/bin/python3 /usr/bin/networkd-dispatcher --run-startup-triggers
root         779  0.0  0.2   7060  3432 ?        Ss   06:19   0:00 /usr/sbin/cron -f -P
polkitd      782  0.0  0.4 306448  8292 ?        Ssl  06:19   0:00 /usr/lib/polkit-1/polkitd --no-debug --log-level=notice
root         786  0.0  2.5 1812844 42708 ?       Ssl  06:19   0:01 /usr/lib/snapd/snapd
root         789  0.0  0.5  18596  9696 ?        Ss   06:19   0:00 /usr/lib/systemd/systemd-logind
root         793  0.0  0.9 543324 15160 ?        Ssl  06:19   0:00 /usr/libexec/udisks2/udisksd
root         826  0.0  0.4  10744  7756 ?        Ss   06:19   0:00 sshd: /usr/sbin/sshd -D [listener] 0 of 10-100 startups
root         851  0.0  0.3   8760  5680 ?        Ss   06:19   0:00 login -- hamza
_chrony      859  0.0  0.3  20556  6464 ?        S    06:19   0:00 /usr/sbin/chronyd -n -F 1
root         861  0.0  1.9 126116 32988 ?        Ssl  06:19   0:00 /usr/bin/python3 /usr/share/unattended-upgrades/unattended-upgrade-shutdown --wait-for-signal
syslog       866  0.0  0.3 220548  6212 ?        Ssl  06:19   0:00 /usr/sbin/rsyslogd -n -iNONE
_chrony      881  0.0  0.1  12096  2408 ?        S    06:19   0:00 /usr/sbin/chronyd -n -F 1
root         891  0.0  0.8 391608 14160 ?        Ssl  06:19   0:00 /usr/sbin/ModemManager
hamza       1253  0.0  0.7  22200 12972 ?        Ss   06:19   0:00 /usr/lib/systemd/systemd --user
hamza       1260  0.0  0.2  23012  4136 ?        S    06:19   0:00 (sd-pam)
hamza       1287  0.0  0.3   8856  5872 tty1     Ss   06:19   0:00 -bash
root        1718  0.0  0.6 318676 11520 ?        Ssl  06:34   0:00 /usr/libexec/upowerd
hamza       1853  0.0  0.2   9764  4688 tty1     R+   06:46   0:00 ps aux
```
