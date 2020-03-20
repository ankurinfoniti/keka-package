# keka-package

[![Issues](https://img.shields.io/github/issues/som-31/keka-package.svg?style=flat-square)](https://github.com/som-31/keka-package/issues)
[![Stars](https://img.shields.io/github/stars/som-31/keka-package.svg?style=flat-square)](https://github.com/som-31/keka-package/stargazers)


##A wrapper for Keka API implemented by Successive technologies

##First set credentials in your keka.php file in config folder: 
- keka_client_id => 'your_keka_client_id'
- keka_secret_key => 'your_keka_secret_key'
- keka_api_key => 'your_api_key'

```php
use Successive\Keka\Http\Services\EmployeeService;

$employeeService = new EmployeeService();
$response = $employeeService->getEmployees(['pagesize' => 400]);
$response = $employeeService->getEmployeeByEmpNo('employeenumber');
$response = $employeeService->currentMonthBirthdays();
$response = $employeeService->currentMonthJoinees();
