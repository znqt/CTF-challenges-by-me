# SVATTT2016

### Vòng chung kết
- Hình thức: on-site attack/defense
- Thời gian: 02/12/2016 tại KS Grand Plaza
- Thể lệ: https://docs.google.com/document/d/1kTAT0hfwKWaYhnkqy0Rg2FbbyHZZr8Tv2gET477sXEM/edit

## Serverlist

`camp1` và `camp2` có thể setup nhiều challenges trên đó.

Name | Type | IP | Port service
--- | --- | --- | ---
castle | Daemons | 128.199.141.114 | 31330 
tower1 | Daemons | 139.59.227.253  | 31331
tower2 | Daemons | 139.59.227.254  | 5002
tower3 | Daemons | 139.59.227.255  | 31333
tower4 | Daemons | 139.59.235.0    | 5004
--- | --- | --- | ---
neutralcamp2 | NeutralCamp | 139.59.235.1 | 40002
neutralcamp4 | NeutralCamp | 139.59.235.1 | 40004
camp2 | None | 139.59.235.2 | None
--- | --- | --- | ---
scorebot | bot | 128.199.95.110 | 9988,5000

## Public-key
l4w
```
ssh-rsa AAAAB3NzaC1yc2EAAAADAQABAAABAQDI9n4f9/cO4QX6FB/iq0EMPLljo5dzDPymup+nKK/zjA1UPtgHxv0hDgIV+e/LzWPIeCWwoRvmllKIKKYs2DQFsacaioFg5YKoiqcdjK/Ub6wIJnvT/HH1x1p+XlS/7EdMpMzYJgFE5OnSZGvJBfXj6b9zBG3s7YN95F1S5j8lIGQceyHL0YK19uEdRFPgSldPBLOKjxvHdq2Qra5o3oL2Lp0Fr0OZuFGMCBYuBZWWcm1Y0NOnqMWreTzm+DSoUSnXgg04vmHOsnPUjyG9hWV1CK6wMfHQJkg+j6dkWWZPlbLtymSugeIbklgwdzfBlHjeRelwfADAGyHTjZLrnT3b navi@0xMacB00k
```
g4mm4
```
ssh-rsa AAAAB3NzaC1yc2EAAAADAQABAAACAQDadblyiX34bmQ7YByR0rsDh/4suV5eHC5dmeyUimMLHtJxc4fx1gwWhr4eu7nTmXDTmbvuQwYhWyciMn8s9SpBRytWZtS1c8sXqcrtv+WQu6glLQmKHLSYOOV/OVTipkmIK+NzwHLn8TlvE5WCgGAGKCgl+qakl3JgB97OirBNvITh8bqP9LOf+MHYsacUCqXg/ZNiQjKMGL9c/f8bl7xgEvZ5/ZJ+JDp6pj9WcBD0lOJF+zqLo3y8lWNfjLuMPnec84dy+ph/DGV1ypWWhJd2cVqcvwDqt2iZ7V81h3wCMX7yLSO4mzy/a/8gTAdB0oLwPk9I7sz5agE7q88fnp3GC1TjIkIpwhqA5VnLq1J/PrzWe+OrSS7HjMhtes/mecs34lb0HxJyzN0otdzF6jyxSqgFC0mCBKiqzjxVimz3FWqagmf+eY1BQ4f85i8UH97OyrXvimGUINaOhe79xntGVElH8aPlRI2cSXuwc7vmuTKbHfofGSAbZPUCFlacYh6iWWiaJxTvP+/wSPSC5+DRHV53YPvCujHKguYO+ryFtkT5v2I6u31H3GuCM1TNpHHwTK7XxmqsnsWYdVmsxat9iWL36PcdZp9INE1ATT/zNLzRMtJceYLSUKCDqlBP4tI5CHXW6hR/3TX6/7bCww2tJf0BJVLs8JqTumIbYb80SQ== gamma95@gmail.com
```


##TODO
- Ra challenges (10 bài?), trong đó có 3 bài attack/defense ở các căn cứ.
- Làm scoreboard cho hình thức A/D (mua/xài vũ khí, blah blah).
- Scorebot kiểm tra các cơ chế game (owner của các căn cứ, check vá/sửa hợp lệ,...)
- Iptables limit connection.

## Challenges 
Update tree ở dưới với format:

**Name|Category|Level|Author**

Sẽ không dùng score, mà mình dùng level để đánh giá, sau đó sẽ có người review lại đề và cho ra thang điểm sau (có cho số điểm tượng trưng cho mọi người dễ hình dung):
* Easy (~ 50-100 points)
* Medium (~ 101-200 points)
* Hard (~ 201-300 points)
* Expert (~ >300 points)

Flag format: SVATTT{hash / base64}

Sau đó push source code/material/description/hints (nếu có).

```
challenges/
|
|___ Daemons
|     |_________ Castle|rev/crypto/pwn|Hard|l4w = 220 gold
|     |_________ Tower 1|rev/crypto|medium|l4w = 140 gold
|     |_________ Tower 2|web|easy|l4w = 100 gold
|     |_________ Tower 3|pwn|easy|l4w = 120 gold
|     |_________ Tower 4|web|medium|l4w = 180 gold
|   
|___ Neutral Creeps
      |_________ Neutral camp 1|web|TBD|g4mm4
      |_________ Neutral camp 2|easy|shellcode(misc)|l4w
      |_________ Neutral camp 3|easy|reverse|l4w      
      |_________ Neutral camp 6|hard|pwn|xboy      
      |_________ ...TBD


```
