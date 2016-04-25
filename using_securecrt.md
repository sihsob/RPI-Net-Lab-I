SecureCRT
=========

Throughout Networkign Lab 1, you will need a program called SecureCRT.  You can
ask your TA about where to get the software and how to install it.  We have also
provided some scripts to help automate the setup and end processes that you will
need each lab.

## Start of Each Lab
1. connect.py
  1. Automatically opens up a channel to connect to all the switches and
       routers of your pod.
  2. Your pod will be assigned to you on the first lab.  If someone is
       using your pod, then you will need to ask your TA to assign you
       another temporary pod.
  3. Click on the 'scripts'??? option on the menu bar and open up the
       file.  You will then be prompted to enter your pod number and the
       password provided to connecting to the pods.
  4. New tabs will be opened with connections to all the switches and
       routers.  If you see a red marking with a slash through it, then it
       most likely means someone else is using your pod already.
2. loadall.py
  1. Automatically loads in all your saved configurations to the proper
       switches and routers.
  2. Assuming you have saved files of your running configurations, click on
       the 'scripts'??? option on the menu bar and open the file.  You will
       then be prompted to type in the full path to where you have saved the
       files.  Make sure you provide the exact path.
  3. If any issues arise when running this script, make sure that you
       have enabled all the devices.  Meaning, you have typed in `en<CR>`.
       Otherwise, ask your TA for help.

## Ending Lab
1. saveall.py
  1. Automatically saves your configurations for each device as text files to
       specified folder.
  2. Click on the 'scripts'??? option on the menu bar and open the file.  You
       will then be prompted to type in the full path to where you want to save
       the files.  Make sure you provide the full path to the folder.  Also make
       sure that you are in enabled mode for all devices. So your prompt should
       only look like `'hostname'>#`.
  3. If any issues arise, ask your TA for help.
2. eraseall.py
  1. Automatically erases all your configurations for each device.
  2. MAKE SURE YOU RUN THIS SCRIPT EVERYTIME BEFORE YOU LEAVE LAB.
  3. Click on the 'scripts'??? option on the menu bar and open the file.  The
       script should automatically execute.  Make sure that you are in enabled
       mode for all the devices.  This can take awhile to fully erase
       everything, but it should be all right if you close (disconnect) from
       SecureCRT once you start the erase script.  It will continue even if you
       are not connected.
  4. If any issues arise, ask your TA for help.
