# ChangePrimaryUser
This is based on David Falkus and Stefan van der Busse scripts

There is a need to change the Primary User inside Azure Active Directory to use the Logged On User rather than the enrolled user.  Prior to Windows AutoPilot, a machine would become enrolled automatically by an IT representative and subsequently would have a Primary User that mirrored that value.  This is not accurate for tracking assets and proves to be problematic when trying to connect the device to the end user for purposes of using Intune or software deployments.

Originally, following the article from March 21st, 2020 at https://svdbusse.github.io/SemiAnnualChat/2020/03/21/Changing-Intune-Primary-User-To-Last-Logged-On-User.html had some great ideas and options, but over time, the code has not been updated and needs some changes such as error checking due to functions having changed.