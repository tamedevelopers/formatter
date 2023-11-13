# tame-currency-format
### @author Fredrick Peterson (Tame Developers)
### 2023 Fredrick Peterson

Javascript/JQuery Plugin for Number/Currency Formatting
```
|--------------------------------------------------------------------------
|This Plugin uses the Javascript Intl.NumberFormat
| Minified version is 3kb for Javacript and 4kb for jQuery
```
[Intl.NumberFormat](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Intl/NumberFormat) <br>
[Reach me on Linkedin](https://www.linkedin.com/in/fredipeterson/)

* [Installation](#installation)
* [Properties](#properties)
* [Currency Symbols](#currency-symbols)
* [Browser](#browser)
* [Usage](#usage)
  * [JQuery](#Jquery)
  * [JQuery Initialize](#jquery-initialize)
  * [Javascript](#javascript)
  * [Javascript Initialize](#javascript-initialize)
* [Useful links](#useful-links)


## Installation
```
npm install tame-format
```

## Properties

| Key               |  Values                       |  Description                                                          |
|-------------------|-------------------------------|-----------------------------------------------------------------------|
| style             |  `currency` \| `decimal`      | Default `currency` When style is `decimal` currency will be ignored   |
| currency          |  `string`                     | Default `HKD` refer to [Currency Symbols](#currency-symbols)          |
| currency_symbol   |  `string` \| `true`           | By default if not provided, takes the global configuration or the currency symbol of `currency` key |
| display           |  bool `true` \| `false`       | Default `true` Display the currency symbol or not                     |
| space             |  bool `true` \| `false`       | Default `true` If there should be space between amount and symbol     |
| position          |  `false` \| `left` \| `right` | Default `false` Takes the normal positioning according to currency    |
| amount            |  numeric `float\|int\|string` | Default `0` Should be numeric figures                                 |
| decimals          |  0-4  `int`                   | Default `2` Decimal point                                             |


## Currency Symbols
- Default symbol is `HKD`

| Symbols                  |
|--------------------------|
| `USD` \|`EUR` \|`JPY` \|`GBP` \|`AUD` \|`CAD` \|`CNY` \|`TRY` \|`AFN` \|`ALL` \|`DZD` \|`AOA` \|`ARS` \|`AMD` \|`AWG` \|`AZN` \|`BSD` \|`BHD` \|`BDT` \|`BBD` \|`BYN` \|`BZD` \|`XOF` \|`BMD` \|`BTN` \|`BOB` \|`BAM` \|`BWP` \|`BRL` \|`BND` \|`BGN` \|`BIF` \|`KHR` \|`XAF` \|`CVE` \|`KYD` \|`CLP` \|`COP` \|`KMF` \|`CDF` \|`NZD` \|`CRC` \|`HRK` \|`CUC` \|`ANG` \|`CZK` \|`DKK` \|`DJF` \|`DOP` \|`XCD` \|`EGP` \|`ERN` \|`ETB` \|`FJD` \|`GMD` \|`GEL` \|`GHS` \|`GIP` \|`GTQ` \|`GNF` \|`GYD` \|`HTG` \|`HNL` \|`HKD` \|`HUF` \|`ISK` \|`INR` \|`IDR` \|`IRR` \|`IQD` \|`ILS` \|`JMD` \|`JOD` \|`KZT` \|`KES` \|`KPW` \|`KRW` \|`KWD` \|`KGS` \|`LAK` \|`LBP` \|`LSL` \|`LRD` \|`LYD` \|`MOP` \|`MKD` \|`MGA` \|`MWK` \|`MYR` \|`MVR` \|`MRU` \|`MUR` \|`MXN` \|`MDL` \|`MNT` \|`MAD` \|`MZN` \|`MMK` \|`NAD` \|`NPR` \|`NIO` \|`NGN` \|`NOK` \|`OMR` \|`PKR` \|`PAB` \|`PGK` \|`PYG` \|`PEN` \|`PHP` \|`PLN` \|`QAR` \|`RON` \|`RUB` \|`RWF` \|`SHP` \|`WST` \|`STN` \|`SAR` \|`RSD` \|`SCR` \|`SLL` \|`SGD` \|`SBD` \|`SOS` \|`ZAR` \|`SSP` \|`LKR` \|`SDG` \|`SRD` \|`SZL` \|`SEK` \|`CHF` \|`SYP` \|`TWD` \|`TJS` \|`TZS` \|`THB` \|`TOP` \|`TTD` \|`TND` \|`TMT` \|`UGX` \|`UAH` \|`AED` \|`UYU` \|`UZS` \|`VUV` \|`VEF` \|`VND` \|`YER` \|`ZMW` |

## Browser
```
<script src="../dist/currencyFormat-javascript..min.js"></script>
<script src="../dist/currencyFormat-jquery.min.js"></script>
```

## Usage
- Jquery and Javascript usage


### Jquery - `Currency Format Jquery Usage`

```
let totalAmount = $.tameCurrency.format({
    style: 'decimal',
    amount: 23900,
})
```

```
$("#amount-div").tameCurrency({
    currency: 'EUR',
    amount: 23900,
})
```

### Jquery Initialize
- [optional] used to change the global currency symbol
```
$.tameCurrency.init('$USD');
```

### Javascript - `Currency Format Javascript Usage`
```
let totalAmount = tameCurrency.format({
    style: 'decimal',
    amount: 23900,
})
```

```
tameCurrency.input("#amount-div", {
    currency: 'EUR',
    amount: 23900,
})
```

### Javascript Initialize
- [optional] used to change the global currency symbol
```
tameCurrency.init('$USD');
```

## Useful links

- If you love this Javascript/JQuery Plugin, you can [Buy Tame Developers a coffee](https://www.buymeacoffee.com/tamedevelopers)
- More examples in the test folder

