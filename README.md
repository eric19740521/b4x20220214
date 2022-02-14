B4X實驗: Capture PC Server(B4J).監控軟體，電腦監看神器.手機(B4A)從遠端可以監控

參考資料:
https://www.b4x.com/android/forum/threads/b4j-cctv-example.34695/page-2#posts
https://www.b4x.com/android/forum/threads/b4x-bytes-to-file.70111/#content
https://www.b4x.com/android/forum/threads/server-cctv-server.37382/


1.APP操作



2.程式碼解說
Server:如何將螢幕截圖.傳送給手機
AWTRobot
		'Capture current monitor screen
		c3po.ScreenCurrentRectangleSetAsRightScreen '<- needed since I have multiple monitors
		c3po.ScreenCaptureToFile(strFileName)		


Client:手機接收到資料.如何轉成imageview所需格式
Private bmp As Bitmap = BytesToImage(Buffer)
SetImageView(ImageView1,bmp,"cover")

  圖片尺寸.要能適應螢幕大小???


3.未來
a.能接收電腦聲音
b.使用者發送語音給電腦
c.能控制使用者的電腦


程式碼:
https://github.com/eric19740521/b4x20220214






