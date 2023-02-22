# 使用EC2搭配自動化指令架設Wordpress
PeggyWang 20230222 Update

Contact mail:eiscfcu@gmail.com

# 實施步驟

![image](https://user-images.githubusercontent.com/103306835/220606021-d046a359-314d-4e01-b950-847d41107714.png)

# 實驗室目前架構

![image](https://user-images.githubusercontent.com/103306835/220606077-f17fb650-eee3-49c1-8158-cb1b10cdb078.png)


# 步驟1：新增EC2執行個體
1.搜尋EC2

![image](https://user-images.githubusercontent.com/103306835/163394416-ae8cb55f-5498-4f54-bc86-9873bb2d0831.png)

2.點選[EC2]

![image](https://user-images.githubusercontent.com/103306835/163394462-976d94b2-0f0b-4c5d-a4a5-e33cdfe31584.png)

3.點選[Instances執行個體]

![image](https://user-images.githubusercontent.com/103306835/163394525-504888e6-32a2-40b2-b4a2-f9b33483a5bd.png)

4.點選[Launch Instances啟動新執行個體]

![image](https://user-images.githubusercontent.com/103306835/163394805-610e7c8b-9731-4155-afb2-a0a75b6b5837.png)

5.輸入執行個體名稱

![image](https://user-images.githubusercontent.com/103306835/220606185-125be3a2-941c-4b51-893d-b6597dd5c7f1.png)

6.選擇作業系統

![image](https://user-images.githubusercontent.com/103306835/220606267-b06e36da-6d84-4140-8f3b-4afe1f9eb8db.png)

7.選擇類型

![image](https://user-images.githubusercontent.com/103306835/220606348-6c1cb1a0-c8f6-4f4d-9566-30f4a867ad1c.png)

8.選擇金鑰

![image](https://user-images.githubusercontent.com/103306835/220606406-35423737-2cb1-46de-8c02-7233501fdca0.png)

9.

# 步驟2：個體存放位置與安全性設定

![image](https://user-images.githubusercontent.com/103306835/220606509-394f38d1-8e93-4332-bde2-3ac82b77fae9.png)


# 目前實施架構

![image](https://user-images.githubusercontent.com/103306835/220607651-b53d7157-d007-47f0-8522-e056d2083b7b.png)


# 步驟3：上傳網站檔案

1.點選[進階詳細資訊]

![image](https://user-images.githubusercontent.com/103306835/220606642-50eceb03-64c7-4fa9-b84b-afb5b91a43a8.png)

2.點選[複製](檔案連結:https://github.com/EISCFCU/wordpress_on_aws_EC2/blob/main/wordpress.aws.sh)

![image](https://user-images.githubusercontent.com/103306835/220606735-19f51036-e6e0-4f8f-9c57-0286b30f53ba.png)


3.貼上程式碼

![image](https://user-images.githubusercontent.com/103306835/220606837-3206f952-22ac-44af-8397-bb47a4e819dd.png)


# 步驟4：啟動Wordpress伺服器

1.點選[啟動執行個體]

![image](https://user-images.githubusercontent.com/103306835/220607042-4ba39bea-e8d2-46fb-aaf5-60a64f19d638.png)

2.建置狀態

![image](https://user-images.githubusercontent.com/103306835/220607118-737b7806-da17-4387-93e9-9d115d8e1d5a.png)


3.點選[檢視所有執行個體]

![image](https://user-images.githubusercontent.com/103306835/220607183-c3e79e20-487b-4b9f-886d-d0a23fbf809f.png)

4.等待Status轉為2/2 checks
![image](https://user-images.githubusercontent.com/103306835/163399726-b86aa254-6f7a-4a81-a009-1fdab2012d0f.png)

# 步驟5：登入你的Wordpress管理後臺

1.勾選Wordpress
![image](https://user-images.githubusercontent.com/103306835/163399889-1a9b3e2e-8107-4540-9493-c75408ac6551.png)

2.點選Public IPv4 address的open address連結
![image](https://user-images.githubusercontent.com/103306835/163400022-b06e5736-adbb-4d9b-ae43-216e6dc4f57c.png)

# 有可能會出現以下錯誤畫面
![image](https://user-images.githubusercontent.com/103306835/163400067-6d06dda1-2f50-46c1-8ea7-875947f4b42f.png)

# 解決方法
將https的s拿掉 網址最後方打上:80
![image](https://user-images.githubusercontent.com/103306835/163400184-57376b83-bae9-46f0-9441-87f4ec1c0be1.png)

3.出現以下畫面即成功開啟wordpress
![image](https://user-images.githubusercontent.com/103306835/163400333-0f10b86d-667d-43ce-9c15-ab3503eceda2.png)

4.語系選擇繁體中文，並按繼續
![image](https://user-images.githubusercontent.com/103306835/163400400-0d7d5a46-e289-41eb-ba61-38f96885af6d.png)

5.網站標題、使用者名稱及密碼可以自訂
![image](https://user-images.githubusercontent.com/103306835/163400479-28f2ef3c-f09e-489d-ae96-0b6fd2eb98d9.png)

6.勾選確認密碼
![image](https://user-images.githubusercontent.com/103306835/163400543-042e4310-7214-4e95-b6b3-641f32b400e8.png)

7.輸入電子郵件
![image](https://user-images.githubusercontent.com/103306835/163400604-72b0527b-c3b3-4cfb-97ac-ea9843a96857.png)

8.點選[安裝wordpress]
![image](https://user-images.githubusercontent.com/103306835/163400670-e68f1812-d9b2-4e60-a4a6-0fea00949c8e.png)

9.點選[登入]
![image](https://user-images.githubusercontent.com/103306835/163400713-07b6d360-52a6-4d5c-834c-d82aa68b2286.png)

10.輸入帳密並登入
![image](https://user-images.githubusercontent.com/103306835/163400766-31c08108-ff7b-4ad1-8f98-bfa2a92ba1b1.png)

11.點選[文章]
![image](https://user-images.githubusercontent.com/103306835/163400837-9f6814da-8532-467b-afad-188d7b170ab8.png)

12.滑鼠滑動至[網站第一篇文章]
![image](https://user-images.githubusercontent.com/103306835/163400884-d0339522-11d4-428b-8092-90c01041b999.png)

13.點選[檢視]
![image](https://user-images.githubusercontent.com/103306835/163400927-9cb48656-8a68-4e0a-be51-e6016dcb431c.png)

14.你的Wordpress網站首頁
![image](https://user-images.githubusercontent.com/103306835/163400979-786c03df-182c-46b6-9f7f-e887e09ad195.png)









