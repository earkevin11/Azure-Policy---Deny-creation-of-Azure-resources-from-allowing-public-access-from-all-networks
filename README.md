# Azure-Policy---Deny-creation-of-Azure-resources-from-allowing-public-access-from-all-networks

# Goal: Establish security baselines for the resources and policies I enforce against the management group.

# Job: Own creating/managing baseline documents related to the policies I am enforcing



# The Azure Initiative contains 2 policies:
1. Built in Policy 1: Storage accounts should restrict network access
2. Built in Policy 2: Azure Key Vault should have firewall enabled or public network access disabled
- I duplicated both and modified default to "Deny" and tested thoroughly

- <img width="1863" height="724" alt="image" src="https://github.com/user-attachments/assets/ac17d832-3fc2-4773-a92c-40f1d963752e" />

=======================================================================================

# Azure Storage Account

The custom policy will only allow users to create a new Storage Account that is in compliance with our security standards.
1. Option #1. Enable public access from selected virtual networks and IP addresses
2. Option #2 Disable public access and use private access

<img width="700" height="800" alt="image" src="https://github.com/user-attachments/assets/5fe3abe1-9a06-4036-afae-0c57df6642f1" />

# When users go to create a Storage account, the options are:
<img width="1312" height="397" alt="image" src="https://github.com/user-attachments/assets/ea7230f6-cdd6-49c1-b1ae-30be54e65957" />

# Impact: 84% of our Azure Storage Accounts were compliant. Remaining are in the backlog.
<img width="1764" height="838" alt="image" src="https://github.com/user-attachments/assets/de5dfccb-3fc0-4fbf-bf8e-ed6ead41bcca" />



=======================================================================================

# Azure Key Vault 

<img width="950" height="886" alt="image" src="https://github.com/user-attachments/assets/80c272d8-3aa5-4b69-a3e5-71b2cfde3623" />

# When users go to create the Azure Key Vault, the options are:
<img width="1154" height="228" alt="image" src="https://github.com/user-attachments/assets/40051777-6fd1-4f0d-b68d-ac2ab09173df" />



# Impact: 100% compliance of all key vaults in our management group

<img width="1767" height="848" alt="image" src="https://github.com/user-attachments/assets/4ef894fa-271b-417d-b04b-1eeffad23fcb" />



