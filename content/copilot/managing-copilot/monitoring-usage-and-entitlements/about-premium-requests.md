---
title: About premium requests
intro: 'Learn about premium requests and how they impact your usage and billing.'
versions:
  feature: copilot
topics:
  - Copilot
redirect_from:
  - /copilot/managing-copilot/managing-copilot-as-an-individual-subscriber/monitoring-usage-and-entitlements/avoiding-unexpected-copilot-costs
  - /copilot/managing-copilot/monitoring-usage-and-entitlements/avoiding-unexpected-copilot-costs
---

<!-- expires 2025-05-05 -->
{% data reusables.copilot.unlimited-premium-requests %}
<!-- end expires 2025-05-05 -->

## What is a request?

A request is any interaction where you ask {% data variables.product.prodname_copilot_short %} to do something for you—whether it’s generating code, answering a question, or helping you through an extension. Each time you send a prompt in a chat window or trigger a response from {% data variables.product.prodname_copilot_short %}, you’re making a request.

If you have {% data variables.product.prodname_copilot_free_short %} enabled, your {% data variables.product.github %} account comes with up to 2,000 code completions and up to 50 chats or premium requests per month.

If you're on a paid plan, you get unlimited code completions, unlimited agent requests, and unlimited chat interactions using the base model. Rate limiting is in place to accommodate for high demand. Learn more about [current models and usage](/copilot/about-github-copilot/plans-for-github-copilot).

Paid plans also receive a monthly allowance of premium requests, which can be used for advanced chat interactions, code completions using premium models, and other premium features. For an overview of the amount of premium requests included in each plan, see [AUTOTITLE](/copilot/about-github-copilot/subscription-plans-for-github-copilot#comparing-copilot-plans).

## Premium requests

Some {% data variables.product.prodname_copilot_short %} features use more advanced processing power and count as premium requests. The number of premium requests a feature consumes can vary depending on the feature and the AI model used.

### Premium features

The following {% data variables.product.prodname_copilot_short %} features can use premium requests:

* {% data variables.product.prodname_copilot_chat_short %}
* {% data variables.product.prodname_copilot_agent_short %} mode
* {% data variables.product.prodname_copilot_short %} code review
* {% data variables.product.prodname_copilot_extensions_short %}

### Model multipliers

Each model has a premium request multiplier, based on its complexity and resource usage. Your premium request allowance is deducted according to this multiplier.

| Model                                                                   | Premium requests                                                             |
|-------------------------------------------------------------------------|------------------------------------------------------------------------------|
| Base model (currently {% data variables.copilot.copilot_gpt_4o %}) [^1] | 0 (paid users), 1 ({% data variables.product.prodname_copilot_free_short %}) |
| {% data variables.copilot.copilot_claude_sonnet_35 %}                   | 1                                                                            |
| {% data variables.copilot.copilot_claude_sonnet_37 %}                   | 1                                                                            |
| {% data variables.copilot.copilot_claude_sonnet_37 %} Thinking          | 1.25                                                                         |
| {% data variables.copilot.copilot_gemini_flash %}                       | 0.25                                                                         |
| {% data variables.copilot.copilot_gemini_25_pro %}                      | 1                                                                            |
| GPT-4.5                                                                 | 50                                                                           |
| {% data variables.copilot.copilot_o1 %}                                 | 10                                                                           |
| {% data variables.copilot.copilot_o3_mini %}                            | 0.33                                                                         |
[^1]: The base model at the time of writing is {% data variables.copilot.copilot_gpt_4o %}. This is subject to change. Response times for the base model may vary during periods of high usage. Requests to the base model may be subject to rate limiting.

## Additional premium requests

> [!NOTE]
> The option to purchase additional premium requests is not available to:
>
> * Users on {% data variables.product.prodname_copilot_free_short %}. To access more premium requests, upgrade to a paid plan.
> * Users who subscribe, or have subscribed, to {% data variables.product.prodname_copilot_pro_short %} or {% data variables.product.prodname_copilot_pro_plus_short %} through {% data variables.product.prodname_mobile %} on iOS or Android.

If you use all of your premium requests, you can still use {% data variables.product.prodname_copilot_short %} with the base model for the rest of the month. If you need more premium requests, you can upgrade to a higher plan or purchase additional premium requests. Additional premium requests beyond your plan’s included amount are billed at {% data variables.copilot.additional_premium_requests %} per request.

<!-- expires 2025-05-05 -->
> [!IMPORTANT]
> You will be able to enable additional premium requests in your account settings starting on{% ifversion ghec %} the following dates{% endif %}:
>
> * **May 5, 2025**: {% data variables.product.prodname_copilot_free_short %}, {% data variables.product.prodname_copilot_pro_short %}, and {% data variables.product.prodname_copilot_pro_plus_short %}{% ifversion ghec %}
> * **May 12, 2025**: Self-service (credit card) {% data variables.product.prodname_copilot_business_short %} and {% data variables.product.prodname_copilot_enterprise_short %}
> * **May 19, 2025**: Sales-served (invoiced) {% data variables.product.prodname_copilot_business_short %} and {% data variables.product.prodname_copilot_enterprise_short %}{% endif %}
<!-- end expires 2025-05-05 -->

To purchase additional premium requests, you’ll need to enable additional premium requests in your account settings first{% ifversion ghec %} or reach out to your {% data variables.product.prodname_enterprise %} administrator if you are on an enterprise plan{% endif %}. See [AUTOTITLE](/copilot/managing-copilot/managing-copilot-as-an-individual-subscriber/managing-your-copilot-plan/managing-copilot-policies-as-an-individual-subscriber){% ifversion fpt %} or{% else %},{% endif %} [AUTOTITLE](/copilot/managing-copilot/managing-github-copilot-in-your-organization/setting-policies-for-copilot-in-your-organization/managing-policies-for-copilot-in-your-organization){% ifversion ghec %}, or [AUTOTITLE](/copilot/managing-copilot/managing-copilot-for-your-enterprise/managing-policies-and-features-for-copilot-in-your-enterprise#additional-copilot-premium-requests){% endif %}.

Additionally, you must set a budget in your account settings{% ifversion ghec %} or ask your enterprise administrator to set one for your account{% endif %}.

## Example of premium request usage

Premium request usage is based on the model’s multiplier and the feature you’re using. For example:

* If you use **GPT-4.5** (50× multiplier) to ask a single question in {% data variables.product.prodname_copilot_chat_short %}, that interaction counts as **50 premium requests**.
* If you're on **{% data variables.product.prodname_copilot_free_short %}**, even interactions with the **base model** use **1 premium request** each.
* If you're on a **paid plan**, using the base model does not count against your monthly premium request allowance.

If you've enabled additional usage, premium requests beyond your included monthly amount will be billed at {% data variables.copilot.additional_premium_requests %} each.
