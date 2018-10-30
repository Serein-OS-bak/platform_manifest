sereinOS

To get started with Serein, you'll need to get familiar with [Git and Repo](http://source.android.com/source/using-repo.html).

Syncing Source
--------------
To initialise local sereinOS repositories in your machine:

    repo init -u https://github.com/Serein-OS/platform_manifest -b pie-release

Then to sync up:

    repo sync -c -jx --force-sync --no-clone-bundle --no-tags

To Build:

    . build/envsetup.sh && lunch serein_<device>-userdebug && make bacon
