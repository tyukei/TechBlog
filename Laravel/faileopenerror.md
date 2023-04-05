## open localhost and error


```
The stream or file "/var/www/storage/logs/laravel.log" 
could not be opened in append mode: 
Failed to open stream: Permission denied 
The exception occurred while attempting to log: 
The stream or file "/var/www/storage/logs/laravel.log" 
could not be opened in append mode: Failed to open stream: 
Permission denied The exception occurred 
while attempting to log: The stream or file
```
![](img/2023-04-03-14-01-57.png)

## how to slove
add Permission

1. ```docker-compose exec workspace bash```
2. ```chmod -R 777 storage bootstrap/cache```
3. ```exit```
4. check localhost
   
![](img/2023-04-03-14-05-43.png)