slimlp_manifest
================

Local Manifest to build SlimLP for the Huawei U8950 (Honor Pro)

Build Instructions
-----------------------------------------------------------------------------

1. Initialize repo using the SlimLP manifest
    
        repo init -u git://github.com/SlimRoms/platform_manifest.git -b lp5.1

2. Add my local manifest

        curl --create-dirs -L -o .repo/local_manifests/slimlp_huawei.xml -O -L https://raw.github.com/SlimLP-U8950/slimlp_manifest/lp5.1/slimlp_huawei.xml

3. Then sync up the repositories
 
        repo sync

4. Apply patches

        sh device/huawei/msm7x27a-common/patches/apply.sh

5. Initialize the build environment

        source build/envsetup.sh
    
6. Build the ROM

        brunch u8950

