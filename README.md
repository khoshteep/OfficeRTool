# Office(R)Tool
**An advanced tool to install, activate,**

**and config MS Office 2016, 2019, and 2021.**

**A Link To Offical MDL** [**Help & Support Thread**](https://forums.mydigitallife.net/threads/84450/)

[<img src="https://raw.githubusercontent.com/DarkDinosaurEx/OfficeRTool/main/Welcome.png" width="70%">](https://forums.mydigitallife.net/threads/office-r-tool-continued.84450/)

[<img src="https://raw.githubusercontent.com/DarkDinosaurEx/OfficeRTool/main/Logo.png" width="85%">](https://forums.mydigitallife.net/threads/office-r-tool-continued.84450/)

# How to get latest release
**- Copy / Paste to PS Console.**

**- Password for Rar file is "MDL2022"**
````
        <# v1.0 based on Xiang ZHU script #>
        <# v1.1 Update by Aonodensetsu #>
        
        $url = 'https://github.com/DarkDinosaurEx/ZixSx/releases/latest'
        $request = [System.Net.WebRequest]::Create($url)
        $response = $request.GetResponse()
        $realTagUrl = $response.ResponseUri.OriginalString
        $version=$realTagUrl.split('/')[-1].Trim('v')
        $O_fileName = "ZickTest.rar"
        $N_fileName = "OfficeRTool.rar"
        $realDownloadUrl = $realTagUrl.Replace('tag', 'download') + '/' + $O_fileName
        $DesktopPath = [Environment]::GetFolderPath("Desktop")
        $OutputFile = $DesktopPath+'\'+$N_fileName
        Invoke-WebRequest -Uri $realDownloadUrl -OutFile $OutputFile
        [Environment]::Exit(1)
        [Environment]::Exit(1)
````

# Latest Changes
## Core function changes
- User-friendly Interface
- Auto Create Package Info file
- Auto Detect system Arch. & Lang
- Multi-Language / Architecture Support
- Activation script based on KMS_VL_ALL (from abbodi1406)
    
## Menu changes
- Install from ISO / Offline folder
- Online / Offline Install Include Create ISO
- Visual Refresh for Current & LTSC Channels
- Downloading Offline Image / Offline Package
- Convert & Activation for Office Products, Include 365 & Home
    
## Misc.
- Last activation Error Code output
- Proxy / Debug / Self Update Options *NEW*
- Using Language Name instead Language code
- Replace 0/1 selection, with something much better
- Remove Not genuine banner & Pop-up (the new one)
