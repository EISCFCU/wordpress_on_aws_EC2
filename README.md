# 使用EC2搭配自動化指令架設Wordpress
PeggyWang 20220414 Update

Contact mail:eiscfcu@gmail.com


# 步驟1：新增EC2執行個體
1.搜尋EC2

![image](https://user-images.githubusercontent.com/103306835/163394416-ae8cb55f-5498-4f54-bc86-9873bb2d0831.png)

2.點選[EC2]

![image](https://user-images.githubusercontent.com/103306835/163394462-976d94b2-0f0b-4c5d-a4a5-e33cdfe31584.png)

3.點選[Instances執行個體]

![image](https://user-images.githubusercontent.com/103306835/163394525-504888e6-32a2-40b2-b4a2-f9b33483a5bd.png)

4.點選[Launch Instances啟動新執行個體]

![image](https://user-images.githubusercontent.com/103306835/163394805-610e7c8b-9731-4155-afb2-a0a75b6b5837.png)

5.選擇作業系統(這裡稱為AMI映像檔)

![image](https://user-images.githubusercontent.com/103306835/163394898-f1b46df6-45ad-4c2d-8a0f-6c33438aace8.png)

6.選擇機器型態

![image](https://user-images.githubusercontent.com/103306835/163395011-a6d59598-5708-4b43-bac4-f912e86a3046.png)

# 步驟2：個體存放位置與安全性設定
放在雲端上的電腦的安全設定；Subnet設定所屬us-east-1a
![image](https://user-images.githubusercontent.com/103306835/163397822-791fd52c-9a95-498e-9c48-46dd03af293c.png)


# 步驟3：上傳網站檔案

1.至Advanced Details 點選[As  file]

![image](https://user-images.githubusercontent.com/103306835/163395634-fc48c632-8fea-4b04-9d74-f6b721e6791f.png)

2.點選[選擇檔案]

![image](https://user-images.githubusercontent.com/103306835/163395671-818f8b16-e514-458c-b277-b9eb24d255dd.png)

3.選擇wordpress.aws.sh(檔案連結:)

![image](https://user-images.githubusercontent.com/103306835/163395733-1b9e1d90-54e5-4c63-b50b-8def15d500b6.png)

4.點選[Next：Add Storage]

![image](https://user-images.githubusercontent.com/103306835/163395804-e6c5567a-a48d-4e05-aed3-65a85539fea6.png)

5.點選[Next：Add Tags]
增加硬碟(EBS)，EBS可以視為電腦的 D槽或是E槽。
![image](https://user-images.githubusercontent.com/103306835/163397961-29406d0f-9ddc-41ad-b6dd-a1163b4ad86f.png)

# 步驟4：命名電腦名稱

1.增加標籤(Tags)

![image](https://user-images.githubusercontent.com/103306835/163396152-15aaefdf-6263-4357-bed8-a4fca274c222.png)

2.點選 [Next：Configure Security Group]

![image](https://user-images.githubusercontent.com/103306835/163396240-b1a06423-6e84-4609-8b46-95e34d1713af.png)

# 步驟5：安全群組與開通網頁瀏覽權限

1.輸入安全群組(Security Group)

![image](https://user-images.githubusercontent.com/103306835/163396374-9dd8fdf0-5f19-4ab1-94ea-7ddb6f28e3de.png)

2.點選[Add Rule]

![image](https://user-images.githubusercontent.com/103306835/163396460-13b61da2-316a-4465-a00b-a53c46f901e9.png)

3.新增Type=HTTP,HTTPS

![image](https://user-images.githubusercontent.com/103306835/163396564-c2d616fc-dd0e-4697-a0d8-3d4f0673e554.png)

4.點選[Review and Launch]

![image](https://user-images.githubusercontent.com/103306835/163396633-63c07c2f-9001-4ea6-b976-9fc9d51164f9.png)

# 步驟6：啟動Wordpress伺服器

1.Launch EC2

![image](https://user-images.githubusercontent.com/103306835/163396764-455e4898-76f9-4b61-be20-f8b9647cd775.png)

2.勾選I acknowledge….

![image](https://user-images.githubusercontent.com/103306835/163396828-c3ee4b27-4c85-469e-bf89-528c1b341f40.png)








