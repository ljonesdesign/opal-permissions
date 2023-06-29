## Setting up File Access Permissions on OPAL Server

Before you (or anyone else) can view your files in a web browser, you must change the access permissions for your home directory on opal. If these permissions are set incorrectly, anyone trying to view your webpage will see a Forbidden error rather than your content.
Follow these instructions to set the correct permissions:

Open an SSH connection to Opal.
 
On Windows, you'll need to use an SSH client for this; on MacOS and Linux, you can open a Terminal window, enter 
						
<pre>ssh your_onyen@opal.ils.unc.edu</pre> <p>and then enter your password when prompted.
					
Once you've connected, you should see a command prompt like this:
						
```
[your_onyen@opal ~] $
```
					
Type
						
```
chmod 711 .
```
						
with <b>both the space and the period.</b> If you get a "missing operand" error, make sure you included the space and the period at the end.

				
### Viewing Your Webpage
After you have uploaded your files and set the correct permissions, your webpage will be viewable at 

```
https://opal.ils.unc.edu/~onyen/
```

This will take you to the index page in your public_html folder; you can also navigate directly to other pages or subfolders you've added, such as 

```
https://opal.ils.unc.edu/~onyen/my_folder/my_page.html
```
