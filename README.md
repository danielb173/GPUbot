# GPUbot

This bot will monitor the Scan website, notifying via discord when RTX3080 stock is available.
<br />Disclaimer: the Scan website uses a captcha prompt to prevent bots from auto buying, this bot is strictly a stock monitor/notifier. 

Bot outline:
- Install python/visual studio (done)
- Create project folder
- Install selenium, BS4, and the chrome webdriver
- Create GPUbot.py file
- Import libraries
- Open browser using selenium
- Login to website via send keys
  - Maybe login not required
- Navigate to 3080fe direct URL: driver.get('https://www.scan.co.uk/nvidia/products/3080/xa3et4n9qf4b3b')
  - Maybe need to configure headers to prevent 503 errors.
- Inspect element for 'Add to Basket'
  - class="btn">Add To Basket
- Use "html = driver.page_source" to get the page source code
- Use BS4 html parser to find these classes, soup.find_all("span", {"class":"container_name"})
- Create WHILE True: loop to continuously check for stock levels in case no stock at the time the bot was run.
  - If("Add to basket" in product.text):
  - time.sleep(5)
- Notify stock levels via discord/emails, sending URL for quick purchase.

Work in progress..
