<h1 align="center">MCT Tool 🔥</h1>
<p><b>👋 Hello there! Welcome to Multi Cloud Transfer Tool (MCT Tool), a Google Colab based Jupyter Notebook that uses Rclone & other popular engines like yt-dlp, aria, libtorrent and 7Zip etc to manipulate & tranfer data (even simultaneously) between two or more cloud services without utilizing one’s own bandwidth or system resources. Sounds awesome, right? 😎

But wait, there’s more! MCT Tool also saves important user session or configuration files in safe (encrypted) format to make work easier next time when user perform same task requiring same configuration or session files. No need to remember those pesky passwords or settings ever again! 🙌

MCT Tool is powered by Rclone, one of the best command line tool for data transfer & data management. It can transfer any amount of data from/to any cloud service without breaking a sweat 💦. It’s like having your own personal cloud assistant that does all the work for you while you sit back and relax ☕.

We use our own <a href="https://cdn.thecaduceus.eu.org" alt="CDN">Content Delivery Network</a> to remotely control general code behaviour and <a href="https://cryptography.thecaduceus.eu.org" alt="Cryptography-API">Cryptography-API</a> to encrypt user provided strings.</b></p>
<div align="center"><a href="https://colab.research.google.com/github/TheCaduceus/Multi-Cloud-Transfer-Tool/blob/main/Rclone.ipynb" target="_parent"><img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open In Colab"/></a></div>


> **Warning**: MCT Tool currently have no active maintainer at the moment, so development of new features is currently stale. For this reason, MCT Tool only receiving bug fixes and minor changes to prevent depreciation. Backend & APIs used by MCT Tool will work as usual.

