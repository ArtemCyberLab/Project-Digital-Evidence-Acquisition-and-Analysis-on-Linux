Project: Digital Evidence Acquisition and Analysis on Linux

In this project, I focused on the process of acquiring digital evidence and subsequent analysis on a Linux operating system. The task was to create a disk image, verify its integrity, mount it, and analyze the contents.

First, I configured the system to log all my actions. This is an important practice in investigations or analysis. I used the history command to track all the commands executed and also recorded the results using the script utility.

Next, I proceeded with data acquisition from the disk. I used the lsblk command to determine which devices were connected to the system, including virtual devices and those that weren't mounted yet. One of these devices was the disk from which I wanted to create an image. I used the dc3dd command to create an exact copy of the disk. During this process, I specified parameters such as the source disk and the target file for the image. The command was executed successfully, and a 1.1 GB image was created.

After the image was created, I checked its integrity using the md5sum command to ensure the extraction process was error-free. I compared the hash value with the original to confirm that they matched.

The next step was to mount the image for further analysis. I created a mount point using the mkdir command and then used the mount command to attach the image to the system. After mounting, I could view the directory structure and files inside the image. At this stage, I continued the analysis, checking for important data within the image.

During the analysis, I found the flag.txt file, which contained the flag required to complete the task. This confirmed that the data acquisition process was done correctly, and the obtained data was valuable.

In the end, the entire process — from creating the image to analyzing the data — was successful, and I was able to achieve the goal by extracting important information from the created image.
