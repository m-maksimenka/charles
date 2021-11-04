# Charles

Protocol: http  
IP: 162.55.220.72  
Port: 5005  

## Ex_1
Method: GET  
EndPoint: /get_method  
Request url params:  
name: str  
age: int  

**Response:**  
```sh
[
    “Str”,
    “Str”
]
```
**Task:**  
Сделать и в Rewrite, и в BreakPoint (можно отключить, чтобы не стопило на каждом запросе).  
Подменить url в Charles, чтобы в запросе ушло имя, которые вы вписали в Postman, а вернулось то, которое вы подставили в Charles.