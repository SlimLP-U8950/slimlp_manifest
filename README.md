rr5.1_manifest
================

Local Manifest to build ResurrectionRemix 5.1 for the Huawei U8950 (Honor Pro)

Build Instructions
-----------------------------------------------------------------------------

1. Initialize repo using the RR5.1 manifest
    
        repo init -u https://github.com/ResurrectionRemix/platform_manifest.git -b lollipop5.1

2. Add my local manifest

        curl --create-dirs -L -o .repo/local_manifests/rr_huawei.xml -O -L https://raw.github.com/U8950-Projects/manifest/rr5.1/rr_huawei.xml

3. Then sync up the repositories
 
        repo sync

4. Build the ROM

        brunch u8950
