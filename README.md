<h1 align="center">Multi Cloud Transfer 🔥</h1>
<p><b>MCT Tool is a Google Colab based Jupyter notebook uses Rclone and other popular engines (aria, yt-dlp, libtorrent, 7zip etc) to manipulate & tranfer data (even simultaneously) between two or more cloud services without utilizing one's bandwidth or system resources. While performing given task, MCT Tool saves important user session or configuration files in safe (encrypted) format to make things easier next time when user perform same task requiring same configuration or session files.</b></p>
<div align="center"><a href="https://colab.research.google.com/github/TheCaduceus/Multi-Cloud-Transfer-Tool/blob/main/Rclone.ipynb" target="_parent"><img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open In Colab"/></a></div>
<h2><b>📑 INDEX</b></h2>
<p><b><a href="https://github.com/TheCaduceus/Multi-Cloud-Transfer-Tool#multi-cloud-transfer-advanced-">⚡MCT Tool</a></b></p>
<p><b><a href="#whats-new">🆕What's New!</a></b></p>
<p><b><a href="#-notice">⛔NOTICE</a></b></p>
<p><b><a href="#before-you-start">🔌Before you Start</a></b></p>
<p><b><a href="#multi-cloud-transfer">♻️Multi Cloud Transfer</a></b></p>
<p><b><a href="#using-service-accounts">🪀Using Service Accounts</a></b></p>
<p><b><a href="#special-add-ons">🪄Special Add-ons</a></b></p>
<p><b><a href="#direct-download-links">->📥Direct Download Links</a></b></p>
<p><b><a href="#download-links-from-txt-file">->📃Download Links from txt file</a></b></p>
<p><b><a href="#youtube-videosplaylist--other-sites">->🎥YouTube videos/playlist & other sites</a></b></p>
<p><b><a href="#magnet-links-dl">->🧲Magnet Links DL</a></b></p>
<p><b><a href="#%EF%B8%8Ftorrent-files-dl">->🗃️Torrent Files DL</a></b></p>
<p><b><a href="#upload-files-to-anonymous-platforms">->📤Upload Files/Folder to Anonymous Platforms</a></b></p>
<p><b><a href="#%E2%93%9C%EF%B8%8Fmega-links-dl">->Ⓜ️MEGA Link DL</a></b></p>
<p><b><a href="#%EF%B8%8Fuup-dump">->🗑️UUP DUMP</a></b></p>
<p><b><a href="#pack--extract-filesfolder">📦Pack & Extract Files/Folder</a></b></p>
<p><b><a href="#modes-of-transfer">🚅Modes of Transfer</a></b></p>
<p><b><a href="#-safe-or-not-">🔐Safe or not?</a></b></p>
<p><b><a href="#need-help">⛑Need help!</a></b></p>
<p><b><a href="#%EF%B8%8Fcredits--thanks">❤️Credits & Thanks</a></b></p>
<h2><b>🆕What's New!</b></h2>
<h4><b>1.Package Upgrades:<b></h4>
  <p><b>  ->Rclone upgraded to <code>v1.61.1</code></b></p>
  <p><b>  ->yt-dlp upgraded to <code>v2023.01.16</code></b></p>
  <p><b>  ->LibTorrent upgraded to <code>v2.0.8</code></b></p>
  <p><b>  ->NoteBook upgraded to <code>v5.0.2</code></p></b>
  <p><b>  ->Installer upgraded to <code>v5.0.1</code></b></p>
<h4><b>2.New changes:<b></h4>
  <p><b>  ->Bulk links download without .txt file.</b></p>
  <p><b>  ->'Upload to Anonfiles' feature renamed to 'Upload to Anonymous platforms' and supports 12 new platforms.</b></p>
  <p><b>  ->Upload folder support with link harvest feature on 12 Anonymous file sharing platform.</b></p>
  <p><b>  ->MEGA Credentials will now be saved in json format instead of txt file and in encrypted format instead of plan text.</b></p>
  <p><b>  ->Seperate direct link generators are removed.</b></p>
  <p><b>  ->New check to block any unknown file to be executed received from any input field provided by the Tool.</b></p>
  <p><b>  ->MCT Tool is 7x faster & smaller then ever!</b></p>