<h2><b>📑 INDEX</b></h2>
<p><b><a href="#mct-tool-">⚡MCT Tool</a></b></p>
<p><b><a href="#-notice">⛔NOTICE</a></b></p>
<p><b><a href="#before-you-start">🔌Before you start</a></b></p>
<p><b><a href="#multi-cloud-transfer">♻️Multi Cloud Transfer</a></b></p>
<p><b><a href="#using-service-accounts">🪀Using Service Accounts</a></b></p>
<p><b><a href="#special-add-ons">🪄Special Add-ons</a></b></p>
<p><b><a href="#direct-download-links">->📥Direct Download Links</a></b></p>
<p><b><a href="#download-links-from-txt-file">->📃Download links from txt file</a></b></p>
<p><b><a href="#youtube-videosplaylist--other-sites">->🎥YouTube videos/playlist & other sites</a></b></p>
<p><b><a href="#%EF%B8%8Ftorrent-dl-specific-files-support">->🗃️Torrent DL: (Specific files support)</a></b></p>
<p><b><a href="#upload-files-to-anonymous-platforms">->📤Upload Files/Folder to Anonymous Platforms</a></b></p>
<p><b><a href="#%E2%93%9C%EF%B8%8Fmega-links-dl">->Ⓜ️MEGA Link DL</a></b></p>
<p><b><a href="#%EF%B8%8Fuup-dump">->🗑️UUP DUMP</a></b></p>
<p><b><a href="#packing--extracting-filesfolder">📦Pack & Extract Files/Folder</a></b></p>
<p><b><a href="#gofile-integration">📂GoFile Integration</a></b></p>
<p><b><a href="#modes-of-transfer">🚅Modes of Transfer</a></b></p>
<p><b><a href="#need-help">⛑Need help!</a></b></p>
<p><b><a href="#%EF%B8%8Fcredits--thanks">❤️Credits & Thanks</a></b></p>
<h2><b>⛔ NOTICE</b></h2>
<h4><b>1.Never use MCT Tool for processing any illegal content (<a href="https://research.google.com/colaboratory/faq.html">Read official FAQ</a>). Since Colab provides flexibility to connect own runtime or server, developers can add features which may or may not be allowed by Colab on runtimes provided by them.</b></h4>
<h4><b>2.Only execute .sh files from trusted authors and never blindly else can cause serious problems like leakage of credentials or API Tokens. Always prefer using official notebook and features provided by original developers.</b></h4>
<h4><b>3.Damage caused due to any type of unofficial edits or forks should not be reported to official contributors. Any error like temporary runtime errors from Colab's side should be reported to Colab team instead of notebook developers, while any report of errors in notebook's code is welcome.</b></h4>
<h4><b>4.Prefer commonly used browsers (MS EDGE & Chrome) to access Colab and verify your browser have javascript & pop-ups enabled else you are mostly likely going to tackle an error. Some browsers (specially MS EDGE & Brave) provides additional specific content & trackers blocker, which can affect the overall working so make sure you disable it for Colab. Extensions are also capable of changing your browser behaviour and can cause same errors.</b></h4>
<!--- Step Area Begin --->
<h2><b>🔌Before you start</b></h2>
<h4><b>1.First connect Google Drive to enable MCT Tool to save/retrieve its configuration files.</b></h4>
<h4><b>Options:</b></h4>
<p><b><code>FORCE_REMOUNT</code>: Forcefully remount Google Drive.</b></p>
<p><b><code>CUSTOM_MOUNT_POINT</code>: Choose different path for mounting Google Drive.</p>
<p><b><code>DEBUG_MODE</code>: To enable or disable DEBUG mode.</b></p>
<img src="https://cdn.thecaduceus.eu.org/MCT/img/1.png" alt="1">
<h4><b>2.Retrieve your previous saved MCT Tool configuration files from Google Drive->My Drive->MCT Config folder to stop wasting your time by setting them again!</b></h4>
<h4><b>Options:</b></h4>
<p><b><code>Custom_Import_Path</code>: Scan a custom path (or directory) given by user for usable MCT Tool configuration files.</p>
<p><b><code>Custom_Export_Path</code>: Export all your MCT configuration files to a gives path.</b></p>
<img src="https://cdn.thecaduceus.eu.org/MCT/img/2.png" alt="2">
<h4><b>4.Use service accounts with MCT Tool to avoid Google Drive's transfer limits, read "Using Service Accounts" section to learn how to.</b></h4>
<h4><b>Options:</b></h4>
<p><b><code>Upload_Service_Accounts</code>: Upload new service accounts on runtime.</b></p>
<p><b><code>Save_To_MyDrive</code>: Save new service accounts to Google Drive -> My Drive. This will overwrite existing service accounts.</b></p>
<img src="https://cdn.thecaduceus.eu.org/MCT/img/3.png" alt="3">
<h4><b>5.Ability to delete your files/folder/directory with different purge methods.</b></h4>
<h4><b>Options:</b></h4>
<p><b><code>delete</code>: Delete the content of folder or single file.</b></p>
<p><b><code>purge</code>: Delete whole directory and leave nothing behind.</b></p>
<p><b><code>rmdir</code>: Completely delete the given path.</b></p>
<p><b><code>rmdirs</code>: Remove any empty directories under the path.</b></p>
<img src="https://cdn.thecaduceus.eu.org/MCT/img/4.png" alt="4">
<h4><b>6.Add-ons are additional features which are not offered by Rclone or any other engine officially but created by MCT Tool developers.</b></h4>
<img src="https://cdn.thecaduceus.eu.org/MCT/img/5.png" alt="5">
<h4><b>7.MCT Tool supports packing & extraction of files or folders in variety of formats and transfer simultaneously.</b></h4>
<img src="https://cdn.thecaduceus.eu.org/MCT/img/6.png" alt="6">

