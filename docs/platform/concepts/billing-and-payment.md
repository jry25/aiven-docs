---
title: Billing and payment
---

You configure billing details, including [payment methods](/docs/platform/howto/manage-payment-card), in [billing groups](/docs/platform/concepts/billing-groups-overview). The payment details saved in a billing group apply to all projects assigned to that billing group.

Billing information, invoices, and a breakdown of charges by category and billing group
are available in the **Billing** section of the [Aiven Console](https://console.aiven.io).
To access this section, you must be an
[organization admin](/docs/platform/concepts/permissions#organization-roles-and-permissions).
 Other users have read-only access to some billing information like billing group details
and invoices using the API.

## Service charges

Services are billed by the hour. The minimum hourly charge unit is one hour.
For example, if you create an Aiven service and power it off after 40 minutes,
you are charged for one hour of usage. After 20.5 hours, you are charged
for 21 hours. [Powering off a service](/docs/platform/concepts/service-power-cycle)
stops the accumulation of new charges immediately.

Costs are calculated for the powered-on services in each project. Projects
are charged separately, but you can consolidate the charges for multiple projects
by assigning them to a [billing group](/docs/platform/concepts/billing-groups-overview).

The prices shown in the Aiven Console are inclusive of:

-   Virtual machine costs
-   Network costs
-   Backup costs
-   Setup costs

There are additional costs for some features such as PrivateLink and
additional storage. Network traffic is not charged separately, but your
application cloud service provider might charge you for the network
traffic going to or from their services.

Migrating a service to another cloud provider or region does not incur
any additional costs.

## Credit card fees

The prices listed on the website and in your invoices are inclusive of
all credit card and processing fees that are payable by Aiven. This
includes credit card processor transaction fees and other fees card issuers
charge merchants.

Some credit card issuers add extra charges on top of the fees charged
by Aiven from your cards. The most common fee is an international transaction fee.
Some issuers charge this fee for transactions where the native country
of the merchant, processor, bank, and card are different. Aiven is based
in Finland and the processor is based in the United States. Such fees are not added by
or visible to Aiven, so they cannot be included in the prices or waived.

## Related pages

- Create [billing groups](/docs/platform/concepts/billing-groups-overview) for your organization
- Set up [payment methods](/docs/platform/howto/payment-methods) to add to your
  billing groups
- Use the [invoice API](https://api.aiven.io/doc/#tag/BillingGroup) to export
  cost information to business intelligence tools
