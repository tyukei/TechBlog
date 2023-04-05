## open localhost and error

```
The stream or file 
"/var/www/html/storage/logs/laravel.log" 
could not be opened in append mode: 
Failed to open stream: Permission denied The
```

![](img/2023-04-05-01-12-12.png)

## how to slove

https://shiraberu.tech/2021/11/27/laravel-storage-permission-error-fix/

```
# chown www-data:www-data ./storage/ -R
```

![](img/2023-04-05-01-14-53.png)