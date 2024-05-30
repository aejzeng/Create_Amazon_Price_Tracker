# Create_Amazon_Price_Tracker

Step 1 - Use BeautifulSoup to Scrape the Product Price
  1. Find a product on Amazon that you want to track and get the product URL or just use the one I'm tracking.
   In addition to the URL, when your browser tries to load up a page in Amazon, it also passes a bunch of other information. e.g. Which browser you're using, which computer you have etc.

  These additional pieces of information are passed along in the request Headers.

  You can see your browser headers by going to this website:

  http://myhttpheader.com/

  2. Use the requests library to request the HTML page of the Amazon product using the URL you got from 1.

  3. Use BeautifulSoup to make soup with the web page HTML you get back. You'll need to use the "lxml" parser instead of the "html.parser" for this to work.

  4. Use BeautifulSoup to get hold of the price of the item as a floating point number and print it out.

Step 2 - Email Alert When Price Below Preset Value
  We want to get an email when the price of our product is below a certain value. e.g in the case of the Instant Pot, we'll set the target price as $100.

  1. So when the price is below 100 then use the smtp module to send an email to yourself. In the email, include the title of the product, the current price and a link to buy the product.

  2. Make sure you've got the correct smtp address for your email provider:

  Gmail: smtp.gmail.com
  
  Hotmail: smtp.live.com
  
  Outlook: outlook.office365.com
  
  Yahoo: smtp.mail.yahoo.com
  
  If you use another email provider, just Google for your email provider e.g. "Gmail SMTP address"

