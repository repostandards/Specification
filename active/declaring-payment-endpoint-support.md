# Declaring Payment Endpoint Support

* Authors: Aarnav Tale, Shuga, Adam Demasi
* Approvers: Hayden Seay, Andrew Wiik, Amy While, Wilson Styres
* Implementation Date: **May 12, 2021**
* Replaces Proposal Feature: [**Specifying-Payment-Endpoint**](../deprecated/specifying-payment-endpoint.md)
* Replaces Proposal Deprecation Date: **May 11, 2022**

## Proposal

The current solution for sending the payment endpoint to a client is via the hardcoded `/payment_endpoint` route. The proposal is to switch this to a more unified system.

> Keep in mind that these features only work on HTTPS repositories and endpoints.

The new way of specifying the repository's payment provider endpoint is via a `Payment-Provider` key within the _Release_ file.

**Example Release file**

```text
Origin: My Repo
Label: My Repo
...
Payment-Provider: https://api.my-repo.com/payments/
Description: Welcome to My Repo!
...
```

Commercial packages that use the payment provider supplied by the repository must be marked with the `works-with::payment-provider` tag in its control.

**Example Packages file**

```text
Package: com.shade.nougat
Name: Nougat
...
Description: Android NC for iOS
Maintainer: Shade Zepheri <ziroalpha@gmail.com>
Author: Shade Zepheri <ziroalpha@gmail.com>
Tag: works-with::payment-provider, compatible_min::ios10.0
Version: 1.3.1
...
```

