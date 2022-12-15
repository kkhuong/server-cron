# Setup
1. To set up, on the user's root directory, clone this repository. Then rename this repository to `cron`.
2. Change the folder and file permissions to 777
3. Edit the files if necessary to the correct path

# Current Cron Tab File
```
*/5 * * * * /home/kkhuong/cron/backup_notebooks.sh >/dev/null 2>&1
*/5 * * * * /home/kkhuong/cron/backup_django.sh >/dev/null 2>&1
@reboot /home/kkhuong/cron/start_notebooks.sh >/dev/null 2>&1
@reboot /home/kkhuong/cron/start_django.sh >/dev/null 2>&1
```

Run `crontab -e` to edit the crontab file.
