+ The script is designed to automate the scanning process of files uploaded on MobSF - the pen-testing app, also for static and dynamic analysis - and give an outlook of critical and high-level threats in the app.
+ It uses the MobSF scan api endpoint to send an http POST request using the hash of the file, file_name, scan_type, and API-key to receive a JSON file.

Running the script
-----------------
+ You can run the script with the target files in the current directory or other directories in the file system. Simply apply the right file path as shown.
+ you can scan multiple files at once to get a breakdown of the issues of the uploaded files.
```Bash
googlecloud@m076er:~/Documents/Projects/Internship-Tasks$ ./auto-scan.py /home/m076er/Downloads/'Diva Application.apk' /home/m076er/Downloads/'Pen test.apk'
```
Prompt
------
+ Once you run the script, the following prompt shows. In the event, input the extension as shown.
```Bash
Enter scan type (apk/ipa): apk
```
Sample output
-------------
+ Here is what you can expect as output for the above scanned files
```Bash
2 dangerous warnings in permissions analysis
=================
0 warnings in permissions analysis
-----------------
1 high/critical warnings in certificate analysis
=================
1 warnings in certificate analysis
-----------------
0 high/critical warnings in manifest analysis
=================
3 warnings in manifest analysis
-----------------
0 high/critical warnings in code analysis
=================
5 warnings in code analysis
-----------------
File: /home/vboxuser/Downloads/NBM merchant.apk
+++++++++++++++++++++++++++++++++++++
Enter scan type (apk/ipa): apk
7 dangerous warnings in permissions analysis
=================
0 warnings in permissions analysis
-----------------
2 high/critical warnings in certificate analysis
=================
1 warnings in certificate analysis
-----------------
0 high/critical warnings in manifest analysis
=================
10 warnings in manifest analysis
-----------------
0 high/critical warnings in code analysis
=================
13 warnings in code analysis
-----------------
File: /home/m076er/Downloads/Pen test.apk
+++++++++++++++++++++++++++++++++++++
