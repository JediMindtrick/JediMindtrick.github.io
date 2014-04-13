[system.reflection.assembly]::loadwithpartialname("microsoft.sharepoint")
$site= New-Object Microsoft.SharePoint.SPSite ("http://Amit-Test-VM/pwa/27test <http://amit-test-vm/pwa/27test>")
$web=$site.OpenWeb()
$list=$web.Lists["Actions"]
$list.Fields |select ID, title, internalname| more
