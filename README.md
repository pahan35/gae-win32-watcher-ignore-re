## Info

This repository contains file with implemented support for ignoring.

## Patch applying
To apply patch you need to replace original file or add changes from the patch.
If you install GAE via installer to default folder, required file should be placed on path `C:\Program Files (x86)\Google\Cloud SDK\google-cloud-sdk\platform\google_appengine\google\appengine\tools\devappserver2\win32_file_watcher.py`


## Version info
Origin GAE version info where this file was modified
```
Google Cloud SDK 215.0.0
app-engine-python 1.9.75
app-engine-python-extras 1.9.74
bq 2.0.34
cloud-datastore-emulator 2.0.2
core 2018.09.04
gsutil 4.33
```

## Bugs
Can't appropriately setup --watcher_ignore_re value cause it fails on `C:/Program Files (x86)/Google/Cloud SDK/google-cloud-sdk/platform/google_appengine/google/appengine/tools/devappserver2/metrics.py:185`
on attempt of serialization of regex values
```
Google Cloud SDK 228.0.0
app-engine-python 1.9.80
app-engine-python-extras 1.9.74
bq 2.0.39
cloud-datastore-emulator 2.0.2
core 2018.12.07
gsutil 4.34
```
To fix this bug please apply changes with this commit on `metrics.py`