<h4><b>3.Bug fixes:<b></h4>
  <p><b>  ->Slow code execution problem caused by recent changes made by Google Colab team in <code>google.colab</code> library or at colab's backend.</b></p>
  <p><b>  ->Let string be string don't interpret, basically MCT Tool was sometime producing unknown errors/outputs caused due to some special signs that a given particular path may or may not contain.</p></b>
  <p><b>  ->Typos in paths (drive or root) of Rclone file causing error in uploading/saving it.</p></b>

<p><b><a href="https://github.com/TheCaduceus/Multi-Cloud-Transfer-Tool/releases">Show Update History</a></b></p>
<h2><b>⛔ NOTICE</b></h2>
<h4><b>1.Never use MCT Tool for processing any illegal content. (Read Google Colab's policy)</b></h4>
<h4><b>2.Only execute .sh files from trusted authors and never blindly else can cause serious problems.</b></h4>
<h4><b>3.Damage caused due to any type of unofficial edits or forks should not be reported to official contributors.</b></h4>
<!--- Step Area Begin --->
<h2><b>🔌Before you Start</b></h2>
<h4><b>1.First connect Google Drive to enable MCT Tool to save/retrive its configuration files.</b></h4>
<h4><b>Options:</b></h4>
<p><b><code>FORCE_REMOUNT</code>: Forcefully remount Google Drive.</b></p>
<p><b><code>CUSTOM_MOUNT_POINT</code>: Choose different path for mounting Google Drive.</p>
<p><b><code>DEBUG_MODE</code>: To enable or disable DEBUG Mode.</b></p>
<img src="https://user-images.githubusercontent.com/87380104/185793270-75d9960d-6edb-4697-a9d6-8008529f1dc1.png">
<h4><b>2.Fetch your previous saved MCT Tool configuration files from Google Drive->My Drive->MCT Config folder to stop wasting your time by creating them again and again@</b></h4>
<h4><b>Options:</b></h4>
<p><b><code>Custom_Import_Path</code>: Scan a custom path (or directory) give by user for usable MCT Configuration files.</p>
<p><b><code>Custom_Export_Path</code>: Export all your MCT Configuration files to a gives path.</b></p>
<img src="https://user-images.githubusercontent.com/87380104/215341558-a385ffd6-4a57-4062-8144-7434161bfb8a.png">
<h4><b>4.Use Service Accounts with MCT Tool to avoid Google Drive's transfer limits, read "Using Service Accounts" Section to learn how to.</b></h4>
<h4><b>Options:</b></h4>
<p><b><code>Upload_Service_Accounts</code>: Upload new Service Accounts.</b></p>
<p><b><code>Save_To_MyDrive</code>: Save new/existing Service Accounts to Google Drive-> My Drive</b></p>
<img src="https://user-images.githubusercontent.com/87380104/215531572-161939bd-48ab-425c-b7be-dd4a06071dea.png" alt="Using SA">
<h4><b>5.Ability to delete your Files/Folder/Directory with different purge methods.</b></h4>
<h4><b>Options:</b></h4>
<p><b><code>delete</code>: Delete the content of folder or single file.</b></p>
<p><b><code>purge</code>: Delete whole directory and leaving nothing behind.</b></p>
<p><b><code>rmdir</code>: Completely delete the given path.</b></p>
<p><b><code>rmdirs</code>: Remove any empty directories under the path.</b></p>
<img src="Img/35.png" alt="Purge Options">
<h4><b>6.Add-ons are additional features which are not offered by Rclone officially but created by two or more engines.</b></h4>
<img src="https://user-images.githubusercontent.com/87380104/169866802-3f5594e6-b1b1-4125-b5c7-17084694ab1d.png">
<h4><b>7.MCT Tool supports packing & extracting files or folders in variety of formats and transfer simultaneously.</b></h4>
<img src="https://user-images.githubusercontent.com/87380104/215342192-23c603bb-74b1-412c-84fd-981fa9aab642.png">

<h2><b>🪝Multi Cloud Transfer</b></h2>
<p><b>MCT Tool uses Rclone, one of the best command line tool for data transfer & data management tool for performing any task involving transfer of data, that means it can transfer any amount of data from/to any cloud service without utilizing one's own bandwidth or system resources.</b></p>
<h4><b>1.Before we procced! I recommend to either create/upload or fetch your Rclone Config file to Google Colab using below methods! Creating and fetching will automatically place the file in correct location!</b></h4>
<h4><b>Options:</b></h4>
<p><b><code>Custom_Import_Path</code>: Scan a custom path (or directory) given by user for usable MCT Configuration files.</p>
<p><b><code>Custom_Export_Path</code>: Export all your MCT Configuration files to a gives path.</b></p>
<img src="Img/24.png">
<h4><b>2.Once you done creating or fetching the config files! just run the cell named <code>Connect to Cloud Accounts</code> and it will automatically detect your config file and will show you the available remotes, follow on-screen instructions to mount them</b></h4>
<h4><b>Options:</b></h4>
<p><b><code>Custom_Mount_Point</code>: To set Custom Mount Point.</b></p>
<p><b><code>Custom_Cache_Dir</code>: To set Custom Cache Directory.</p>
<img src="https://user-images.githubusercontent.com/87380104/185793654-f658a130-c9d3-4fa6-b2e3-e53535b1f99e.png">
<h4><b>3.After mounting those remotes or cloud Accounts, now click on the file icon as shown in the image and then navigate to the folder where you mounted your remoted (default folder is <code>drives</code>) and you will see the names of remotes or cloud account which you mounted previously!</b></h4>
<img src="Img/26.png">
<h4><b>4.Now copy the file or folder path which needs to be copied and then right click on the file or folder and select <code>Copy Path</code> option from the list.</b></h4>
<img src="Img/27.png">
  <h4><b>5.After that! paste the path of file or folder in <code>Source</code> field and again go to <code>File Icon->drives</code> and open the cloud Account into which you want to transfer files/folders and copy its path! You can either directly copy the path of cloud Account or of any folder inside it and paste the path in <code>Destination</code> field.</b></h4>
<img src="Img/28.png">
<h4><b>6.Choose the transfer mode trough which you want to transfer your data! refer to "<a href="#modes-of-transfer">🚅Modes of Transfer</a>" below to learn about all of them.</b></h4>
<h4><b>9.Finally! run the code by pressing play button to initiate transfer.</b></h4>
<h2><b>🪀Using Service Accounts</b></h4>
<h4><b>Service Accounts are just like normal Google Account and thus have same upload or download limits as Google Account which is 750GB upload and 10TB download. They are used to act on behalf of a Google Account and hence we can use them to prevent hitting Google Drive transfer limits by creating them in a bulk amount.</b></h4>
  <h4><b>1.Don't have Service Accounts?<a href="https://github.com/TheCaduceus/CloneBot_V2#-making-service-accounts" alt="Creating SA"> Create Here</a></b></h4>
  <h4><b>2.After creating! make the zip of <code>accounts</code> folder which have 100 Json files and keep its name as <code>accounts.zip</code>.</b></h4>
  <h4><b>3.Now back to Google Colab screen and select saving options for Service Accounts to use them without uploading them again next time.</b></h4>
  <h4><b>Options:</b></h4>
  <p><b><code>Upload_Service_Accounts</code>: Upload new Service Accounts.</b></p>
  <p><b><code>Save_To_MyDrive</code>: Save new/existing Service Accounts to My Drive->MCT Config folder.</b></p>
  <img src="https://user-images.githubusercontent.com/87380104/215347396-83aaeb07-dc85-4b6d-9743-f1a1ce72cd60.png">
  <h4><b>4.After it! click the file icon, then open <code>accounts</code> folder and right click on anyone Json file and select <code>Copy path</code>.</b></h4>
  <img src="Img/32.png">
  <h4><b>5.Run the <code>Create/Edit/Delete Rclone Config File</code> and paste the path in <code>service_account_file</code> during creating remote for Google Drive.</b></h4>
  <img src="Img/33.png">
  <h2><b>🪄Special Add-ons</b></h2>
  <h4><b>Add-ons are the special functions not provided by any single engine and are made by combining two or more engines while performing any particular task simultaneously. Each of these functions (or simply add-ons) are explained below with their steps to use.</b></h4>
  <img src="https://user-images.githubusercontent.com/87380104/169764820-a9678d13-4708-4232-9c65-2cfb682f4bec.png">

  <h3><b>📥Direct Download Links:</b></h3>
  <h4><b>Function enables to download files or data from single or multiple direct download links to any cloud. It uses Aria engine to deliver best and fastest performance possible. You can also download two or more links at same time with this.</b></h4>
  <h4><b>Just put your direct download links in Source field and then enter the Destination path to where you want to download data. You can enter multiple Direct Download links in the source field by separating them using <code>,</code> between each link in the following format: </b></h4>
  <p><b><code>Link1,Link2</code></b></p>
  <img src="https://user-images.githubusercontent.com/87380104/169864446-a8c1de39-8121-4451-9d85-416452dc57fc.png">
  <h3><b>📃Download Links from txt file:</b></h3>
  <h4><b>Functions enables to download all links written in a given txt file. This function is useful when we have too many links and it will take too much time separate each link with <code>,</code>.</b></h4>
  <h4><b>User just need to upload the txt file containing the download links to any cloud or in runtime provided by Google Colab then have to provide its path in Source field and Destination path in Destination field to where you want to download the data. Best format to arrange links in txt file: </b></h4>
  <p><b><code>Link1</code></b></p>
  <p><b><code>Link2</code></b></p>
  <p><b><code>Link3</code></b></p>
  <img src="https://user-images.githubusercontent.com/87380104/169865084-b2bad643-e1e8-4565-8ec7-cae651bd9e1f.png">
  <h3><b>🎥YouTube videos/playlist & other sites</b></h3>
  <h4><b>Function gives the flexibility to download YouTube Videos or Playlist and videos from other supported sites directly to any cloud. It uses <code>yt-dlp</code> which downloads everything is maximum quality. You can download two or more videos which are not in same playlist or even two separate playlists at once. Refer to <a href="https://github.com/yt-dlp/yt-dlp" alt="yt-dlp">yt-dlp documentation</a> for more information.</b></h4>
  <h4><b>Just provide the YouTube link of video or playlist or link to videos located on other website (Non-DRM Protected) in <code>Source</code> field and Destination path in <code>Destination</code> field to where you want to download it. You can separate the link of videos or playlist by providing space between each in following format:</b></h4>
  <p><b><code>VideoLink1</code> <code>VideoLink2</code></b></p>
  <p><b><code>PlaylistLink1</code> <code>PlaylistLink2</code></b></p>
  <p><b><code>VideoLink1</code> <code>PlaylistLink1</code></b></p>
  <img src="https://user-images.githubusercontent.com/87380104/169865516-cd07abd2-bc78-40f1-8356-75f1960db86a.png">
  <h3><b>🧲Magnet Links DL:</b></h3>
  <h4><b>Function allow anyone to download torrent using magnet link directly into any cloud with high speed. It uses LibTorrent which is a lightweight powerful BitTorrent client. User can download multiple magnet links at once, just keep the <code>Source</code> field empty.</b></h4>
  <h4><b>Provide the Destination path in <code>Destination</code> field where all downloaded torrent files will be copied and run the code. User can provide as many magnet link as you can but only 1 magnet link per input box and hit enter! once you done adding magnet links, just type <code>Exit</code> and it will start downloading it.</b></h4>
  <img src="https://user-images.githubusercontent.com/87380104/169769919-fcc52d17-3b1c-4bb7-ba28-c29960d00b56.png">
  <h3><b>🗃️Torrent Files DL:</b></h3>
  <h4><b>Function gives ability to download torrent from <code>.torrent</code> files, user can provide as many torrent files as much it want. This function also uses LibTorrent to deliver fast download speed.</b></h4>
  <h4><b> have to provide <code>Destination</code> path to where all downloaded torrent data will be moved and torrent file through <code>Choose file</code> option. Once you provided torrent file you want to download then click <code>Cancel Upload</code> then it will start downloading torrent for you.</b></h4>
  <img src="https://user-images.githubusercontent.com/87380104/169771367-677c9dad-fcfe-41f9-b77c-476e77c23f69.png">
  <h3><b>📤Upload Files to Anonymous Platforms</b></h3>
    <h4><b>Function allow one to upload files or folder to 12 supported anonymous file sharing platforms and harvest all generated links in <code>.txt</code> file, officially none of these platform support 'folder upload' & 'link harvest' feature which sometimes makes thing defficult like when we need to share multiple files but MCT Tool uses 'for loop' after detecting a given path as 'folder' to continously upload files availabe in given folder and provides option to export all generated links in <code>.txt</code> file to make things more easier.</b></h4>
  <h4><b>1.For this, just provide the required path (file or folder) in source field and follow on-screen instruction.</b></h4>
  <h3><b>Ⓜ️MEGA Links DL:</b></h3>
  <h4><b>Function downloads MEGA Link with or without your using MEGA Account to directly any cloud.</b></h4>
  <h4><b>1.As stated above! user can use MEGA Account and MCT tool will save its credentials in safe format automatically for future use. Enter MEGA Link in <code>Source</code> field and Destination Path in <code>Destination</code> field where MEGA link needs to be downloaded.</b></h4>
  <h4><b>2.If destination path is not provided then downloaded files will be moved to <code>downloads</code> folder in connected runtime (Temporary storage).<b></h4>
    <h3><b>🗑️UUP DUMP:</b></h3>
    <h4><b>Function enables to collect files mentioned in <code>uup_download_linux.sh</code> files and upload them to any cloud mentioned as <code>Destination</code>. It makes work super easy for users making<code>ISO</code> files using <code>.sh</code> file given by <a href="https://uupdump.net">UUP DUMP</a> or any other websites.</b></h4>
    <h4><b>1.First download any UUP file in your device, then either upload it to Google Colab or any other cloud.</b></h4>
  <h4><b>2.Now copy the path of <code>uup_download_linux.sh</code> file or path of folder which contaning <code>.sh</code> file and paste it as <code>Source</code>, now mount or connect any cloud using steps given above and copy the path and paste it as <code>Destination</code>.</b></h4>
    <img src="https://user-images.githubusercontent.com/87380104/179364517-b28b76bc-5ba5-4c3c-8be6-8c2835551d7a.png">
    <h4><b>3.Once done! run the cell and let program download all files.</b></h4>
  <h2><b>📦Packing & Extracting Files/Folder</b></h2>
  <h4><b>MCT Tool comes with the ability to pack or extract any files or folder in variety of formats with or without Password Protection while moving the data from one cloud to another cloud. What you need is just Source Path which needs to be packed or extracted and destination path where you need the final result, so let's learn how to use this function.</b></h4>
  <h4><b>1.First mount remotes between which you need to transfer the packed or extracted data. Please read STEP 2 of "🪝Multi Cloud Transfer" section to learn how to do that!</b></h4>
  <h4><b>2.Now Get both source path & destination path.</b></h4>
  <h4><b>3.After it! choose the action which needs to be done with the source path and then enter following Details:</b></h4>
    <p><b><code>Packed_File_Name</code>: Enter the name of Packed or Zipped file if zipping/packing anything.</b></p>
    <p><b><code>Source_Path</code>: The Path of Data which needs to be processed.</b></p>
    <p><b><code>Destination_Path</code>: The Path on which you want the final output.</b></p>
  <h4><b>4.Then run cell to start your given task.</b></h4>

<h2><b>🚅Modes of Transfer</b></h2>
<h4><b>As this project use Rclone as a base! and Rclone support multiple options to help you move or clean your Data, in this Project those options are known as Modes. Here is the list of the Modes that this Project supports:</b></h4>
    <h4><b><code>Copy</code>: Copy files from source to dest, skipping identical files.</b></h4>
    <h4><b><code>Copyto</code>: This can be used to upload single files to other than their current name.</b></h4>
    <h4><b><code>CopyURL</code>: Download a URL's content and copy it to the destination without saving it in temporary storage.</b></h4>
    <h4><b><code>Move</code>: Moves the contents of the source directory to the destination directory.</b></h4>
    <h4><b><code>Moveto</code>: If source:path is a file or directory then it moves it to a file or directory named dest:path.</b></h4>
    <h4><b><code>Check</code>: Checks the files in the source and destination match. It compares sizes and hashes (MD5 or SHA1) and logs a report of files that don't match. It doesn't alter the source or destination.</b></h4>
    <h4><b><code>Sync</code>: Sync the source to the destination, changing the destination only. Doesn't transfer files that are identical on source and destination, testing by size and modification time or MD5SUM. Destination is updated to match source, including deleting files if necessary (except duplicate objects, see below).</b></h4>
    <h4><b><code>Bisync</code>: Bisync provides a bidirectional cloud sync solution in rclone. It retains the Path1 and Path2 filesystem listings from the prior run. On each successive run it will:</b></h4>
    <h4><b><code>Cat</code>: Rclone cat sends any files to standard output.</b></h4>
    <h4><b><code>CleanUp</code>: Clean up the remote if possible. Empty the trash or delete old file versions. Not supported by all remotes.</b></h4>
    <h4><b><code>ls</code>: List all the objects in the path with size and path.</b></h4>
    <h4><b><code>lsd</code>: List all directories/containers/buckets in the path.</b></h4>
    <h4><b><code>lsl</code>: List all the objects in the path with size, modification time and path.</b></h4>
    <h4><b><code>test makefile</code>: Make files with random contents and of any size.</b></h4>
    <h4><b><code>md5sum</code>: Produce an md5sum file for all the objects in the path.</b></h4>
    <h4><b><code>sha1sum</code>: Produce a sha1sum file for all the objects in the path.</b></h4>
    <h4><b><code>size</code>: Return the total size and number of objects in path.</b></h4>
    <h4><b><code>genautocomplete</code>: Output shell completion scripts for rclone.</b></h4>
    <h4><b><code>gendocs</code>: Output markdown docs for rclone to the directory supplied.</b></h4>
    <h4><b><code>obscure</code>: Obscure password for use in the rclone.conf.</b></h4>
    <h4><b><code>tree</code>: List the contents of the remote in a tree like fashion.</b></h4>
  <p><b>Following Modes can easily cause Data Loss:</b></p>
    <h4><b><code>Delete</code>: Remove the files in path.</b></h4>
    <h4><b><code>Purge</code>: Will delete whole Directory and leaving nothing behind.</b></h4>
    <h4><b><code>rmdir</code>: Completely Delete the given path.</b></h4>
    <h4><b><code>rmdirs</code>: Remove any empty directories under the path.</b></h4>
<h2><b>🔐 Safe or Not?</b></h2>
<h4><b>1.MCT Tool saves all important credentials like MEGA Credetials in encrypted format as json file in private MCT-Config folder (MyDrive) and hence follow common security standards.</b></h4>
<h4><b>2.Program automatically moderates & block all unknown files provided during additional input field & hence never touch them to prevent any unknown behaviour.</b></h4>
<h2><b>⛑Need help!</b></h2>
<h4><b>Telegram Channel:<a href="https://t.me/TheCaduceusOfficial"> Subscribe</a></b></h4>
<h4><b>Send personal meesage on Telegram<a href="https://telegram.me/HelpAutomatted_Bot"> here</a>.</b></h4>
<h2><b>❤️Credits & Thanks</b></h2>
<p><b><a href="https://github.com/TheCaduceus">Dr.Caduceus</a>: For making this project and guide.</b></p>
<p><b><a href="https://rclone.org/">Rclone</a>: The backbone of this powerful project.</b></p>
