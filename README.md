# hdhomerun record systemd service
## Starting hdhomerun_record under Debian Linux with Systemd
### Place the service file and configure it
* service file is located in this repository under ```image```
* Place the ```hdhomerun_record.service``` file in ```/etc/systemd/system directory```
* Edit the path to the ```WorkingDirectory``` in the service file
* Edit the ```ExecStart``` absolute path to the executable
* Edit the ```User``` and ```Group```

### Start the service
* kill off any existing ```hdhomerun_record``` execution.

  example:
    ```
    pkill hdhomerun_record_x64
    ```
* Use ```systemctl``` to start the service

    ```
    systemctl daemon-reload
    systemctl start hdhomerun_record.service
    ```

### Getting status

   ```
   systemctl status hdhomerun_record.service
   ```
or
   ```
   /opt/hdhomerun/hdhomerun_record status
   ```

Substitute for ```/opt/hdhomerun``` with your path to the
```hdhomerun_record``` program.
