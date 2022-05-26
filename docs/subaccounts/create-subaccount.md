# Create a subaccount

> Create a transfer subaccount

```php
<?php
$data = [
    'account_number' => '0690000034',
    'account_bank' => '044'
];

$subaccount = Flutterwave::subaccounts()->create($data);

dd($subaccount);
```

## Parameters

| Parameter | Required | Description                                                                                                                                                                                                 |
| --------- | -------- | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| account_number | True     | The subaccount's bank account number. When testing on staging, you can find a list of all the available test bank accounts [here](https://developer.flutterwave.com/docs/test-bank-accounts). |
| account_bank     | True     | This is the subaccount’s bank code, you can use the [List of Banks](/banks/list-banks) to retrieve a bank code.      |
