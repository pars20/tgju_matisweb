# MatisWeb TGJU Live Market Prices

This plugin fetches the latest market prices for various indexes from TGJU and stores them.
You can easily display this data anywhere on your WordPress website using shortcodes. 🧐

Here’s the complete documentation for the shortcode:


## Index Price

Displays the latest trade price fetched from TGJU for the specified index.

`[TGJU matisweb INDEX_NAME]`


examples:

`[TGJU matisweb geram18]`

`[TGJU matisweb geram24]`

`[TGJU matisweb mesghal]`


# Options
We offer several options to generate custom outputs using **shortcodes**

`[TGJU matisweb INDEX_NAME OPTIONS]`

### Options List

+ **title** : Returns the title of the index.

+ **price** : Returns the price of the index.

+ **date** : The last time for retrieved price.

+ **change** : Returns the +/- sign and the amount of change in compare with yesterday.

+ **changePercent** : Returns the +/- Sign and the Percentage of change and the % sign.

+ **toman** : Converts the unit to Toman (no direct output).

+ **rial** : Converts the unit to Rials (no direct output).



## Index Price in Tomans
Thia way we display the last trade price for the **INDEX_NAME** In **Tomans**

`[TGJU matisweb INDEX_NAME toman+price]`


> description: First we change the unit to Tomans, Then we call the price

example:

`[TGJU matisweb geram18 toman+price]`

## Index Price in Rials
Thia way we display the last trade price for the **INDEX_NAME** In **Rials**

`[TGJU matisweb INDEX_NAME rial+price]`


> description: The default unit is Rials and you do not need to use this option, but in the mixed options this can be useful

example:

`[TGJU matisweb geram18 rial+price]`



## Price Change
Shows the **Price change** in compared to the previous day's price

`[TGJU matisweb INDEX_NAME change]`

example:

`[TGJU matisweb geram18 change]`

## Price Change Percent
Shows the **Price change percent** in compared to the previous day's price

`[TGJU matisweb INDEX_NAME changePercent]`

example:

`[TGJU matisweb geram18 changePercent]`

## Last trade time
Shows the Time for the last trade which we have retrieved

`[TGJU matisweb INDEX_NAME date]`

example:

`[TGJU matisweb geram18 date]`

## Index Title
Shows the Title of the **INDEX_NAME**

`[TGJU matisweb INDEX_NAME title]`

example:

`[TGJU matisweb geram18 title]`



# Mix the options
This is where the MAGIC happens! 🤩

You can combine these options to create custom outputs:


`[TGJU matisweb INDEX_NAME option+option+...]`


example:

`[TGJU matisweb geram18 title+toman+price+change+changePercent+date]`

> This will show the Title, next we change the unit to Tomans, then we show price, and other fields.

### Multiple units

[TGJU matisweb geram18 title+**toman**+price+**rial**+change+changePercent+date]

`[TGJU matisweb geram18 title+toman+price+rial+change+changePercent+date]`

> First we set the unit to Tomans, show price.0Then we change the unit to Rial, and the fields after this will be shown in Rials.


[TGJU matisweb geram18 **toman**+price+**rial**+price]

`[TGJU matisweb geram18 toman+price+rial+price]`

> Showing price in Tomans and also in Rialsa.

### Custom titles and words inside Options

[TGJU matisweb geram18 toman+**قیمت:**+price+**تومان**+rial+price+**ریال**]

`[TGJU matisweb geram18 toman+قیمت:+price+تومان+rial+price+ریال]`




# CSS
We can use these **css selectors** to customize all the parts of this shortcode in _fornt-end_: 😎

### Title
`span#title`

### Price
`span#price`

### Change
`span#change`

`span#change.up`
`span#change.down`

### Change Percent
`span#changePercent`

`span#changePercent.up`
`span#changePercent.down`

### Date/Time
`span#date`
















