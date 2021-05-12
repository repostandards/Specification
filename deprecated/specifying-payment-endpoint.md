# Declaring Payment Endpoint Support

---

* Authors: Jamie Bishop
* Approvers: CoolStar
* Implementation Date: **December 29, 2018**

---

## Proposal
The standardized payment endpoint should be made available to the package manager via a route on the repo that returns a plain text URL for the repository's payment API.
> This only supports HTTPS capable repos and endpoints

Example:  
`GET https://repo.chariz.com/payment_endpoint`  
Returns `https://chariz.com/api/sileo/`  

In this scenario, `https://chariz.com/api/sileo/` is the base URL for documented payment endpoint API methods.
