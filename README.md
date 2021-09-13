# GPUbot

The goal is to learn Selenium + Python

This bot will monitor and notify stock levels for RTX3080 graphics cards.

Bot outline:
- Install python and selenium
- Create GPUbot.py file
- Import libraries
- Open browser
- Login to website via send keys.
- Navigate to filtered 3080 URL: https://www.scan.co.uk/shop/gaming/virtual-reality/nvidia-geforce-rtx-3080-graphics-cards#filter=1&manufacturers=ASUS%7CEVGA%7CMSI
- Maybe need to configure headers to prevent 503 errors.
- Search page for stock levels below £800
- Inspect element for 'Add to Basket' and 'Price'
- Create FOR loop to continuously check for stock levels in case no stock at the time the bot was run.
- Capture URL and price for products in stock
- Notify stock levels via discord/emails, sending price and URL for quick purchase.

Work in progress..
