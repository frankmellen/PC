# Chrome 和 Safari  同步时发生书签合并问题的解决方法

**经历：**
1. Chrome 书签在本地做了大量的整理变动。
2. Chrome 和 Safari 已经许久无法自动同步书签。
3. 卸载 iCloud 程序和扩展，从 Microsoft Store 重装。
4. 再次同步，iPhone 上的 Safari 书签跟 PC 上的 Chrome 书签发生了合并问题。

Windows 版的 Chrome 安装了 iCloud 扩展程序，

在 iPhone 的 Safari 和 PC 的 Chrome 进行同步书签时，

可能会发生一个很严重的问题：Safari 和 Chrome 的书签会合并，

并不是以 Chrome 的书签为主同步更新到 iPhone 上的 Safari。

---

## 解决方法 1

1. 备份 Chrome 现有的完整书签，关闭 Chrome
2. 打开目录：%LocalAppData%\Google\Chrome\User Data\Default
3. 找到两个文件 ‘Bookmarks’ & ‘Bookmarks.bak’
4. 删除 ‘Bookmarks’
5. 删除 ‘Bookmarks.bak’的后缀名‘.bak’
6. 打开 Chrome

此方法是否能够完美恢复历史书签取决于两个文件的修改时间。


## 解决方法 2

在发生书签合并同步后，马上去 Google 账号下载备份数据。

1. 备份 Chrome 现有的完整书签。
2. 打开 Google 账号的数据下载页：https://takeout.google.com/
3. 取消全选，选择 ‘Chrome’ 进行下载。
4. 清空 Chrome 的所有书签，iPhone 上的 Safari 书签会逐渐消失。
5. 导入从 Google 账号上下载的 ‘Bookmarks.html’。

此方法大概率能够恢复历史书签，本地大量书签变动后，在 Google 账号中还未来得及归档。

## 解决方法 3

最原始的方法就是在现有书签的基础上删除重复。

1. 安装 [Bookmarks clean up](https://chrome.google.com/webstore/detail/bookmarks-clean-up/oncbjlgldmiagjophlhobkogeladjijl) 扩展程序。
2. [使用教程](https://key.chtouch.com/ContentView.aspx?P=3008 "Bookmarks clean up 輕鬆找出重複或已失效的書籤 - Chrome 瀏覽器擴充功能")

---

写下解决方法，将来碰到同样问题可以快速解决。

2019/11/01

Frank