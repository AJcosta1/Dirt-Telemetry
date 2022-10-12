# Dirt-Telemetry

1-Open the folder with the configuration file
Make sure that Dirt Rally is currently not running but was started at least once!

Open the folder C:\Users\YOURUSERNAME\Documents\My Games\Dirt Rally\hardwaresettings (YOURUSERNAME must be replaced with your current username).

Open the file hardware_settings_config.xml with a texteditor (e.g. Notepad)

2-Find the motion_platform entry in the textfile
Search in the opened file for the entry motion_platform. You may find an entry as shown on the screenshot.

It is also possible, that the entry is already in use (enabled="true"), or that no entry is in the file.

3-Update the textfile
We now change the entry to:

<udp enabled="true" extradata="3" ip="127.0.0.1" port="20777" delay="1" extradata="0" / >

(The port, here 20777 must be consistend with the port in the SIM Dashboard Server application).

If no entry <udp...> is available, you can just create one as described above.

If an entry <udp enabled="true" ip="....> is already defined, you must adapt it as described.

Now save the textfile (Make sure that the file ending is .xml and NOT .xml.txt!)Afterwards you can start the game.