<h2><b>🪝Multi Cloud Transfer</b></h2>
<p><b>MCT Tool uses Rclone, one of the best command line tool for data transfer & data management for performing any task involving transfer of data, that means it can transfer any amount of data from/to any cloud service without utilizing one's own bandwidth or system resources.</b></p>
<h4><b>1.Before we procced, we recommend to either create/upload or retrieve your Rclone config file (<code>rclone.conf</code>) to Colab using below methods. Creating and retrieving will automatically place the file in correct location.</b></h4>
<h4><b>Options:</b></h4>
<p><b><code>Custom_Import_Path</code>: Scan a custom path (or directory) given by user for usable MCT Configuration files.</p>
<p><b><code>Custom_Export_Path</code>: Export all your MCT Tool configuration files to a gives path.</b></p>
<img src="https://cdn.thecaduceus.eu.org/MCT/img/7.png" alt="7">
<h4><b>2.Once you done creating or retrieving the config files, just run the cell named "Connect to Cloud Accounts" and it will automatically detect your config file and will show you the available remotes, follow on-screen instructions to mount them</b></h4>
<h4><b>Options:</b></h4>
<p><b><code>Custom_Mount_Point</code>: To set custom mount point.</b></p>
<p><b><code>Custom_Cache_Dir</code>: To set custom cache directory.</p>
<img src="https://cdn.thecaduceus.eu.org/MCT/img/8.png" alt="8">
<h4><b>3.After mounting those remotes, now click on the file icon as shown in the image and then navigate to the folder where you mounted your remote (default folder is <code>drives</code>) and you will see the names of remoteswhich you mounted previously.</b></h4>
<h4><b>4.Now copy the file or folder path which needs to be copied, right click on the file or folder and select <code>Copy Path</code> option from the list.</b></h4>
<img src="https://cdn.thecaduceus.eu.org/MCT/img/9.png" alt="9">
  <h4><b>5.After that! paste the path of file or folder in <code>Source</code> field and again go to <code>File Icon->drives</code> and open the mounted remotes into which you want to transfer files/folders and copy its path. You can either directly copy the path of mounted remotes or of any folder inside them and paste the path in <code>Destination</code> field.</b></h4>
