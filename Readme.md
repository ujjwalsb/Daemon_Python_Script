1. After writing your "script.sh" file place it in the "/etc/init.d" directory

2. Make sure that it has the full permission of 777

3. Place your executable (python) script file in the exact location where you have mentioned in "script.sh"
	For my case-
		DIR=/usr/local/bin
		DAEMON=/$DIR/script.py

4. To avoid any future problems please make sure that your executable python scripts can run on a terminal, also it has the full permission.
	For my case-
		$ python3 script.py

5. After this followup in the command line or terminal from any location.
	$ sudo /etc/init.d/script.sh start
	$ sudo /etc/init.d/script.sh stop
	$ sudo /etc/init.d/script.sh restart

This should perform your desired task.