_________          _______ _________ _______       _______  _______  _______           _______ __________________         
/\\__   __/|\     /|(  ____ \\__   __/(  ____ )     (  ____ \(  ____ \(  ____ \|\     /|(  ____ )\__   __/\__   __/|\     /|
/ /   ) (   | )   ( || (    \/   ) (   | (    )|     | (    \/| (    \/| (    \/| )   ( || (    )|   ) (      ) (   ( \   / )
/ /    | |   | (___) || (__       | |   | (____)|     | (_____ | (__    | |      | |   | || (____)|   | |      | |    \ (_) /
/ /     | |   |  ___  ||  __)      | |   |     __)     (_____  )|  __)   | |      | |   | ||     __)   | |      | |     \   /  
/ /      | |   | (   ) || (         | |   | (\ (              ) || (      | |      | |   | || (\ (      | |      | |      ) (   
/ /       | |   | )   ( || (____/\___) (___| ) \ \__     /\____) || (____/\| (____/\| (___) || ) \ \_____) (___   | |      | |   
\/        )_(   |/     \|(_______/\_______/|/   \__/_____\_______)(_______/(_______/(_______)|/   \__/\_______/   )_(      \_/   
                                            (_____)                                                                       
Cloudcat POC

//Overview
This script is an initial POC to set up a cloud server automatically with Hashcat, Seclist and OpenCL drivers to enable hashcat to run on the cloud with minimal user set up. I have tested this on Vultr's hosting platform and evidence of this can be seen either on my blog or youtube.

//Usage
To use this first access your cloud server (either through SSH or online terminal)
Use;
git clone https://github.com/theirsecurity/cloudcat
Identify the script that applies to your cloud server then use
chmod +x <BASH_SCRIPT_NAME>
./<BASH_SCRIPT_NAME>

Once this has run you need to copy over the hash file you want to use with hascat, i did this using SCP to the /root/hashes folder e.g
scp /<INSERT_LOCAL_HASH_DIRECTORY> <CLOUD_USERNAME>@<CLOUD_IP>:/hashes

//Next Steps
Over the next few days there will be more updates to this as a GPU Script will be added once tested and also showing some benchmarks on my site and YT.

//Contact
marc@theirsecurity.com