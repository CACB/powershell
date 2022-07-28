# powershell
Powershell commands

COUNT ASSETS FOR INVENTORY
===========================

Users:

(Get-ADUser -Filter *).Count

Groups:

(Get-ADGroup -Filter *).Count

Computers:

(Get-ADComputer -Filter *).Count

GPOs:

(Get-GPO -All).Count

(get-sdmGPO *).Count


OUs:

Get-ADOrganizationalUnit -Filter * | select Name,distinguishedName

(Get-ADOrganizationalUnit -Filter * | select Name,distinguishedName).Count
