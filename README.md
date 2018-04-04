# GiHhub-Activity-2

## Various Android versions

A list of various Android versions and their properties.

### 1.Android Oreo
Android "Oreo" (codenamed Android O during development) is the eighth major version of the Android operating system. It was first released as an alpha quality developer preview in March 2017 and released to the public on August 21, 2017.

It contains a number of major features, including notification grouping, picture-in-picture support for video, performance improvements and battery usage optimization, and support for autofillers, Bluetooth 5, system-level integration with VoIP apps, wide color gamuts, and Wi-Fi Aware. Android Oreo also introduces two major platform features: Android Go – a software distribution of the operating system for low-end devices – and support for implementing a hardware abstraction layer.

#### Features

* **User experience-**

Notifications can be snoozed, and batched into topic-based groups known as "channels". Android Oreo contains integrated support for picture-in-picture modes (supported in the YouTube app for YouTube Red subscribers). The "Settings" app features a new design, with a white theme and deeper categorization of different settings, while its ringtone, alarm and notification sound settings now contain an option for adding custom sounds to the list.The Android 8.1 update supports the display of battery percentages for connected Bluetooth devices, makes the notification shade slightly translucent, and dims the on-screen navigation keys in order to reduce the possibility of burn-in.

* **Android Go-**

A tailored distribution for low-end devices known as Android Go was unveiled for Oreo; it is intended for devices with 1 GB of RAM or less. This mode has platform optimizations designed to reduce mobile data usage (including enabling Data Saver mode by default), and a special suite of Google Mobile Services designed to be less resource- and bandwidth-intensive. The Google Play Store will also highlight lightweight apps suited for these devices. The operating system's interface is also modified, with the quick settings panel providing greater prominence to information regarding the battery, mobile data limit, and available storage, the recent apps menu using a modified layout and being limited to four apps (in order to reduce RAM consumption), and an API for allowing mobile carriers to implement data tracking and top-ups within the Android settings menu. Google Play Services was also modularized to reduce its memory footprint.

* **Security-**

Android Oreo re-brands automatic scanning of Google Play Store and sideloaded apps as "Google Play Protect", and gives the feature, as well as Find My Device (formerly Android Device Manager) higher prominence in the Security menu of the Settings app. As opposed to a single, system-wide setting for enabling the installation of apps from sources outside of the Google Play Store, this function is now implemented as a permission that can be granted to individual apps (i.e. clients for third-party app repositories such as Amazon Appstore and F-Droid). Verified boot now includes a "Rollback Protection" feature, which enforces a restriction on rolling back the device to a previous version of Android, aimed at avoiding a potential thief from bypassing security measures by installing a previous version of the operating system that doesn't have them in place.


### 2.Android Nougat
Android "Nougat" (codenamed Android N during development) is the seventh major version of the Android operating system. First released as an alpha test version on March 9, 2016, it was officially released on August 22, 2016, with Nexus devices being the first to receive the update. The LG V20 was the first smartphone released with Nougat.Nougat introduces notable changes to the operating system and its development platform, including the ability to display multiple apps on-screen at once in a split-screen view, support for inline replies to notifications, and an expanded "Doze" power-saving mode that restricts device functionality once the screen has been off for a period of time. Additionally, the platform switched to an OpenJDK-based Java environment and received support for the Vulkan graphics rendering API, and "seamless" system updates on supported devices.Nougat received positive reviews. The new app notification format received particular praise, while the multitasking interface was seen as a positive change, but reviewers experienced incompatible apps. Critics had mixed experiences with the Doze power-saving mode, but faster app installs and "tweaks" to the user interface were also reviewed positively.

#### Features

* **User experience-**

Nougat redesigns the notification shade, which now features a smaller row of icons for settings, replacing notification cards with a new "sheet" design, and allowing inline replies for notifications. This feature is implemented via existility on Android Wear. Multiple notifications from a single app can also be "bundled", and there is greater per-app control over notifications.A split-screen display mode was introduced for phones, in which two apps can be snapped to occupy halves of the screen. An experimental multi-window mode is also available as a hidden feature, where multiple apps can appear simultaneously on the screen in overlapping windows.

The "Doze" power saving mechanism introduced in Android Marshmallow was expanded to include a state activated when the device is running on battery and the screen has been off for a period of time but is not stationary. In this state, network activity is restricted, and apps are granted "maintenance windows" in which they can access the network and perform background tasks. As in Marshmallow, the full Doze state is activated if the device is stationary with its screen off for a period of time. A new "Data Saver" mode restricts background mobile data usage, and can trigger internal functions in apps that are designed to reduce bandwidth usage, such as capping the quality of streaming media.

* **Platform-**

In December 2015, Google announced that Android Nougat would switch its Java Runtime Environment from the defunct Apache Harmony to OpenJDK—the official open source implementation of the Java platform maintained by Oracle Corporation and the Java community. The Android Runtime (ART) now incorporates a profile-guided compilation system, utilizing a JIT compiler and profiling alongside its current ahead-of-time compiler to further optimize apps for a device's hardware and other conditions in the background.

