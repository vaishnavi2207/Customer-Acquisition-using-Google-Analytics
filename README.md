# Customer-Acquisition-using-Google-Analytics
This analysis would prove extremely useful in creating customized strategies for different customer segments. Forecasting the traction will help in systematic presentation of promotional offers, special packages etc.

# Introduction
Google Analytics is presently one of the most popular digital analytics software. It can provide valuable insights that can help business shape their strategies to target more customers. Though like everything in the world of Data Science and Analytics, there is a tradeoff – a cost of $150k for customer level insights. Across industries, customer acquisition work in similar ways. This analysis would prove extremely useful in creating customized strategies for different customer segments. Forecasting the traction will help in systematic presentation of promotional offers, special packages etc.

# Problem Statement
Google Analytics has data available at vast combinations of metrics and dimensions. We were working for a client who was entering a new market and they were using their website to sell their products.

What information will benefit a new business tremendously?

When will their website have the highest traction -
We cannot emphasize enough on the benefits that come with knowing this one number. Depending on the kind of business, it can help reduce uncertainties in different parts and answer pressing questions like “How much inventory should I keep?” or “How do I allocate my resources” — salesforce in our case. While in our case knowing the number of visitors on the website tomorrow may not help too much (since the website is already up and running and designed to handle moderate traffic), knowing the number of people who will “enroll” for the services in the future can help us forecast our demand (and many other things) which can answer a lot of important questions.

Which customers have a higher lift of conversion -
Once we know the forecast for the demand in the future, understanding what drives that demand can be highly valuable information, especially for a nascent company. GA tracks a myriad of attributes about the users — the channel they came through, their age, their gender, the device they are using, etc. Leveraging these attributes to set strategies proves to be highly beneficial.

# Accessing the Data

Google provides you with you access to download everything you can see on your GA dashboard. But there is a catch! The granularity of the accessible data depends if you are a premium or a non-premium account holder. GA offers a premium membership that gives access to user-event level information and it comes with an annual fee of $150k to be paid to Google. But even with non-premium accounts, we have access to pretty much whatever we can see on the dashboard with a limited view. You can download individual files for subset of data but that is inefficient. We have used the Google API's to access our data. All one requires is a JSON file (from your website) and our ga_connect.py (from our git repository). These are the steps to follow -

Create your key file — ‘client_secret.json’ for your website.
This will help you connect to Google’s core reporting API.
We have developed a data pipeline which establishes a connection to access GA data
Note - You need to have a Google Analytics service account linked to your website to initialize a json file.
