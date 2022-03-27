# Multi Cloud Transfer (Advanced!) 🔥
<p><b>The most Advanced yet simple Multi Cloud Transfer tool to transfer Your Data from any cloud to any cloud remotely based on Rclone.⚡</b></p>
<h2><b>🆕What's New!🆕</b></h2>
<p><b><i>v2.2.5 (Multi Cloud Transfer Integration)</i><b></p>
<h4><b>1.Multi Cloud Transfer Tool Added!⚡</b></h4>
<h4><b>2.Auto Reconnecter is Added in support of large transfer.😙</b></h4>
<h4><b>3.Added New Sections and updated the guide.😌</b></h4>
<h4><b><i>4.Service Accounts Randomizer (In Beta)</i><b></h4>
<h4><b>5.Config will now move to My Drive at place of frustrating you by downloading in your Device.</b></h4>
<p><b><i>v2.2.4 (R-1.58.0)</i><b></p>
<h4><b>1.Project upgraded & optimized for Rclone 1.58.0 ☺️</b></h4>
<h4><b>2.Multi Cloud Transfer Tool (in Beta)</b></h4>
<h4><b>3.Guide Updated and Steps are added for new auto-config authorization.</b></h4>
<p><b><i>v2.2.3 (Migrating to 1.58.O Beta)</i><b></p>
<h4><b>1.Rclone will now auto-fetch the saved progress including Rclone config file (If Any) from your Google Drive (My Drive).🔥</b></h4>
<h4><b>2.Now you can use your own Rclone Config File! Just upload it to your My Drive and fetch it</b>🙃</h4>
<h4><b>3.File will be shifted to Google Drive at place of starting download to your Device!</b></h4>
<p><b><i>v2.2.1 (R-1.57.0)</i></b></p>
<h4><b>1.Create/Delete/Edit Rclone config file/remote!🤩</b></h4>
<h4><b>2.Download Rclone config file!😀</b></h4>
<h4><b>3.Support all Rclone Commands!😎</b></h4>
<h4><b>4.Store your Rclone progress on Cloud and access it from anywhere!😉</b></h4>
<h2><b>⛔ NOTICE</b></h2>
<h4><b>1.This Repository is now Merged with <a href="https://www.caduceus.ml/Rclone-Setup-on-Google-Colab/">Rclone on Google Colab</a> repository to make your Work even more simple!☺️</b></h4>
<h4><b>2.The Project is now updated and everything is optimized for new changes made by Rclone v1.58.0 written in 3rd point.</b></h4>
<h4><b>3.In Latest Rclone Version v1.58.0, they made some changes in Auto-Config. Don't worry I am aware of that and till that you can either follow the New Steps or if you are making config file for Google Drive then you can provide your CLIENT ID and CLIENT SECRET to Work around that situation! I will update you in my Update Channel ,once I find some alternative to help you out in that Step.</b></h4>
<h4><b>4.For auto-config always choose No(n) because we are going to run the Rclone not on our own local device! Otherwise login will not work.</b></h4>
<h2><b>📝 Introduction</b></h2>
<h4><b>This Project makes it easy and possible to Perform every Rclone Task on Google Colaborately and Store your progress on the cloud and continue it where you left it anytime and anywhere! This Project comes with In-Build support to perform basic task like Creating/Editing/Viewing and Deleteing and also Downloading your Rclone Config file which is needed by almost all Rclone User to perform task! To execute any rclone command you just need to type "!rclone" (After installing Required Setup Files) before any command like "!rclone config" where config is the Command name!</b></h4>
<!--- Step Area Begin --->
<h2><b>🔌Before you Start!</b></h2>
<h4><b>Please Connect your Google Account, So that Rclone can easily save its progress automatically.</b></h4>
<img src="Img/rq-1.png">
<h4><b>If you want to use your own Rclone config file or the progress saved in your Google Drive in My Drive! Then run the following Code as shown in the image</b></h4>
<img src="Img/rq-2.png">
<h4><b.Run the Time Out Preventer to prevent Google Colab from getting timeout before your Transfer got Completed.</b></h4>
<img src="Img/30.png">
<p><b>Lets move Data from any cloud to any cloud as you want! Since we are using Colab, So it will not consume your Internet or System Resource.</b></p>
<h2><b>⚙️ How to use?</b></h2>
<h4><b>Since this repository is just a small part of my Large prpject <a href="https://www.caduceus.ml/Rclone-Setup-on-Google-Colab/">Rclone on Google Colab</a>, So please read it there to learn about all tools!</b></h4>
<h4><b>1.Before we procced! I recommend to either create or fetch your Rclone Config file to Google Colab using above two methods! Creating and fetching will automatically place the file in correct location!</b></h4>
<img src="Img/24.png">
<h4><b>2.Once you done creating or fetching the config file! Just run the Code named "Connect to Cloud Accounts" and it will automatically detect your config file and will show you  dropdown list to mount multiple remotes as shown in the image. Now select remoted and click mount to connect to those remotes between which you have to transfer your Data.</b></h4>
<img src="Img/25.png">
<h4><b>3.After mounting those remotes or Cloud Accounts, Now click on the File icon as shown in the image and then you will see two folder named "drives" open the second folder named "drives" and you will see the names of Remotes or Cloud Account which you mounted previously!</b></h4>
<img src="Img/26.png">
<h4><b>4.Now Simply open that Folder and copy the file or folder path which needs to be copied and then right click on the file or folder and select "Copy Path" option from the list</b></h4>
<img src="Img/27.png">
<h4><b>5.After that! Paste the path of file or folder in "Source" field and again go to File Icon-->drives and open the Cloud Account into which you want to transfer files/folders and copy its path! You can either directly copy the path of Cloud Account or of any folder inside it and paste the path in "destination" field.</b></h4>
<img src="Img/28.png">
<h4><b>6.Choose the mode to "Copy" otherwise you can use other like "Check". And you can also Enter some extra arguments/flags (optional). Refer to Flag section to see all available flags all arguments!</b></h4>
<h4><b>7.If you want to get notified! when your transfer got completed then tick the Email_notification option and provide Gmail Email ID as well as its password and the Receiver Email ID on which you want to receive the notification!  (optional)</b></h4>
<p><b>
  Email_notification: Select this option to enable following options.<br>
  logs: Check this option to also get log in Mail.<br>
  emailID: Enter your Gmail ID.<br>
  password: Enter Password of given Gmail ID.<br>
  Receiver_ID: The Email ID on which you want to receive the Notification.
  </p></b>
