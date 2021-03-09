# subscan-locale
Subscan uses [Vue I18n](https://kazupon.github.io/vue-i18n/introduction.html) for language localization. 

This repo contains locale file for Subscan, PRs are welcome.

## Contribute
Please spend several minutes reading these notes before you create an issue or pull request.

###  Do not Change Variable Name
For example, this is a snippet in en.json, the word `currency` is a variable and should be left as it is.
```
//en.json
"balance_currency": "Balance {currency}",


//zh-CN.json
"balance_currency": "余额 {currency}",  //good case

"balance_currency": "余额 {货币}",  //bad case
```

###  Pay Attention to Letter Case
Some languages are case-sensitive, thus you should be careful with the letter case and make it consistent with the source file.
```
//en.json
"balance_currency": "Balance {currency}",


//ru.json
"balance_currency": "Баланс {currency}",  //good case

"balance_currency": "баланс {currency}",  //bad case
```