Nougat introduces a system for enabling "seamless", automatic system updates, based upon and sharing some code with the implementation of similar functionality on Chrome OS. The system uses a pair of SquashFS partitions; the Android system executes from an "online" partition, while updates are applied in the background to a redundant "offline" partition. On the next boot following the installation of an update, the redundant partition is designated as active, and the device henceforth boots into the updated system. The previous system partition is kept as a backup in case of update failure, and to serve as the "offline" partition for the next update. This system removes the requirement for the device to reboot into the system recovery environment to apply the update (which prevents the device from being used until the update is complete) and also provides the ability for an update to be automatically rolled back in case of a failure. Due to the partitioning requirements of this system, existing devices will not support seamless updates. Additionally, due to the ART changes on Nougat, apps no longer need to be re-compiled upon the first boot after a system update.

* **Security-**

In response to the Stagefright family of bugs disclosed and fixed in 2015, several changes were made to harden the media stack against future vulnerabilities. Runtime integer overflow detection was implemented, preventing the majority of Stagefright-like programming bugs from becoming vulnerabilities, in addition to helping fix and prevent such bugs. Android's monolithic MediaServer process was redesigned to better adhere to the principle of least privilege. MediaServer is now split into several separate processes, each running in its own unprivileged sandbox, and granted only the permissions required for its task. For example, only the AudioServer can access Bluetooth, and libstagefright now runs within the MediaCodecService sandbox, which is only granted GPU access. Further constraints were placed on the media stack through seccomp.

Various mechanisms were enabled to reduce the possibility of malicious code being injected and/or executed inside the Linux kernel, including dividing kernel memory into logical segments for code and data, with page access permissions of read-only and no-execute as appropriate. The kernel was also restricted from directly accessing user space memory, and stronger stack protection was enabled in the GCC compiler to reduce stack smashing. To limit exposure of the kernel to potentially malicious code, perf was disabled by default, ioctl commands were restricted by SELinux, and seccomp-bpf was enabled to grant processes the ability to restrict system calls.

### 3.Android Marshmallow

Android "Marshmallow" (codenamed Android M during development) is the sixth major version of the Android operating system. First released as a beta build on May 28, 2015, it was officially released on October 5, 2015, with Nexus devices being the first to receive the update.Marshmallow primarily focuses on improving the overall user experience of its predecessor, Lollipop. It introduced a new permissions architecture, new APIs for contextual assistants (first used by a new feature "Now on Tap" to provide context-sensitive search results), a new power management system that reduces background activity when a device is not being physically handled, native support for fingerprint recognition and USB-C connectors, the ability to migrate data and applications to a microSD card, and other internal changes.

#### Features

* **User experience-**

A new "Assist" API allows information from a currently opened app, including text and a screenshot of the current screen, to be sent to a designated "assistant" application for analysis and processing. This system is used by the Google Search app feature "Google Now on Tap", which allows users to perform searches within the context of information currently being displayed on-screen. While the "Home" button was used in Android 5 to show available apps, the "Home" button is used now (together with a voice command) to generate on-screen cards which display information, suggestions, and actions related to the content. "Direct Share" allows Share menus to display recently used combinations of contacts and an associated app as direct targets.

"Adoptable storage" allows a newly inserted SD card or other secondary storage media to be designated as either "portable" or "internal" storage. "Portable" maintains the default behavior of previous Android versions, treating the media as a secondary storage device for storage of user files, and the storage media can be removed or replaced without repercussions, but is subject to access restrictions by apps. When designated as "Internal" storage, the storage media is reformatted with an encrypted ext4 file system, and is "adopted" by the operating system as the primary storage partition. Existing data (including applications and "private" data folders) are migrated to the external storage, and normal operation of the device becomes dependent on the presence of the media. Apps and operating system functions will not function properly if the adopted storage device is removed.

* **Platform-**

Android Marshmallow introduces a redesigned application permissions model; apps are no longer automatically granted all of their specified permissions at installation time. An opt-in system is now used, in which users are prompted to grant or deny individual permissions (such as the ability to access the camera or microphone) to an application when they are needed for the first time. Applications remember the grants, which can be revoked by the user at any time. The new permissions model is used only by applications developed for Marshmallow using its software development kit (SDK), and older apps will continue to use the previous all-or-nothing approach. Permissions can still be revoked for those apps, though this might prevent them from working properly, and a warning is displayed to that effect.

Marshmallow introduces new power management schemes known as "Doze" and "App Standby"; when running on battery power, a device will enter a low-power state if it is inactive and not being physically handled. In this state, network connectivity and background processing is restricted, and only "high-priority" notifications are processed. Additionally, network access by apps is deferred if the user has not recently interacted with the app. Apps may request a permission to exempt themselves from these policies, but will be rejected from Google Play Store as a violation of its "Dangerous Products" policy if their core functionality is not "adversely affected" by them.