<img src="Img/29.png">
<h4><b>8.Dry Run option is just to check the Source as well as destination path without copying anything.(Optional)</b></h4>
<h4><b>9.Finally! Run the code by pressing Play button to start transferring. Enjoy!🙃</b></h4>
<h2><b>🎌Flags</b></h2>
<h4><b>You can use Arguments to control the behavior or customize the command as per your need! Here is the list of all flags:</b></h4>
<h3><b><a href="https://rclone.org/flags/" alt="Global Flag Page">Show Flags</a></b></h3>
<h2><b>🎯Points to be Remembered</b></h2>
<h4><b>1.Always choose No (n) for Auto-Config because we are not going to use Rclone on our Local Device/Machine otherwise login will not work!</b></h4>
<h4><b>2.Don't forget to type '!' before executing any custom Rclone Command.</b></h4>
<h4><b>3.For Safety! Rclone will always save progress in your My Drive! Not in any of your Shared Drive.</b></h4>
<h4><b>4.Use the Dry Run option to check both Source and Destination path without copying anything.</b></h4>
<h4><b>5.You can either choose the path of Cloud Account folder or anyother folder inside it</b></h4>
<h2><b>Supported Command List</b></h2>
<h4><b><a href="https://github.com/TheCaduceus/Rclone-Setup-on-Google-Colab/blob/main/Cmds.md">Show List</a></b></h4>
<h2> 🔐 Safe or Not? ✅</h2>
<h4><b> 1.Don't Worry! No data will be shared with anyone, if you use the <a href="https://github.com/TheCaduceus/Rclone-Setup-on-Google-Colab">Original code</a>.🔒</b></h4>
<h4><b> 2.This code do not share even a single piece of data to any third party source and not create any log of that!🔑</b></h4>
<h4><b> 3.Do not trust any other copy of this Code.📚</b></h4>
<h2>⛑Contact Us!</h2>
<h4><b>Join our Update Channel at Telegram:<a href="https://telegram.me/TheCaduceusUPDATE"> Join Now!</a></b></h4>
<h4><b>Directly Contact the Developer using Telegram <a href="https://telegram.me/HelpAutomatted_Bot">@HelpAutomatted_Bot</a></b></h4>
<h2>❤️Credits & Thanks</h2>
<p><b><a href="https://github.com/TheCaduceus">Dr.Caduceus</a>: For making this Project and Guide.</b></p>
<p><b><a href="https://rclone.org/">Rclone</a>: The Backbone of this Powerful Project.</b></p>
