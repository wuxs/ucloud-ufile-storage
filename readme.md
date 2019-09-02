# Ucloud ufile storage for Laravel
Base on: 
* https://docs.ucloud.cn/api/ufile-api/
* https://github.com/xujif/ucloud-ufile-sdk
* https://github.com/xujif/ucloud-ufile-storage

# Usage:
register the `Jekhy\UcloudUfileStorage\UfileServiceProvider::class;` in your app configuration file:
```php
'providers' => [
    // Other service providers...
    Jekhy\UcloudUfileStorage\UfileServiceProvider::class,
],
```
config/filesystems.php
```
'disks' => [
    'yourDiskName'=>[
        'driver' => 'ucloud-ufile',
        'bucket'=>'xxx',
        'public_key'=>'xxx',
        'secret_key'=>'xxx',
        'suffix'=>'.ufile.ucloud.cn',
        'prefix'=>'',
    ],
]
```
