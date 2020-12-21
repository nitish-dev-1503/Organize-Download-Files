**Cronjob** is a system utility and a time-based scheduler in Unix based operating systems _(for Windows Task Scheduler under administrative tools can be used)_. It is used to execute background tasks on a routine basis. 
Cron requires a file called crontab which contains the list of tasks to be executed at a particular time. All these jobs are executed in the background at the specified time.

* To view all the cronjobs running on your system, go to terminal and run the following command:
### crontab -l
It will show the list of jobs in the crontab file. 
* To add a new cron job we need to edit the crontab file using the following command:
### crontab -e
It will open the crontab file in the default text editor, where you can add jobs by writing commands in the following format:
### * * * * * command_to_execute
* Here each * symbol from left to right specifies the following:
    - Min (0–59)
    - Hour (0–23)
    - Day of Month (1–31)
    - Month (1–12)
    - Day of Week (0–6) (0–6 are Sunday to Saturday)


* To make automation.py a cronjob which runs at 0 min every hour we can add following command in the crontab file
    0 */1 * * * cd ~/Downloads/ && python3 automation.py >> ~/Downloads/Log/log.txt

