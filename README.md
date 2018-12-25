# lightened-posts
![TamperMonkey v4.7](https://img.shields.io/badge/TamperMonkey-v4.7-brightgreen.svg)
![Chrome x64 v70.0](https://img.shields.io/badge/Chrome%20x64-v70.0-brightgreen.svg)

[中文页面](https://greasyfork.org/zh-CN/scripts/370927-%E6%A0%B9%E6%8D%AEuid%E5%B1%8F%E8%94%BD%E4%B8%BB%E9%A2%98%E5%B8%96%E5%8F%8A%E5%9B%9E%E5%A4%8D-nga)


## Intro

Lightened-posts is a javascript for TamperMonkey, which can alter unpleasing posts, according to posters' uid, into a lightened style. It works on [the NGA forum](bbs.ngacn.cc).

I just came to javascript as soon as I started this script. I would be thankful if you could tell me my problems, and would also be glad if these codes can help you a little bit.

Please post Issues for any problem.

Currently version: 0.2

## Installation

You can get this script on [Greasyfork](https://greasyfork.org/scripts/370927-根据uid屏蔽主题帖及回复-nga), or import this file [lightened-post.js](https://github.com/Elypha/lightened-posts-NGA/blob/master/lightened-post.js) manually.

## Features

Lightened-posts can block/unblock a certain user in his or her info page through the buttons above user name. Putting in a series of uids is also possible now, and this is recommended as a way to make your backup.

Lightened-posts is compatible with [NGA Auto Pager V2](https://greasyfork.org/users/63731) which is created by Sunness.

## Usage

4 buttons will be added to the user info page after proper installation, which is currently (https://bbs.ngacn.cc/nuke.php?func=ucp&uid=?).

* **Block.** Add this user to your block list.
* **Remove.** Remove this user from your block list.
* **Input.** By clicking this button there would next be an alert messagebox which writes the instructions. Please make sure you fill in the blank in a right way. This helps you to import a series of uids, and is mostly used when you want to restore your settings.
* **View.** By clicking this button you would be able to see your whole block list in an alert messagebox. You can do copy (tested on Chrome) to make a backup. Please be noticed that the 00000000, which is at the end of the whole list, is simply an end mark.

## Tips

The data are saved in `localstorage.uid_list`. If you want to wipe them manually please active this line at the beginning of the script, save it and then come back and refresh the nga page.
```bash
//CLEAR
//localstorage.removeItem(uid_list)
```
