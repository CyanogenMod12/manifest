manifest
========

Local Manifest to build CyanogenMod for the Huawei G510/Y300

Build Instructions
-----------------------------------------------------------------------------

1. Initialize repo using the CyanogenMod manifest
    
        repo init -u git://github.com/CyanogenMod/android.git -b cm-12.0

2. Add my local manifest

        mkdir .repo/local_manifests
        Copy huawei.xml to .repo/local_manifests

3. Then sync up the repositories
 
        repo sync

4. Initialize the build environment

        source build/envsetup.sh
    
5. Build the ROM

        For G510:
            brunch u8951
        For Y300:
            brunch u8833