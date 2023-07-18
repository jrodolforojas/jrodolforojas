# Add your Namecheap custom domain to your railway app

Custom domains are pretty cool but sometimes hard to configure if you don't know about them, that was my case. Too much talk, let's do it!

Once you bought your domain and you have your railway app available on the internet are some steps you have to follow.

Go to your railway app domain settings by `Clicking in the card`, and `Settings` and go to the **Domain Section**. After that, you will see a button called **+ Custom Domain**.

![Railway domain section](/blog/images/01_custom_domain_button.png)

If an input appeared, write your domain name. In my case, I want a **subdomain** of my domain `carpil.app`. It will be `api.carpil.app` and click on the **Add Domain** button.

![Add Custom Domain input](/blog/images/01_add_custom_domain_name.png)

Appears a modal to **Create a DNS Record**, this info will be inserted on your Namecheap domain advanced DNS configuration.

![Create DNS Record modal](/blog/images/01_create_dns_record.png)

To do that, go to your `Account`, `Domain List`, and click on the `Manage` button of your domain previously bought. Once you are in your domain config go to the `Advanced DNS` section.

![Advanced DNS configuration](/blog/images/01_advanced_dns_configuration.png)

Finally, click on `add new record` button and fill in the DNS info provided by your railway app.

![Advanced DNS configuration with railway dns records](/blog/images/01_dns_config_filled.png)

<aside>
⚠️ It could take up to 24 to 72 hours to propagate the DNS for the internet but in just a couple of minutes they are ready

</aside>

That's it! Hope it helps you. 😄

[@jrodolforojas](https://www.linkedin.com/in/jrodolforojas/)
