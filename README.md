# Early Exercise of American Options

### Introduction

This program intends to help traders make decisions on early exercise of american options. American options holders unlike European option holders who can only exercise the option on the expiration date may exercise anytime up to expiraiton. Traders should capture the advantage if its European value has fallen below intrinsic value and prevent making an error and not exercising an option early.

Options data will be scrapped from the Yahoo stock finance API by python libaries.

### Inputs Required

1. Ticker, Type and Strike Price
2. Declared Dividend / Estimated Dividend
3. Applicable Interest Rate (e.g. SOFR)
4. Ex-dividend date, Pay-date and Expiration Date

### Reminder

1. For a call options to be an early exercise candidate, the underlying must pay dividends.

2. Call options should only be exercised immediately prior to the stock paying dividend. No other day will early exercise be optimal.

3. Even if a put option is an early exercise candidate, there is a blackout perod prior to the ex-dividend date during which it is not possible for traders to earn enough interest to compensate the loss of the dividend.
