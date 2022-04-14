# wordpress_on_aws
Update 20220414 PeggyWang

Contact mail:eiscfcu@gmail.com


#方案1：使用EC2搭配自動化指令架設Wordpress

#步驟1：新增EC2執行個體
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

#步驟2：個體存放位置與安全性設定

![image](https://user-images.githubusercontent.com/103306835/163395489-ce0a12af-cfd7-4440-bd63-461ad24f4b1a.png)

#步驟3：上傳網站檔案

1.至Advanced Details 點選[As  file]

![image](https://user-images.githubusercontent.com/103306835/163395634-fc48c632-8fea-4b04-9d74-f6b721e6791f.png)

2.點選[選擇檔案]

![image](https://user-images.githubusercontent.com/103306835/163395671-818f8b16-e514-458c-b277-b9eb24d255dd.png)

3.選擇wordpress.aws.sh(檔案連結:)

![image](https://user-images.githubusercontent.com/103306835/163395733-1b9e1d90-54e5-4c63-b50b-8def15d500b6.png)

4.點選[Next：Add Storage]

![image](https://user-images.githubusercontent.com/103306835/163395804-e6c5567a-a48d-4e05-aed3-65a85539fea6.png)

5.點選[Next：Add Tags]

![image](https://user-images.githubusercontent.com/103306835/163395889-9d00e6b2-570a-4565-8a7b-2e1a939c3449.png)

#步驟4：命名電腦名稱



