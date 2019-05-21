# restic-backup

Generate a config file, use the sample in the ```conf``` directory.
It may be a good idea to backup the config file in a safe place.

Use the systemd units to plan the backup jobs.
The given config sample would result in a backup job for "test1".

```
systemctl enable --now restic-backup@test1.timer
systemctl enable --now restic-prune@test1.timer
```