<img src="https://cdn.thecaduceus.eu.org/MCT/img/10.png" alt="10">
<h4><b>6.Choose the method trough which you want to transfer your data, refer to "<a href="#modes-of-transfer">🚅Modes of Transfer</a>" below to learn about all of them.</b></h4>
<h4><b>7.Finally, run the code by pressing play button to initiate transfer.</b></h4>
<h2><b>🪀Using Service Accounts</b></h4>
<h4><b>Service accounts are just like normal Google account and thus have same upload or download limits as Google account which is 750GB upload and 10TB download per 24hrs. They are used to act on behalf of a Google account and hence we can use them to prevent hitting Google Drive transfer limits by creating them in a bulk amount.</b></h4>
  <h4><b>1.Don't have service accounts?<a href="https://github.com/TheCaduceus/CloneBot_V2#-making-service-accounts" alt="Creating SA"> create here</a></b></h4>
  <h4><b>2.After creating, make the zip of <code>accounts</code> folder which have 100 or more json files and keep its name as <code>accounts.zip</code>.</b></h4>
  <h4><b>3.Now comeback to Colab screen and select saving options for service accounts to use them without uploading zip file again next time.</b></h4>
  <h4><b>Options:</b></h4>
  <p><b><code>Upload_Service_Accounts</code>: Upload new service accounts.</b></p>
  <p><b><code>Save_To_MyDrive</code>: Save new service accounts to My Drive->MCT Config folder. This will overwrite existing service accounts file.</b></p>
  <img src="https://cdn.thecaduceus.eu.org/MCT/img/11.png" alt="11">
  <h4><b>4.After it, click the file icon, then open <code>accounts</code> folder and right click on anyone json file and select <code>Copy path</code>.</b></h4>
  <img src="https://cdn.thecaduceus.eu.org/MCT/img/12.png" alt="12">
  <h4><b>5.Run "Create/Edit/Delete Rclone Config File" section and paste the path in <code>service_account_file</code> during creating remote for Google Drive.</b></h4>
  <img src="https://cdn.thecaduceus.eu.org/MCT/img/13.png" alt="13">
  <h2><b>🪄Special Add-ons</b></h2>
  <h4><b>Add-ons are the special functions not provided by any single engine officially and are offered by MCT Tool developers. Each of these functions (or simply add-ons) are explained below with their steps to use.</b></h4>
  <img src="https://cdn.thecaduceus.eu.org/MCT/img/5.png" alt="5">

  <h3><b>📥Direct Download Links:</b></h3>
  <h4><b>Function enables to download files or data from single or multiple direct download links to any cloud. It uses Aria engine to deliver best and fastest performance possible. You can also download two or more links at same time with this.</b></h4>
  <h4><b>Just put your direct download links in source field and then enter the destination path to where you want to download data. You can enter multiple direct download links in the source field by separating them using <code>,</code> between each link in the following format: </b></h4>
  <p><b><code>Link1,Link2</code></b></p>
  <img src="https://cdn.thecaduceus.eu.org/MCT/img/14.png" alt="14">
  <h3><b>📃Download links from txt file:</b></h3>
  <h4><b>Function enables to download all links written in a given txt file. This function is useful when we have too many links and it will take too much time separate each link with <code>,</code>.</b></h4>
  <h4><b>User just need to upload the txt file containing the download links to any cloud or in runtime provided by Colab then have to provide its path in source field and destination path in destination field to where you want to download the data. Best format to arrange links in txt file: </b></h4>
  <p><b><code>Link1</code></b></p>
  <p><b><code>Link2</code></b></p>
  <p><b><code>Link3</code></b></p>
  <img src="https://cdn.thecaduceus.eu.org/MCT/img/15.png" alt="15">
  <h3><b>🎥YouTube videos/playlist & other sites</b></h3>
  <h4><b>Function gives the flexibility to download YouTube videos or playlist and videos from other supported sites directly to any cloud or in local runtime storages. It uses yt-dlp which downloads everything in maximum quality by default, you can overwrite by passing flags. User can download two or more videos which are not in same playlist or even two separate playlists at once. Refer to <a href="https://github.com/yt-dlp/yt-dlp" alt="yt-dlp">yt-dlp documentation</a> for more information.</b></h4>
  <h4><b>Just provide the YouTube link of video or playlist or link to videos located on other website (Non-DRM Protected) in <code>Source</code> field and Destination path in <code>Destination</code> field to where you want to download it. You can separate the link of videos or playlist by providing space between each in following format:</b></h4>
  <p><b><code>VideoLink1</code> <code>VideoLink2</code></b></p>
  <p><b><code>PlaylistLink1</code> <code>PlaylistLink2</code></b></p>
  <p><b><code>VideoLink1</code> <code>PlaylistLink1</code></b></p>
  <img src="https://cdn.thecaduceus.eu.org/MCT/img/16.png" alt="16">
  <h3><b>🗃️Torrent DL: (Specific files support)</b></h3>
  <h4><b>Function gives ability to download torrents from <code>.torrent</code> files or magnet links. This function uses LibTorrent to deliver fast download speed as much possible.</b></h4>
  <h4><b>User can download whole torrent content or individual files by specifying their list numbers seperated with a space. Additionally, provide destination to overwrite the download location, by default all downloads goes in local runtime directory <code>/content/</code>.</b></h4>
  <h4><b>MCT Tool also accepts range, what if user need to select all files ranging from 5 to 50? mentioning each of file indices manually? nope this is enough to make anyone sick, user will simply define that particular range (<code>x-y</code> where x < y) using <code>-</code> (dash) like in this case it is <code>5-50</code>, this will tell MCT Tool to automatically detect rest of in-between indices.</b></h4>
  <h4><b>LibTorrent have some limitations while downloading individual files, so it may partially download unspecified files or user may need to stop execution manually after reaching 100% of download progress.</b></h4>
  <img src="https://cdn.thecaduceus.eu.org/MCT/img/17.png" alt="17">
  <h3><b>📤Upload Files to Anonymous Platforms</b></h3>
    <h4><b>Function allow one to upload files or folder to supported anonymous file sharing platforms and harvest all generated links in <code>.txt</code> file, MCT Tool provides additional features like "recursive upload" to upload data recursively from a given folder & "harvest links" to export all generated links in txt file with filename.
    <br><br>Checkout <a href="https://cdn.thecaduceus.eu.org/MCT/json/mct.json" alt="MCT-Json">MCT Json</a> for all supported anonymous platform list, feel free to create issue if you have any other similar platform (having API & same json key mapping) which can be added. Even though MCT Tool provides additonal features, it still compiles with TOS of these platforms and in no way bypass any kind of rate-limit and API limits applies accordingly.
    </b></h4>
  <h4><b>For this, user just need to provide the required path (file or folder) in source field and follow on-screen instruction.</b></h4>
  <h3><b>Ⓜ️MEGA Links DL:</b></h3>
  <h4><b>Function downloads MEGA Link with or without using user's MEGA account to directly any cloud.</b></h4>
  <h4><b>As stated above, user can use MEGA account and MCT Tool will save its credentials in safe format automatically for future use. Enter MEGA link in source field and destination path where MEGA link needs to be downloaded, by default if no destination path is mentioned then link data will be moved to downloads folder in runtime's local storage.</b></h4>
    <h3><b>🗑️UUP DUMP:</b></h3>
    <h4><b>Function enables to collect files mentioned in <code>uup_download_linux.sh</code> files and upload them to any cloud mentioned as destination. It makes work easier for users making ISO files using .sh file given by <a href="https://uupdump.net">UUP DUMP</a> or any other website.</b></h4>
    <h4><b>Provide the exact path of <code>uup_download_linux.sh</code> file or folder path contaning .sh file in source field and destination path where all files needs to be downloaded using given .sh file.</b></h4>
    <img src="https://cdn.thecaduceus.eu.org/MCT/img/18.png" alt="18">
  <h2><b>📦Packing & Extracting Files/Folder</b></h2>
  <h4><b>MCT Tool comes with the ability to pack or extract any files or folder in variety of formats with or without password protection while moving the data from one cloud to another cloud.</b></h4>
  <h4><b>First mount remotes between which you need to transfer the packed or extracted data. Read STEP 2 of "🪝Multi Cloud Transfer" section to learn how to do that.</b></h4>
  <h4><b>Now Get both source path & destination path.</b></h4>
  <h4><b>After it, choose the action which needs to be done with the source path and then enter following Details:</b></h4>
    <p><b><code>Packed_File_Name</code>: Name of output zipped file. If no name is passed then MCT Tool will use original name.</b></p>
    <p><b><code>Source_Path</code>: The path of data which needs to be processed.</b></p>
    <p><b><code>Destination_Path</code>: The path on which you want the final output.</b></p>
  <h4><b></b>User can also encrypt filename & other important file attributes by enabling <code>ENCRYPT_FILENAME</code> option, filename encryption is only supported by <code>.rar</code> and <code>.7z</code> formats and using given option with unsupported formats or conditions will only add standard password protection.</h4>
