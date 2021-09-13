# GPUbot

# Selenium API + Python

# Monitor and notify stock levels for RTX3080 graphics cards.

Bot outline:
- Install python and selenium
- Create GPUbot.py file
- Import dependencies 
- Open browser
- Login to website via send keys.
- Navigate to filtered 3080 URL: https://www.scan.co.uk/shop/gaming/virtual-reality/nvidia-geforce-rtx-3080-graphics-cards#filter=1&manufacturers=ASUS%7CEVGA%7CMSI
- Maybe need to configure headers to prevent 503 errors.
- Search page for stock levels below £800
- Capture URL for products in stock
- Notify stock levels via discord/emails, sending price and URL for quick purchase.
