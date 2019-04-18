# wine-patch

A collection of wine patch for my self compile version of wine.

Support wine-staging 4.6.

To apply patches use `git apply *.patch` or `git am *.patch`.

# Patch Lists

    - 0001-patches/0001_staging-config.patch
    Toggle upstream CSMT implementation patch from https://github.com/wine-staging/wine-staging/pull/60

    - 0001-patches/0002_use_clock_monotonic.patch
    ntdll, server: Never use CLOCK_MONOTONIC_RAW
    Using CLOCK_MONOTONIC avoids a kernel call.

    - 0001-patches/0003_enable_stg_shared_mem_def.patch
    ntdll: Enable STAGING_SHARED_MEMORY by default.

    - 0001-patches/0004_large_address_aware-staging.patch
    ntdll/loader: add support for overriding IMAGE_FILE_LARGE_ADDRESS_AWARE Staging version.

    - 0001-patches/0005_plasma_systray_fix.patch
    winex11.drv: Fix system tray on KDE Plasma.
    from https://github.com/Tk-Glitch/PKGBUILDS/blob/master/wine-tkg-git/wine-tkg-patches/plasma_systray_fix.patch

    - 0001-patches/0008_FS_bypass_compositor.patch
    Proton's Bypass compositor patch.

    - 0001-patches/0010-Added-support-for-Win-1-and-2-applications.patch
    Add support for Windows 1.x and 2.x applications.
    This is a patch file version of https://github.com/TransmissionZero/Wine

    - 0002-winevdm/*.patch
    Patches ported from the winevdm project (wine on Windows) version 0.7.0, https://github.com/otya128/winevdm

    - 0003-wine-thaiapi/*.patch
    Patch set to add Thai language API from Windows 3.1/9x Thai Edition support to wine.
    From https://github.com/kytulendu/wine-thaiapi
