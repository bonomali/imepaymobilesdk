# IME PAY Mobile SDK MERCHANT PAYMENT

Receive payment from your customer through IME pay.

Overview
--------

SDK Usage 
-----------
1. Add IME pay Android SDK dependency to your project using the .aar file

2. Create an object for `IMEPayment`
```java
IMEPayment imePayment = new IMEPayment(Activity.this);

imePayment.performPayment("MERCHANT_CODE",
                         "MERCHANT_NAME",
                         "PAYMENT_AMOUNT",
                         "CUSTOMER_MOBILENUMBER",
                         "MERCHANT_REFERENCE_VALUE",
                         "MERCHANT_MODULE",
                         "MERCHANT_USER",
                         "MERCHANT_PASSWORD",
                         new IMEPaymentCallback() {
                            @Override
                            public void onSucess(String s) {
                                Utils.showToast(Activity.this, "Payment Successful");
                            }
                        });
                
```