<h2><b>📂GoFile Integration</b></h2>
<h4><b>GoFile is a free file sharing & unlimited storage platform, MCT Tool provides special integration through which users can upload files/folders to GoFile from any cloud service with recursive upload support.</b></h4>
<h4><b>MCT Tool supports both, anonymous upload or upload using specific account in specific folder using user's API Token provided by GoFile. Additionally, MCT Tool saves API Tokens (in json format) provided by user in encrypted form to make work easier next time.</b></h4>
<h4><b>By default, GoFile creates a random new folder (with random name) to receive the given file if no parent folder id is mentioned which creates mess if large amount of files are uploaded at once, MCT Tool automatically pass root folder id as parent folder id to keep user's account clean.</b></h4>
<img src="https://cdn.thecaduceus.eu.org/MCT/img/19.png" alt="19">

<b>Methods:</b><br>
`Manage Tokens` - Save/Remove your GoFile tokens.<br>
`Upload Files` - Upload files or folder.<br>
`Server Details` - Show GoFile's server information.<br>
`Account Details` - Request GoFile for user's account details & make it human readable, also generates login URL.<br><br>
<b>Fields:</b><br>
`SOURCE` - File or Folder path to upload.<br>
`DESTINATION` - Parent Folder ID in which data needs to be uploaded, provided by GoFile. If not provided, files or folder will be automatically uploaded to root folder.<br><br>
<b>Options:</b><br>
`RECURSIVE` - Upload folder data recursively.<br>
`RAW` - Show API Response as raw.
<h2><b>🚅Modes of Transfer</b></h2>
<h4><b>MCT Tool supports all transfer methods provided by Rclone as follows:</b></h4>
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
<h2><b>⛑Need help!</b></h2>
<h4><b><a href="https://t.me/TheCaduceusOfficial">Subscribe</a> Telegram channel.</a></b></h4>
<h4><b>Send personal message on Telegram<a href="https://telegram.me/TheCaduceusHere"> here</a>.</b></h4>
<h2><b>❤️Credits & Thanks</b></h2>
<p><b><a href="https://github.com/TheCaduceus">Dr.Caduceus</a>: Owner of MCT Tool & maintainer.</b></p>
<p><b><a href="https://rclone.org/">Rclone</a>: The backbone of this powerful project.</b><p>
