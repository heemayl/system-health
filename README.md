## System health monitoring and notifying program for GNU/Linux

#### Monitors load average, memory usage and disk usage of the system
 against given respective thresholds (given via environmment variables);
 generates report and sends that via mail. Suitable for running via
 system startup script or via `cron`.

---

##### Required programs:

- `gawk`  (GNU `awk`)
- `mailx`

---

##### Installation/Run:

- Clone the repository (`git clone git@gitlab.com:heemayl/system-health.git`) or download the repository
- Run `system_health_checker_notifier.sh` with modified environment variables (see the script)
- If you're using `systemd` as service manager, leverage the `systemd` service unit file `system-health-systemd.service` (change the script path in the `ExecStart` directive)

---

