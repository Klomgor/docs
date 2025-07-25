---
title: View billing history
weight: 40
description: Learn how to view and download billing history, manage invoices, and check your subscription renewal date.
keywords: payments, billing, subscription, invoices, renewals, invoice management, billing administration, download invoices, VAT, billing support, Docker billing
aliases:
    - /billing/core-billing/history/
---

Learn how you can view your billing history, manage your invoices, and verify
your renewal date. All monthly and annual subscriptions are automatically
renewed at the end of the term using the original form of payment.

{{% include "tax-compliance.md" %}}

## Invoices

Your invoice includes the following:

- Invoice number
- Date of issue
- Date due
- Your "Bill to" information
- Amount due (in USD)
- Description of your order, quantity if applicable, unit price, and
amount (in USD)

The information listed in the **Bill to** section of your invoice is based on
your billing information. Not all fields are required. The billing information
includes the following:

- Name (required): The name of the administrator or company
- Email address (required): The email address that receives all billing-related
emails for the account
- Address (required)
- Phone number
- Tax ID or VAT

You can’t change an invoice once it's been issued. When you update your billing
information, this change won't update an existing invoice. If you need to
update your billing information, make sure you do so before your subscription
renewal date when your invoice is finalized. For more information, see
[Update the billing information](details.md).

### View renewal date

{{< tabs >}}
{{< tab name="Docker subscription" >}}

You receive your invoice when the subscription renews. To verify your renewal
date, sign in to [Docker Billing](https://app.docker.com/billing). Your renewal
date and amount are displayed on your subscription card.


{{< /tab >}}
{{< tab name="Legacy Docker subscription" >}}

You receive your invoice when the subscription renews. To verify your renewal
date:

1. Sign in to [Docker Hub](https://hub.docker.com).
1. Select your user avatar to open the drop-down menu.
1. Select **Billing**.
1. Select the user or organization account to view the billing details. Here
you can find your renewal date and the renewal amount.

{{< /tab >}}
{{< /tabs >}}

### Include your VAT number on your invoice

> [!NOTE]
>
> If the VAT number field is not available, complete the
[Contact Support form](https://hub.docker.com/support/contact/). This field may
need to be manually added.

{{< tabs >}}
{{< tab name="Docker subscription" >}}

To add or update your VAT number:

1. Sign in to [Docker Home](https://app.docker.com/) and choose your
organization.
1. Select **Billing**.
1. Select **Billing information** from the left-hand menu.
1. Select **Change** on your billing information card.
1. Ensure the **I'm purchasing as a business** checkbox is checked.
1. Enter your VAT number in the Tax ID section.

    > [!IMPORTANT]
    >
    > Your VAT number must include your country prefix. For example, if you are
    entering a VAT number for Germany, you would enter `DE123456789`.

1. Select **Update**.

Your VAT number will be included on your next invoice.

{{< /tab >}}
{{< tab name="Legacy Docker subscription" >}}

To add or update your VAT number:

1. Sign in to [Docker Hub](https://hub.docker.com).
1. Select your organization, then select **Billing**.
1. Select the **Billing address** link.
1. In the **Billing Information** section, select **Update information**.
1. Enter your VAT number in the Tax ID section.

    > [!IMPORTANT]
    >
    > Your VAT number must include your country prefix. For example, if you are
    entering a VAT number for Germany, you would enter `DE123456789`.

1. Select **Save**.

Your VAT number will be included on your next invoice.

{{< /tab >}}
{{< /tabs >}}

## View billing history

You can view the billing history and download past invoices for a personal
account or organization.

### Personal account

{{< tabs >}}
{{< tab name="Docker subscription" >}}

To view billing history:

1. Sign in to [Docker Home](https://app.docker.com/) and choose your
organization.
1. Select **Billing**.
1. Select **Invoices** from the left-hand menu.
1. Optional. Select the **Invoice number** to open invoice details.
1. Optional. Select the **Download** button to download an invoice.

{{< /tab >}}
{{< tab name="Legacy Docker subscription" >}}

To view billing history:

1. Sign in to [Docker Hub](https://hub.docker.com).
1. Select your organization, then select **Billing**.
1. Select the **Payment methods and billing history** link.

You can find your past invoices in the **Invoice History** section, where
you can download an invoice.

{{< /tab >}}
{{< /tabs >}}

### Organization

> [!NOTE]
>
> You must be an owner of the organization to view the billing history.

{{< tabs >}}
{{< tab name="Docker subscription" >}}

To view billing history:

1. Sign in to [Docker Home](https://app.docker.com/) and select your
organization.
1. Select **Billing**.
1. Select **Invoices** from the left-hand menu.
1. Optional. Select the **invoice number** to open invoice details.
1. Optional. Select the **download** button to download an invoice.

{{< /tab >}}
{{< tab name="Legacy Docker subscription" >}}

To view billing history:

1. Sign in to [Docker Hub](https://hub.docker.com).
1. Select your organization, then select **Billing**.
1. Select the **Payment methods and billing history** link.

You can find your past invoices in the **Invoice History** section, where you
can download an invoice.

{{< /tab >}}
{{< /tabs >}}
