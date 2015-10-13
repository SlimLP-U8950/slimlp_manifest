cm12.1_manifest
================

Local Manifest to build CM12.1 for the Huawei U8950 (Honor Pro)

Build Instructions
-----------------------------------------------------------------------------

1. Initialize repo using the CM12.1 manifest
    
        repo init -u git://github.com/CyanogenMod/android.git -b cm-12.1

2. Add my local manifest

        curl --create-dirs -L -o .repo/local_manifests/cm_huawei.xml -O -L https://raw.github.com/U8950-Projects/manifest/cm-12.1/cm_huawei.xml

3. Then sync up the repositories
 
        repo sync

4. Build the ROM

        brunch u8950
