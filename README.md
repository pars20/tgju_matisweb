# MatisWeb TGJU Live Market Prices


## Index Price
Shows the last trade price retrieved from the tgju for the **INDEX_NAME**

`[TGJU matisweb INDEX_NAME]`


examples:

`[TGJU matisweb geram18]`

`[TGJU matisweb geram24]`

`[TGJU matisweb mesghal]`


# Options
We have some option to get custom output with **shortcodes**

`[TGJU matisweb INDEX_NAME OPTIONS]`


## Index Price in Tomans
Shows the last trade price for the **INDEX_NAME** In **Tomans**

`[TGJU matisweb INDEX_NAME toman+price]`


> description: First we change the unit to Tomans, Then we call the price

example:

`[TGJU matisweb geram18 toman+price]`

## Index Price in Rials
Shows the last trade price for the **INDEX_NAME** In **Rials**

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
We can use the options in combined way:

`[TGJU matisweb INDEX_NAME option+option+...]`

example:

`[TGJU matisweb geram18 title+toman+price+change+changePercent+date]`

> This will show the Title, next we change the unit to Tomans, then we show price, and other fields.

[TGJU matisweb geram18 title+toman+price+**rial**+change+changePercent+date]

`[TGJU matisweb geram18 title+toman+price+rial+change+changePercent+date]`

> This will show the Title, next we change the unit to Tomans, then we show price.
>
> Then we change the unit to Rial, and the fields after this will be shown in Rials.
















