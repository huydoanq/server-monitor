# server-monitor
Some scripts to monitor server status and send email

##How to setup

- Run setup.sh
- [Config SSMTP to send email](http://www.nixtutor.com/linux/send-mail-with-gmail-and-ssmtp/)
- In terminal run:
```shel
chmod +x your-python-file.py
```
- Scheduling the job with crontab
```shel
crobtab -e
```
then add:
```shel
*/5 * * * * /home/vagrant/job/job.py https://goplay.la https://gtoken.com
```
This command will check run the job each 5 minutes
