**Create Project**
	After create the project when page alert **port number must be 0 to 65535** the OK button is spinning until page refresh
	![[Pasted image 20250321125154.png]]
**Add Group**
	~~In the table not show the new group but only show in the side bar~~ 
	![[Pasted image 20250321125301.png]]
**Edit Group**
	==Edit group can't edit and change parent==
**Real Time Edit Tag** 
	Minimum can minus
	Unit allowed more than 50 characters
	Max and Minimum have range are **-999999999 to 999999999
	![[Pasted image 20250321125839.png]]**
	==Search doesn't show data when search blank==
	![[Pasted image 20250321135604.png]]
	![[Pasted image 20250321135657.png]]
	~~==Page show Integer + Decimal should be less than 5 after edit decimal to any number==~~
	![[Pasted image 20250321130041.png]]
	after saved
	![[Pasted image 20250321130105.png]]
	![[Pasted image 20250321130121.png]]
	==When create read only tag, it can enter write topic but it has error: **"Read topic is required for read-only permission"**  but doesn't has a popup==
	==Read-write Tag can create with only write topic==
	![[Pasted image 20250321130328.png]]
	==Can't edit Integer to 0 it err **Argument `integer`: Invalid value provided. Expected Int, NullableIntFieldUpdateOperationsInput or Null, provided String."** but it can created with integer 0==
	![[Pasted image 20250321130421.png]]
	
~~**Alarm Tag**~~
	Alarm tag can't create when tags are **all tag loss and Some tag loss**
	![[Pasted image 20250321140003.png]]
	![[Pasted image 20250321140011.png]]
	Alarm Tag can create with out alarm condition but it show == 0 in the table
	![[Pasted image 20250321140207.png]]
	![[Pasted image 20250321141113.png]]
	and it can edit to blank when tick check box to true and false again
	![[Pasted image 20250321141221.png]]
	![[Pasted image 20250321141250.png]]
	Alarm Tag can't create and edit alarm to line
	==When enter start time and date time website is explode==
	![[Pasted image 20250321141657.png]]
	![[Pasted image 20250321141615.png]]
**Historical** 
	~~==Edit historical tag unequal align==~~
	![[Pasted image 20250321142145.png]]
	doesn't has start date must be before end date err popup 
	![[Pasted image 20250321143432.png]]
**Trend Monitoring**
	~~==Can create new trend with minus==~~ 
	![[Pasted image 20250321143815.png]]
	![[Pasted image 20250321143916.png]]
	~~==Trend can create with tag but when look in edit it doesn't show anything==~~
	![[Pasted image 20250321144320.png]]
	![[Pasted image 20250321144231.png]]
	~~==Trend monitoring can create with out time and date format~~==![[Pasted image 20250321144443.png]] ~~==Trend edit can save with **fixed minus y range** but can't save **tag==**~~ 
	![[Pasted image 20250321144729.png]]
	Trend monitor some minus number can click ok
	![[Pasted image 20250321144918.png]]
**Report**
	report can continue creating after err 
	![[Pasted image 20250321150811.png]]
	![[Pasted image 20250321151237.png]]
	When create with 0 input it show err but OK button still spinning
	 ![[Pasted image 20250321152620.png]]
	 ~~report can create with blank header, footer and curve name~~
	 ![[Pasted image 20250321152809.png]]
	 When edit report with new blank curve the webpage is explode
	 ![[Pasted image 20250321153244.png]] ![[Pasted image 20250321153307.png]]
	 ==report can create with skip curve== 
	 ![[Pasted image 20250321153748.png]]![[Pasted image 20250321154059.png]]
	 when report created (true condition) it err
	 ![[Pasted image 20250321154447.png]]
	 ![[Pasted image 20250321154611.png]]