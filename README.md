# sdk-logs

## Como Configurar
- Este pacote utiliza como base o jenssegers/laravel-mongodb
- Utilize o comando `composer install .`
- Registar o Provider
```
LogManager\SdkLogs\SdkLogsServiceProvider::class,
```
- Registar o Aliases
```
'SDKLogs' => LogManager\SdkLogs\Facades\SDKLogs::class,
```
- Criar o arquivo de configuração deste package, com o comando 
````
php artisan vendor:publish --provider="LogManager\SdkLogs\SdkLogsServiceProvider" --tag="config"
`
