# automount

> Reads the /etc/auto_master file and mounts `autofs` on the appropriate mount points to trigger on-demand mounting of directories. Essentially, it's a way to manually initiate the system's automounting process.
> Note: You'll most likely need to run with `sudo` if you don't have the necessary permissions.

- Run automount, flush the cache(-c) beforehand, and be verbose(-v) about it (most common use):

`automount -cv`

- Automatically unmount after 5 minutes of inactivity (timeout):

`automount -t 300`

- Unmount(-u) anything previously mounted by automount and/or defined in /etc/auto_master:

`automount -u`


