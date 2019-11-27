---
group: extensions
title: Install Amazon Sales Channel
---

The Amazon Sales Channel extension installs and adds features to integrate your Magento catalog with Amazon Seller Accounts to sell through the Amazon Marketplace. To review additional information, see the [Amazon Sales Channel Marketplace](http://marketplace.magento.com/magento-module-amazon.html) page.

## Requirements

-  **Magento Instance**: Amazon Sales Channel can be installed on instances with {{site.data.var.ce}} and {{site.data.var.ee}} versions 2.2.4+ and 2.3.X. We do not support the extension on Magento 2.1 or Magento 1.

-  **Magento Web Account**: You should have a Magento web account, which is used to create and track an API key.

-  **API Key**: Get an Amazon Sales Channel API key through your Magento web account. The following instructions include these steps.

## Get the Amazon Sales Channel extension

1. Locate Amazon Sales Channel in the [Magento Marketplace](https://marketplace.magento.com/magento-module-amazon.html).

1. On the extension page, choose your **Edition** and **Your store version**.

1. Click **Add to Cart**.

1. Click the shopping cart icon and complete the checkout process.

    You will need your Magento Web Account login credentials to complete checkout.

1. On the _Thank you for your purchase!_ screen, ignore the _Install_ and _Download_ options and skip to Install the extension.

## Install the extension

When installing the extension, use the name `magento/amazon-sales-channel` for composer installation: `composer require magento/amazon-sales-channel`.

1. Follow the instructions for [General CLI Installation]({{ site.baseurl }}/extensions/install/).

{:.bs-callout .bs-callout-info}
After installation, you must add the Amazon API Key.

## Add the Amazon API key

1. Follow the instructions to [Add or Verify the Amazon API Key](https://docs.magento.com/m2/ce/user_guide/sales-channels/amazon/amazon-verify-api-key.html){:target="_blank"}.

To begin onboarding, see [Onboarding Amazon Sales Channel](https://docs.magento.com/m2/ce/user_guide/sales-channels/amazon/amazon-onboarding-home.html).

## Additional configuration options

You have the following options for configuring Amazon Sales Channel. You do not need to modify these settings to begin onboarding and selling on Amazon. We recommend advanced administrators consider these options.

1. Log into the Magento Admin.

1. On the _Admin_ sidebar, go to **Stores** > _Settings_ > **Configuration**.

1. Click **Sales Channels**, then **Global Settings**.

1. If you want to display the **Revenue** section on the store's dashboard screen, set **Show Dashboard Chart** to `Yes`.

1. For **Clear Log History**, indicate the interval for clearing the collected logs. Options include Once Daily, Once Weekly, and Once Monthly (default).

1. Advanced users recommended: **Background Tasks (CRON) Source**. All background tasks are handled by CRON jobs using the Magento CRON. Advanced users can change this setting to Command Line (CLI) CRON.

1. Click **Save Config**.

## Update the Amazon Sales Channel version

1. Follow the instructions to [upgrade an extension]({{site.baseurl}}/extensions/install/#upgrade-an-extension).
