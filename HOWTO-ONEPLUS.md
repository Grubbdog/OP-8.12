How to install on Oneplus 3T?
------
1. clone fork to /data/ and make sure it's named openpilot:
```
cd /data/ && rm -rf openpilot ; git clone https://github.com/cfranhonda/openpilot.git -b devel-0.8.8-OP3T --depth=1
```

2. run command:
```
cd /data/openpilot/scripts/ && ./oneplus_update_neos.sh
```

3. Let it download and complete it update, after a couple of reboot, your screen will then stay in fastboot mode.

4. In fastboot mode, select use volume button to select to `Recovery mode` then press power button.

5. In Recovery mode, tap `apply update` -> `Choose from emulated` -> `0/` -> `update.zip` -> `Reboot system now`
   
6. You should be able to boot into openpilot, if touch screen is not working, try to reboot again.
