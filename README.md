# Traits-Laravel7-BPJSKesehatan-Bridging
BPJS Kesehatan Bridging, File trait for laravel 7 or laravel 8

## 1. Tambahkan beberapa credential yang di file .env.
```
BPJS_BASE_URL=
BPJS_CONS_ID=
BPJS_CONS_PWD=
BPJS_USER_KEY=
BPJS_KODE_PK=
```
## 2. Install library LZString menggunakan composer.
```bash
composer require nullpunkt/lz-string-php
```

## 4. Copy file BpjsTraits.php ke App\Http\Traits\BpjsTraits.php

## 5. Panggil BpjsTraits.php disetiap controller yg dibutuhkan.
```php
namespace App\Http\Controllers;

use Illuminate\Http\Request;
use Illuminate\Support\Facades\Http;
use Validator;
use Illuminate\Validation\Rule;


use App\Http\Traits\BpjsTraits;

class SepMasterVclaimController extends Controller
{
    use BpjsTraits;
}
```
