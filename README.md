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

## Ex_2:  
Method: POST  
EndPoint: /user_info_3  
Request form data:  
name: str  
age: int  
salary: int  

**Response:**  
```sh
{
    'name': name,
    'age': age,
    'salary': salary,
    'family': {
        'children': [
            [
                'Alex', 
                24
            ], 
            [
                'Kate', 
                12
            ]
        ],
        'u_salary_1_5_year': salary * 4
    }
}
```
**Task:** 
Сделать и в Rewrite, и в BreakPoint (можно отключить, чтобы не стопило на каждом запросе).  
Подменить body в Charles так, чтобы в запросе ушла salary, которую вы вписали в Postman, а в u_salary_1_5_year цифра вернулась меньше оригинальной из запроса.

## Ex_3:  
Method: GET  
EndPoint: /object_info_1  
Request url params:   
name: str  
age: int  
weight: int  

**Response:**  
```sh
{
    'name': name,
    'age': age,
    'daily_food': weight * 0.012,
    'daily_sleep': weight * 2.5
}
```
**Task:**  
Сделать и в Rewrite, и в BreakPoint (можно отключить, чтобы не стопило на каждом запросе).
Подменить параметры запроса в Charles так, чтобы в Postman пришел ответ, где другой name, daily_food > weight из запроса, а daily_sleep < weight из запроса.

## Ex_4:
Method: GET  
EndPoint: /object_info_3  
Request url params:  
name: str  
age: int  
salary: int  

**Response:**  
```sh
{
    'name': name,
    'age': age,
    'salary': salary,
    'family': {
        'children': [
            [
                'Alex', 
                24
            ], 
            [
                'Kate', 
                12
            ]
        ],
        'pets': {
            'cat': {
                'name':'Sunny',
                'age': 3
            },
            'dog': {
                'name':'Luky',
                'age': 4
            }
        },
        'u_salary_1_5_year': salary * 4
    }
}
```
**Task:**  
Сделать и в Rewrite, и в BreakPoint (можно отключить, чтобы не стопило на каждом запросе).  
- Сделать через Charles так, чтобы сервер вернул 500 код.
- Сделать через Charles так, чтобы сервер вернул 405 код.