1. Put the shutdown script in /Scripts dir
2. Setup a task in Task Scheduler to run the script at pc start

In Task Scheduler
Create new task
Name: ShutdownIFTT
Choose:
Run whether user is logged on or not
Check:
Run with highest privileges
Hidden
Select:
Configure for: Widnows 10

On Triggers tab
Create new trigger
Select:
Begin the task: At startup
OK

On Actions tab
Create new Action
Select: 
Action: Start a program
Choose:
Program/script:
C:\Windows\System32\WindowsPowerShell\v1.0\powershell.exe
Add arguments:
C:\Scripts\ShutdownIFTTT.ps1
OK

OK
Type in PC user password

Restart PC
