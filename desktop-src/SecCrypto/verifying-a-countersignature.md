---
Description: Explains how to verify a countersignature by using CryptMsgVerifyCountersignatureEncoded.
ms.assetid: b7be0d4c-338f-4319-bd82-5cf3d158d6fe
title: Verifying a Countersignature
ms.technology: desktop
ms.prod: windows
ms.author: windowssdkdev
ms.topic: article
ms.date: 05/31/2018
---

# Verifying a Countersignature

**To verify a countersignature**

1.  Call [**CryptMsgOpenToDecode**](/windows/desktop/api/Wincrypt/nf-wincrypt-cryptmsgopentodecode) to get a handle to the signed message.
2.  Get a pointer to the countersigner's certificate ( [**CERT\_INFO**](/windows/desktop/api/Wincrypt/ns-wincrypt-_cert_info)).
3.  Call [**CryptMsgGetParam**](/windows/desktop/api/Wincrypt/nf-wincrypt-cryptmsggetparam) to retrieve the signer information from the message.
4.  Call [**CryptMsgGetParam**](/windows/desktop/api/Wincrypt/nf-wincrypt-cryptmsggetparam) to retrieve the [*countersignature*](security.c_gly#-security-countersignature-gly) from the message.
5.  Call [**CryptMsgVerifyCountersignatureEncoded**](/windows/desktop/api/Wincrypt/nf-wincrypt-cryptmsgverifycountersignatureencoded) to verify the countersignature.

If the [**CryptMsgVerifyCountersignatureEncoded**](/windows/desktop/api/Wincrypt/nf-wincrypt-cryptmsgverifycountersignatureencoded) function call succeeds, the [*countersignature*](security.c_gly#-security-countersignature-gly) is verified.

 

 


