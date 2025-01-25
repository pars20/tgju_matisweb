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




















