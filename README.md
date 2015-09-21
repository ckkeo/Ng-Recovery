__<center><big>New Generation - Recovery Image for android (Based on ClockworkMod 6 based / Advanced Edition)</big></center>__

.

__Home page__
http://forum.xda-developers.com/showthread.php?t=2201860

#### Building

Clone ng-recovery to bootable/ng-recovery folder

    git clone https://github.com/ckkeo/nr-recovery bootable/ng-recovery -b cm-11.0

Now build with RECOVERY_VARIANT flag set to ng-recovery:

    . build/envsetup.sh && lunch && mka -j3 recoveryimage RECOVERY_VARIANT=ng-recovery

or

    export RECOVERY_VARIANT=ng-recovery
    . build/envsetup.sh && lunch && mka -j3 recoveryimage

or

    add to device BoardConfig.mk:
        RECOVERY_VARIANT := ng-recovery
    and run:
        build/envsetup.sh && lunch && mka -j3 recoveryimage
