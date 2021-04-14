<br>以系統管理員執行cmd，複製一份目前的開機項目
<br>> bcdedit /copy {default} /d "Windows 10 Without Hyper-V"
<br>執行完，會取得一串ID，替換掉下面的ID
<br>> bcdedit /set {ID} hypervisorlaunchtype off
<br>檢查啟動項目
<br>> bcdedit /enum
<br>
<br>
https://blog.cwlove.idv.tw/docker-work-with-vmware/

<br><br>
用 msconfig 檢查並修改開機選單時間


<br><br><br>
方法二：
<br>
windows 10 版本為20H1以上、vmware為15.5.5以上，<br>
安裝vmware時，需再安裝WHP(Windows Hypervisor Platform)<br>
設置虛擬機cpu選項中將三項虛擬化引擎取消勾選。
