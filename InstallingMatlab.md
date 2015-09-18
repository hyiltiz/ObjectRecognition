===== Installing MATLAB =====
=============================

If you're an NYU student and you have a personal laptop, follow the instructions below to install MATLAB on your laptop. This will give you a "network license" which means you can only use MATLAB while you are on the NYU network (e.g. "nyu" wifi), or by using the NYU VPN to access the NYU network while off-campus (VPN instructions at www.nyu.edu/its/nyunet/offcampus/vpn/). Students unfortunately do not qualify for a standalone license.

If you're not an NYU student, follow your home department's instructions for MATLAB. If your home department does not provide MATLAB, talk to us.

==== New install (CNS and Psych) ====
=============================

To install a fresh copy of MATLAB, the easiest way is to physically go to a departmental machine, and use a USB stick to copy the files. You can also ask your classmates who have already downloaded the files to lend you their USB stick.

If you would like to try downloading the MATLAB files from outside CNS, you can try copying them from the gateway machine at janus.cns.nyu.edu using an SSH-based file-transfer app (e.g. Cyberduck) but this is more difficult than the USB-stick method.

The information in this section can be found at http://www.cns.nyu.edu/unixadmin/#september7-2012
  
== Mac, Unix, Linux ==
=============================

  * On a departmental unix machine, find the most recent version of MATLAB.
    * For the mac version, you can look in Finder for the Network Applications folder or go to /share/Applications/
    * For the Unix/Linux version, go to /share/erda/matlab8.3 (or whatever the most recent version is)
  * Copy the app to your computer via a USB stick.
    * On a mac, put the app in your applications folder.
    * On Unix/Linux, put the files in /usr/local/bin or anywhere else you are used to installing programs.
  * In MATLAB.app/licenses/, rename network.lic.nyu to network.lic and remove all other license files in there.
    * On a mac you can view the contents of the matlab app bundle by clicking on "show package contents" while it is highlighted.
  * Leave the app on your USB stick and bring it to the installation help session if you want to help your classmates!

== Windows ==
=============================

On windows, you cannot just copy the app; instead, you need to copy the installer and then run the installer. See the install instructions at http://www.cns.nyu.edu/unixadmin/standalone-mat/2INSTALL-WIN. Using your USB device, copy the install media from /share/Public/Distros/Windows along with the network.lic file.

==== Existing install, new license (CNS and Psych) ====
=============================

If you already have MATLAB installed on your computer, but you were using a previous institution's license, you will need a new license.

The following text should be inserted into a file named "network.lic" and put into your MATLAB licenses folder. 

  # MATLAB license passcode file for use with FLEXlm. NYU servers
  SERVER lm0.es.its.nyu.edu 005056B10009 27000
  SERVER lm1.es.its.nyu.edu 005056B1000A 27000
  SERVER lm2.es.its.nyu.edu 005056B1000C 27000
  USE_SERVER

Recent copies of this file can be found on CNS departmental computers at ''MATLAB.app/licenses/'' or ''/share/erda/matlab/licenses/''

Try looking in these places for your licenses folder, where you should put the file:
  * Wherever your MATLAB is installed, look under that directory: $MATLAB\licenses
  * C:\Users\<username>\AppData\Roaming\MathWorks\MATLAB\R2008a_licenses (for Windows Vista and higher)
  * /home/<username>/.matlab/R2008a_licenses (for Unix/Linux/Mac)
  * /Users/<username>/.matlab/R2012b_licenses (Mountain Lion OS 10.8)

==== Other NYU students ====
=============================

Students from the NYU Medical School should be able to get licenses from the Medical School. Unfortunately the mathtools instructors do not have NYUMC accounts so we cannot verify the following methods.

Try the following link to access the Medical School keyserver:
http://nyumc.net.ezproxy.med.nyu.edu/nyu/mcit/services/software/keyserver.jsp

Other NYU departments also provide site licenses. If you are unable to install MATLAB from your department, please talk to the TAs.

===== Other ways of accessing MATLAB =====
=============================

On-campus, you can use MATLAB on one of the departmental machines in CNS and Psychology.

From a browser, you can use MATLAB by accessing NYU's "virtual computer lab". You must first install a Citrix ICA plugin before the virtual computer lab will work. See http://www.nyu.edu/its/vcl/ for more information about the Virtual Computer Lab. 

These are useful options if at any point you don't have a laptop you can use (you don't own a laptop, or yours is broken).

===== Installation help sessions =====
=============================

We ask all students to have MATLAB installed before the first Friday lab. If you are having difficulty getting MATLAB installed on your own, the TA's will hold a help session to get you started installing MATLAB. Please bring a USB stick to the installation session if you own one.

===== Departmental help desk =====
=============================

The TA's are available as your first point of help, but if you're really stuck you can try contacting your department's help desk:
  * CNS shop: http://www.cns.nyu.edu/info/
  * Psychology shop: http://psych.nyu.edu/shop/contact.html
  * School of Medicine: www.med.nyu.edu/it

