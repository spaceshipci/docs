# How to Use Jenkins Job on Spaceship CI

Jenkins jobs are use to run your task. Here is how to use Jenkins Job at Spaceship CI.

## Creating a job

Each user allowed to have max 5 Jenkins Job. To create a new Job you can follow this instruction:
- Login to Jenkins
- Click "New item"
- Fill the job name. Please to attach yout username on the job name to avoid being confused with other user's job
- Select "Freestyle Project"
- Then, add your build script by clicking "Build" Tab
- Click "Add build step"
- Click "Execute shell"
- After a big textbix appears, you can start adding your build Script. Please see examples bellow


## Build script for Downloading ROM Source

In this case, let's say i am going to build PixelExpereince, Build script used are:
```
#!/bin/bash

cd /home/YOUR_USERNAME
umask 0000

# Operation
mkdir PE
cd PE
repo init -u https://github.com/PixelExperience/manifest -b twelve
repo sync -c -j$(nproc --all) --force-sync --no-clone-bundle --no-tags
```


Then, click Save at the bottom of the page and click "Build Now"

## Build script for Building ROM
Still same with above, we will use PixelExperience as reference. And let;s say i am going to build it for lavender.

```
#!/bin/bash

cd /home/YOUR_USERNAME
umask 0000

# Operation
cd PE
. build/envsetup.sh
lunch aosp_lavender-userdebug
make bacon -j16
```

## Additional

You just have to edit the script starting from ```# Operation``` to the end as you need. You can also compile kernel/ applications, etc.

Also, you shouldn't modify anything except ```YOUR_USERNAME``` from commands above ```# Operation```
