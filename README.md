# DockerizedAppDemo
此專案示例.NET App容器化，版本使用最新的Visual Studio 2022以及.NET 6

【操作步驟】
1. 本機先行安裝好Docker
2. 以任意方式創建一.NET應用程式
3. 於該專案路徑下，創建名為「Dockerfile」的檔案，並複製貼上本次範例之內容
4. 於該專案路徑下，創建名為「.dockerignore」的檔案，並複製貼上本次範例之內容
5. 開啟CMD，移至專案檔路徑位置
6. 輸入指令：docker build -t [your_image_name] .
7. 輸入指令：docker run -it --rm [your_image_name] [your_container_name]
8. Hello, World!
<br /> 

>*(1) 新版本為佳  
(2) 建議以簡易console app為測試範例，若是Web app則尚需增加指令：-p [machine_port]:[container_port]  
(3) 記得更改.NET版本、專案及DLL名稱；特別注意該檔案無「副檔名」  
(4) 該步驟為建制忽略檔，若省略該步驟亦可成功操作  
(5) 移動當前路徑指令為：cd [your_project_directory]  
(6) 「-t」為標註tag name，「.」為指定當前路徑位置，[your_image_name]依喜好自行輸入  
(7) 「-i」為開啟控台互動，「-t」為pseudo-TTY，「--rm」為程式結束後即刪除該容器，[your_container_name]依喜好自行輸入  
(8) 操作成功！  
