# hdhomerun
##Starting hdhomerun_record under Debian Linux with Systemd
###Place the service file and configure it
*Place the hdhomerun_record.service file in /etc/systemd/system directory.
*Edit the path to the WorkingDirectory.
*Edit the ExecStart absolute path to the executable.
*Edit the User and Group
###Start the service
*kill of any existing hdhomerun_record
**example
**pkill hdhomerun_record_x64
*systemctl daemon-reload
*systemctl start hdhomerun_record.service
###Getting status
*systemctl status hdhomerun_record.service
*/opt/hdhomerun/hdhomerun_record status
		Substitute your path to the hdhomerun_record program
