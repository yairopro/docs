---
title: Disabling webhooks
intro: 'You can disable a webhook to unsubscribe from events that occur on {% data variables.product.prodname_dotcom %}.'
versions:
  fpt: '*'
  ghes: '*'
  ghae: '*'
  ghec: '*'
topics:
  - Webhooks
---

## About disabling webhooks

{% ifversion fpt %}You can disable a webhook that was previously enabled for a repository, organization, {% data variables.product.prodname_marketplace %} account, {% data variables.product.prodname_sponsors %} account, or {% data variables.product.prodname_github_app %}.{% endif %}

{% ifversion ghec %}You can disable a webhook that was previously enabled for a repository, organization, {% data variables.product.prodname_enterprise %}, {% data variables.product.prodname_marketplace %} account, {% data variables.product.prodname_sponsors %} account, or {% data variables.product.prodname_github_app %}.{% endif %}

{% ifversion ghes or ghae %}You can disable a webhook that was previously enabled for a repository, organization, {% data variables.product.prodname_enterprise %}, or {% data variables.product.prodname_github_app %}.{% endif %}

To disable a webhook, you can choose to deactivate or delete it. When you deactivate a webhook, the webhook deliveries will stop, and you can choose to reactivate the webhook at a later time. When you delete a webhook, it cannot be restored.

For more information, see "[AUTOTITLE](/webhooks/about-webhooks)" and "[AUTOTITLE](/webhooks/using-webhooks/creating-webhooks)."

## Disabling a repository webhook

To disable a repository webhook, you can deactivate or delete it. You must be a repository owner, or have admin access in the repository, to disable webhooks.

You can use the {% data variables.product.prodname_dotcom %} web interface or the REST API to delete a webhook for a repository. For more information about using the REST API to delete a repository webhook, see "[AUTOTITLE](/rest/webhooks/repos#delete-a-repository-webhook)."

{% data reusables.repositories.navigate-to-repo %}
{% data reusables.repositories.sidebar-settings %}
{% data reusables.webhooks.sidebar_webhooks %}
{% data reusables.webhooks.disable_webhook %}

## Disabling an organization webhook

To disable an organization webhook, you can deactivate or delete it. Only organization owners can disable webhooks in an organization.

You can use the {% data variables.product.prodname_dotcom %} web interface or the REST API to delete an organization webhook. For more information about using the REST API to delete an organization webhook, see "[AUTOTITLE](/rest/orgs/webhooks#delete-an-organization-webhook)."

1. In the upper-right corner of any page on {% data variables.location.product_location %}, click your profile photo.
1. Click **Your organizations**.
1. To the right of the organization, click **Settings**.
{% data reusables.webhooks.sidebar_webhooks %}
{% data reusables.webhooks.disable_webhook %}

{% ifversion ghec or ghes or ghae %}
## Disabling a global webhook for a {% data variables.product.prodname_enterprise %}

Enterprise owners can disable a global webhook in an {% data variables.product.prodname_enterprise %}. For more information, see "[AUTOTITLE](/admin/monitoring-activity-in-your-enterprise/exploring-user-activity-in-your-enterprise/managing-global-webhooks)."

{% endif %}

{% ifversion fpt or ghec %}

## Disabling a {% data variables.product.prodname_marketplace %} webhook

You can deactivate a webhook that was previously enabled for events relating to an app that you published on {% data variables.product.prodname_marketplace %}. You cannot delete the webhook. Only the owner of the app can deactivate the {% data variables.product.prodname_marketplace %} webhook for the app. If an organization has designated any app managers for a {% data variables.product.prodname_github_app %} owned by the organization, the app managers can also deactivate the {% data variables.product.prodname_marketplace %} webhook.

1. Navigate to your [{% data variables.product.prodname_marketplace %} listing page](https://github.com/marketplace/manage).
1. Next to the {% data variables.product.prodname_marketplace %} listing that you want to view webhook deliveries for, click **Manage listing**.
1. In the sidebar, click **Webhook**.
1. Deselect **Active**.
1. Click **Update webhook**.

## Disabling a {% data variables.product.prodname_sponsors %} webhook

You can disable webhooks that were previously enabled for events relating to {% data variables.product.prodname_sponsors %}. Only the owner of the sponsored account can disable sponsorship webhooks for that account. For more information, see "[AUTOTITLE](/sponsors/integrating-with-github-sponsors/configuring-webhooks-for-events-in-your-sponsored-account)."

{% endif %}

## Disabling webhooks for a {% data variables.product.prodname_github_app %}

You can disable webhook deliveries to your {% data variables.product.prodname_github_app %}, or change the events it subscribes to. For more information, see "[AUTOTITLE](/apps/maintaining-github-apps/modifying-a-github-app-registration#activating-or-deactivating-the-github-app-webhook)."