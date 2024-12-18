# 解决msix安装包提示证书无法安装的问题

## 导语

笔者在倒腾软件时偶尔会出现“无法验证此应用包的发布者证书”的问题，提示

> “无法验证此应用包的发布者证书。请与系统管理员或应用开发人员联系，以获取具有验证证书的新应用包。必须验证应用包中签名的根证书和所有直接证书(0x800B010A)”


很是苦恼，在网上找到了一个解决办法，分享出来

## 教程

首先右键该msix安装包
![屏幕截图 2024-12-18 121353](https://github.com/user-attachments/assets/452b2551-3814-4c71-b7a9-b632d3e686a3)

点击“属性”
移到”数字签名”一栏
![屏幕截图 2024-12-18 121416](https://github.com/user-attachments/assets/23210580-9767-4f69-87b5-bc347446b6dd)
点击“详细信息”

在接下来的窗口中点击“查看证书”
![屏幕截图 2024-12-18 121427](https://github.com/user-attachments/assets/2d07e4dd-f2ea-4c8d-bd51-8d1a48e8f1a7)

下一个窗口点击“安装证书”
![屏幕截图 2024-12-18 121435](https://github.com/user-attachments/assets/49e5765a-6b9f-4a00-ac4a-850eaa8f1551)

选择“存储到本地计算机”，下一步
![4981a070-7978-4af1-80b2-d69a1b9e6592](https://github.com/user-attachments/assets/1c5df67a-a07e-4289-bf27-c312189a622e)

选择存储位置，“受信任的根证书颁发机构”，确定
![8fdfca64-6e3c-46fc-921e-8e75b282d125](https://github.com/user-attachments/assets/518b09d3-94a5-446d-bae8-260476949432)
![b7a05ebb-faa4-4d17-bbd9-f32de8c8222f](https://github.com/user-attachments/assets/f7e71980-50e5-4f08-9d6b-48cd77583a36)

“完成”即可导入证书
![e18d8e8e-8244-48f2-a44c-bd0f920b4ff7](https://github.com/user-attachments/assets/c44a2b21-8c99-4470-85c4-90df7cd24317)
再次点击安装包即可正常安装
