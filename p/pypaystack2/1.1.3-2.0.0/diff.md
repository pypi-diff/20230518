# Comparing `tmp/pypaystack2-1.1.3.tar.gz` & `tmp/pypaystack2-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pypaystack2-1.1.3.tar", max compression
+gzip compressed data, was "pypaystack2-2.0.0.tar", max compression
```

## Comparing `pypaystack2-1.1.3.tar` & `pypaystack2-2.0.0.tar`

### file list

```diff
@@ -1,34 +1,34 @@
--rw-r--r--   0        0        0     1079 2022-12-24 17:31:04.212452 pypaystack2-1.1.3/LICENSE
--rw-r--r--   0        0        0     3978 2023-03-10 10:12:18.157520 pypaystack2-1.1.3/README.md
--rw-r--r--   0        0        0      688 2023-03-10 10:54:35.486792 pypaystack2-1.1.3/pypaystack2/__init__.py
--rw-r--r--   0        0        0     3883 2023-03-10 10:52:49.476012 pypaystack2-1.1.3/pypaystack2/api/__init__.py
--rw-r--r--   0        0        0     1876 2022-12-25 04:20:11.696401 pypaystack2-1.1.3/pypaystack2/api/apple_pay.py
--rw-r--r--   0        0        0     5816 2022-12-25 04:20:11.696401 pypaystack2-1.1.3/pypaystack2/api/bulk_charges.py
--rw-r--r--   0        0        0     6923 2023-03-10 10:57:21.224195 pypaystack2-1.1.3/pypaystack2/api/charge.py
--rw-r--r--   0        0        0     1246 2022-12-25 04:20:11.696401 pypaystack2-1.1.3/pypaystack2/api/control_panel.py
--rw-r--r--   0        0        0     9160 2023-03-10 10:19:35.544340 pypaystack2-1.1.3/pypaystack2/api/customers.py
--rw-r--r--   0        0        0    11503 2023-03-10 10:03:57.779942 pypaystack2-1.1.3/pypaystack2/api/dedicated_accounts.py
--rw-r--r--   0        0        0     8748 2022-12-25 04:20:11.696401 pypaystack2-1.1.3/pypaystack2/api/disputes.py
--rw-r--r--   0        0        0    11032 2023-03-10 10:19:35.541007 pypaystack2-1.1.3/pypaystack2/api/invoices.py
--rw-r--r--   0        0        0     4000 2023-03-10 10:19:35.541007 pypaystack2-1.1.3/pypaystack2/api/miscellaneous.py
--rw-r--r--   0        0        0     6357 2023-03-10 10:19:35.541007 pypaystack2-1.1.3/pypaystack2/api/payment_pages.py
--rw-r--r--   0        0        0     2810 2022-12-25 04:20:11.696401 pypaystack2-1.1.3/pypaystack2/api/paystack.py
--rw-r--r--   0        0        0     6659 2022-12-25 04:20:11.696401 pypaystack2-1.1.3/pypaystack2/api/plans.py
--rw-r--r--   0        0        0     5877 2023-03-10 10:19:35.537674 pypaystack2-1.1.3/pypaystack2/api/products.py
--rw-r--r--   0        0        0     3916 2022-12-25 04:20:11.699734 pypaystack2-1.1.3/pypaystack2/api/refunds.py
--rw-r--r--   0        0        0     3374 2022-12-25 04:20:11.699734 pypaystack2-1.1.3/pypaystack2/api/settlements.py
--rw-r--r--   0        0        0     6756 2022-12-25 04:20:11.699734 pypaystack2-1.1.3/pypaystack2/api/splits.py
--rw-r--r--   0        0        0     7892 2022-12-25 04:20:11.699734 pypaystack2-1.1.3/pypaystack2/api/subaccounts.py
--rw-r--r--   0        0        0     5744 2023-03-10 10:19:35.541007 pypaystack2-1.1.3/pypaystack2/api/subscriptions.py
--rw-r--r--   0        0        0     7076 2023-03-10 10:19:35.544340 pypaystack2-1.1.3/pypaystack2/api/terminals.py
--rw-r--r--   0        0        0    22484 2022-12-25 04:20:11.699734 pypaystack2-1.1.3/pypaystack2/api/transactions.py
--rw-r--r--   0        0        0     7516 2022-12-25 04:20:11.699734 pypaystack2-1.1.3/pypaystack2/api/transfer_recipients.py
--rw-r--r--   0        0        0     4230 2022-12-25 04:20:11.699734 pypaystack2-1.1.3/pypaystack2/api/transfers.py
--rw-r--r--   0        0        0     3659 2022-12-25 04:20:11.699734 pypaystack2-1.1.3/pypaystack2/api/transfers_control.py
--rw-r--r--   0        0        0     3179 2023-03-10 10:19:35.541007 pypaystack2-1.1.3/pypaystack2/api/verification.py
--rw-r--r--   0        0        0     4069 2022-12-25 04:20:11.699734 pypaystack2-1.1.3/pypaystack2/baseapi.py
--rw-r--r--   0        0        0      471 2022-12-25 04:20:11.699734 pypaystack2-1.1.3/pypaystack2/errors.py
--rw-r--r--   0        0        0     8781 2022-12-25 04:20:11.699734 pypaystack2-1.1.3/pypaystack2/utils.py
--rw-r--r--   0        0        0      159 2023-03-10 10:21:42.011727 pypaystack2-1.1.3/pypaystack2/version.py
--rw-r--r--   0        0        0      869 2023-03-10 11:29:24.645240 pypaystack2-1.1.3/pyproject.toml
--rw-r--r--   0        0        0     4783 1970-01-01 00:00:00.000000 pypaystack2-1.1.3/PKG-INFO
+-rw-r--r--   0        0        0     1079 2023-05-18 18:19:22.020864 pypaystack2-2.0.0/LICENSE
+-rw-r--r--   0        0        0     1075 2023-05-18 18:19:22.020864 pypaystack2-2.0.0/README.md
+-rw-r--r--   0        0        0     1770 2023-05-18 18:19:22.024197 pypaystack2-2.0.0/pypaystack2/__init__.py
+-rw-r--r--   0        0        0      159 2023-05-18 18:19:22.024197 pypaystack2-2.0.0/pypaystack2/_metadata.py
+-rw-r--r--   0        0        0     3930 2023-05-18 18:19:22.024197 pypaystack2-2.0.0/pypaystack2/api/__init__.py
+-rw-r--r--   0        0        0     3924 2023-05-18 18:19:22.024197 pypaystack2-2.0.0/pypaystack2/api/apple_pay.py
+-rw-r--r--   0        0        0    10735 2023-05-18 18:19:22.024197 pypaystack2-2.0.0/pypaystack2/api/bulk_charges.py
+-rw-r--r--   0        0        0    12592 2023-05-18 18:19:22.027530 pypaystack2-2.0.0/pypaystack2/api/charge.py
+-rw-r--r--   0        0        0    16779 2023-05-18 18:19:22.027530 pypaystack2-2.0.0/pypaystack2/api/customers.py
+-rw-r--r--   0        0        0    21621 2023-05-18 18:19:22.027530 pypaystack2-2.0.0/pypaystack2/api/dedicated_accounts.py
+-rw-r--r--   0        0        0    15954 2023-05-18 18:19:22.027530 pypaystack2-2.0.0/pypaystack2/api/disputes.py
+-rw-r--r--   0        0        0     2387 2023-05-18 18:19:22.027530 pypaystack2-2.0.0/pypaystack2/api/integration.py
+-rw-r--r--   0        0        0     7214 2023-05-18 18:19:22.027530 pypaystack2-2.0.0/pypaystack2/api/miscellaneous.py
+-rw-r--r--   0        0        0    11648 2023-05-18 18:19:22.027530 pypaystack2-2.0.0/pypaystack2/api/payment_pages.py
+-rw-r--r--   0        0        0    20737 2023-05-18 18:19:22.027530 pypaystack2-2.0.0/pypaystack2/api/payment_requests.py
+-rw-r--r--   0        0        0    12243 2023-05-18 18:19:22.027530 pypaystack2-2.0.0/pypaystack2/api/plans.py
+-rw-r--r--   0        0        0    10712 2023-05-18 18:19:22.027530 pypaystack2-2.0.0/pypaystack2/api/products.py
+-rw-r--r--   0        0        0     7205 2023-05-18 18:19:22.027530 pypaystack2-2.0.0/pypaystack2/api/refunds.py
+-rw-r--r--   0        0        0     6360 2023-05-18 18:19:22.027530 pypaystack2-2.0.0/pypaystack2/api/settlements.py
+-rw-r--r--   0        0        0    12345 2023-05-18 18:19:22.027530 pypaystack2-2.0.0/pypaystack2/api/splits.py
+-rw-r--r--   0        0        0    14547 2023-05-18 18:19:22.027530 pypaystack2-2.0.0/pypaystack2/api/subaccounts.py
+-rw-r--r--   0        0        0    10647 2023-05-18 18:19:22.027530 pypaystack2-2.0.0/pypaystack2/api/subscriptions.py
+-rw-r--r--   0        0        0    13088 2023-05-18 18:19:22.027530 pypaystack2-2.0.0/pypaystack2/api/terminals.py
+-rw-r--r--   0        0        0    32495 2023-05-18 18:19:22.027530 pypaystack2-2.0.0/pypaystack2/api/transactions.py
+-rw-r--r--   0        0        0    13598 2023-05-18 18:19:22.027530 pypaystack2-2.0.0/pypaystack2/api/transfer_recipients.py
+-rw-r--r--   0        0        0     9574 2023-05-18 18:19:22.027530 pypaystack2-2.0.0/pypaystack2/api/transfers.py
+-rw-r--r--   0        0        0     7014 2023-05-18 18:19:22.027530 pypaystack2-2.0.0/pypaystack2/api/transfers_control.py
+-rw-r--r--   0        0        0     6234 2023-05-18 18:19:22.027530 pypaystack2-2.0.0/pypaystack2/api/verification.py
+-rw-r--r--   0        0        0     5043 2023-05-18 18:19:22.027530 pypaystack2-2.0.0/pypaystack2/baseapi.py
+-rw-r--r--   0        0        0      471 2023-05-18 18:19:22.030863 pypaystack2-2.0.0/pypaystack2/errors.py
+-rw-r--r--   0        0        0     6660 2023-05-18 18:19:22.030863 pypaystack2-2.0.0/pypaystack2/paystack.py
+-rw-r--r--   0        0        0    13981 2023-05-18 18:19:22.030863 pypaystack2-2.0.0/pypaystack2/utils.py
+-rw-r--r--   0        0        0      845 2023-05-18 18:19:22.030863 pypaystack2-2.0.0/pyproject.toml
+-rw-r--r--   0        0        0     1856 1970-01-01 00:00:00.000000 pypaystack2-2.0.0/PKG-INFO
```

### Comparing `pypaystack2-1.1.3/LICENSE` & `pypaystack2-2.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pypaystack2-1.1.3/pypaystack2/api/__init__.py` & `pypaystack2-2.0.0/pypaystack2/api/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -23,52 +23,52 @@
     - `transfers_control`: A module containing implementations for interfacing with Paystack's Transfers Control API
     - `verification`: A module containing implementations for interfacing with Paystack's Verification API
 """
 
 from pypaystack2.api.apple_pay import ApplePay
 from pypaystack2.api.bulk_charges import BulkCharge
 from pypaystack2.api.charge import Charge
-from pypaystack2.api.control_panel import ControlPanel
+from pypaystack2.api.integration import Integration
 from pypaystack2.api.customers import Customer
 from pypaystack2.api.dedicated_accounts import DedicatedAccount
 from pypaystack2.api.disputes import Dispute
-from pypaystack2.api.invoices import Invoice
+from pypaystack2.api.payment_requests import PaymentRequest
 from pypaystack2.api.miscellaneous import Miscellaneous
-from pypaystack2.api.payment_pages import Page
+from pypaystack2.api.payment_pages import PaymentPage
 from pypaystack2.api.plans import Plan
 from pypaystack2.api.products import Product
 from pypaystack2.api.refunds import Refund
 from pypaystack2.api.settlements import Settlement
-from pypaystack2.api.splits import Split
+from pypaystack2.api.splits import TransactionSplit
 from pypaystack2.api.subaccounts import SubAccount
 from pypaystack2.api.subscriptions import Subscription
 from pypaystack2.api.terminals import Terminal
 from pypaystack2.api.transactions import Transaction
-from pypaystack2.api.transfer_recipients import TransferRecipient
+from pypaystack2.api.transfer_recipients import RecipientType
 from pypaystack2.api.transfers import Transfer
 from pypaystack2.api.transfers_control import TransferControl
 from pypaystack2.api.verification import Verification
 
 # prevent removal of unused import
 ApplePay
 BulkCharge
 Charge
-ControlPanel
+Integration
 Customer
 DedicatedAccount
 Dispute
-Invoice
+PaymentRequest
 Miscellaneous
-Page
+PaymentPage
 Plan
 Product
 Refund
 Settlement
-Split
+TransactionSplit
 SubAccount
 Subscription
 Terminal
 Transaction
-TransferRecipient
+RecipientType
 Transfer
 TransferControl
-Verification
+Verification
```

### Comparing `pypaystack2-1.1.3/pypaystack2/api/charge.py` & `pypaystack2-2.0.0/pypaystack2/api/refunds.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,215 +1,201 @@
-from typing import Any, Optional
+from typing import Optional
 
-from ..baseapi import BaseAPI, Response
-from ..utils import add_to_payload, validate_amount
+from pypaystack2.baseapi import BaseAPI, BaseAsyncAPI
+from pypaystack2.utils import (
+    Currency,
+    add_to_payload,
+    append_query_params,
+    validate_amount,
+    HTTPMethod,
+    Response,
+)
 
 
-class Charge(BaseAPI):
-    """Provides a wrapper for paystack Charge API
-
-    The Charge API allows you to configure payment channel of your choice when initiating a payment.
-    https://paystack.com/docs/api/#charge
+class Refund(BaseAPI):
+    """Provides a wrapper for paystack Refunds API
 
+    The Refunds API allows you to create and manage transaction refunds.
+    https://paystack.com/docs/api/#refund
     """
 
-    def charge(
-            self,
-            email: str,
-            amount: int,
-            bank: Optional[dict[str, Any]] = None,
-            auth_code: Optional[str] = None,
-            pin: Optional[str] = None,
-            metadata: Optional[dict[str, Any]] = None,
-            reference: Optional[str] = None,
-            ussd: Optional[dict[str, Any]] = None,
-            mobile_money: Optional[dict[str, Any]] = None,
-            device_id: Optional[str] = None,
+    def create(
+        self,
+        transaction: str,
+        amount: Optional[int] = None,
+        currency: Optional[Currency] = None,
+        customer_note: Optional[str] = None,
+        merchant_note: Optional[str] = None,
     ) -> Response:
-        """Initiate a payment by integrating the payment channel of your choice.
+        """Initiate a refund on your integration
 
-        Parameters
-        ----------
-        email: str
-            Customer's email address
-        amount: int
-            Amount should be in kobo if currency is NGN, pesewas, if currency is GHS,
-            and cents, if currency is ZAR
-        bank: Optional[dict[str,Any]]
-            Bank account to charge (don't send if charging an authorization code)
-        auth_code: Optional[str]
-            An authorization code to charge (don't send if charging a bank account)
-        pin: Optional[str]
-            4-digit PIN (send with a non-reusable authorization code)
-        metadata: Optional[dict[str, Any]]
-            A dictionary of data.
-        reference: Optional[str]
-            Unique transaction reference. Only -, .\\`, = and alphanumeric characters allowed.
-        ussd: Optional[dict[str, Any]]
-            USSD type to charge (don't send if charging an authorization code, bank or card)
-        mobile_money: Optional[dict[str, Any]]
-            Mobile details (don't send if charging an authorization code, bank or card)
-        device_id: str
-            This is the unique identifier of the device a user uses in making payment. Only -, .\\`,
-            = and alphanumeric characters allowed.
-
-        Returns
-        -------
-        Response
+        Args:
+            transaction: Transaction reference or id
+            amount: Amount ( in kobo if currency is NGN, pesewas, if currency is
+                GHS, and cents, if currency is ZAR ) to be refunded to the
+                customer. Amount is optional(defaults to original
+                transaction amount) and cannot be more than the original
+                transaction amount
+            currency: Any value from the ``Currency`` enum
+            customer_note: Customer reason
+            merchant_note: Merchant reason
+
+        Returns:
             A named tuple containing the response gotten from paystack's server.
         """
 
-        amount = validate_amount(amount)
-        payload = {"email": email, "amount": amount}
+        if amount is not None:
+            amount = validate_amount(amount)
+        url = self._parse_url("/refund")
+        payload = {"transaction": transaction}
         optional_params = [
-            ("bank", bank),
-            ("authorization_code", auth_code),
-            ("pin", pin),
-            ("metadata", metadata),
-            ("reference", reference),
-            ("ussd", ussd),
-            ("mobile_money", mobile_money),
-            ("device_id", device_id),
+            ("amount", amount),
+            ("currency", currency),
+            ("customer_note", customer_note),
+            ("merchant_note", merchant_note),
         ]
         payload = add_to_payload(optional_params, payload)
-        url = self._url("/charge")
-        return self._handle_request("POST", url, payload)
+        return self._handle_request(HTTPMethod.POST, url, payload)
 
-    def submit_pin(self, pin: str, reference: str) -> Response:
-        """Submit PIN to continue a charge
+    def get_refunds(
+        self,
+        reference: Optional[str] = None,
+        currency: Optional[Currency] = None,
+        pagination: int = 50,
+        page: int = 1,
+        start_date: Optional[str] = None,
+        end_date: Optional[str] = None,
+    ) -> Response:
+        """Fetch refunds available on your integration.
 
-        Parameters
-        ----------
-        pin: str
-            PIN submitted by user
-        reference: str
-            Reference for transaction that requested pin
+        Args:
+            reference: Identifier for transaction to be refunded
+            currency: Any value from the ``Currency`` enum
+            pagination: Specifies how many records you want to retrieve per page.
+                If not specified we use a default value of 50.
+            page: Specifies exactly what refund you want to page.
+                If not specified we use a default value of 1.
+            start_date: A timestamp from which to start listing refund e.g. 2016-09-21
+            end_date: A timestamp at which to stop listing refund e.g. 2016-09-21
 
-        Returns
-        -------
-        Response
+        Returns:
             A named tuple containing the response gotten from paystack's server.
         """
 
-        payload = {"pin": pin, "reference": reference}
-        url = self._url("/charge/submit_pin")
-        return self._handle_request("POST", url, payload)
+        url = self._parse_url(f"/refund?perPage={pagination}")
+        query_params = [
+            ("reference", reference),
+            ("currency", currency),
+            ("page", page),
+            ("start_date", start_date),
+            ("end_date", end_date),
+        ]
+        url = append_query_params(query_params, url)
+        return self._handle_request(HTTPMethod.GET, url)
 
-    def submit_otp(self, otp: str, reference: str) -> Response:
-        """Submit OTP to complete a charge
+    def get_refund(self, reference: str) -> Response:
+        """Get details of a refund on your integration.
 
-        Parameters
-        ----------
-        otp: str
-            OTP submitted by user
-        reference: str
-            Reference for ongoing transaction
+        Args:
+            reference: Identifier for transaction to be refunded
 
-        Returns
-        -------
-        Response
+        Returns:
             A named tuple containing the response gotten from paystack's server.
         """
 
-        payload = {"otp": otp, "reference": reference}
-        url = self._url("/charge/submit_otp")
-        return self._handle_request("POST", url, payload)
+        url = self._parse_url(f"/refund/{reference}")
+        return self._handle_request(HTTPMethod.GET, url)
 
-    def submit_phone(self, phone: str, reference: str) -> Response:
-        """Submit Phone when requested
 
-        Parameters
-        ----------
-        phone: str
-            Phone submitted by user
-        reference:str
-            Reference for ongoing transaction
+class AsyncRefund(BaseAsyncAPI):
+    """Provides a wrapper for paystack Refunds API
+
+    The Refunds API allows you to create and manage transaction refunds.
+    https://paystack.com/docs/api/#refund
+    """
+
+    async def create(
+        self,
+        transaction: str,
+        amount: Optional[int] = None,
+        currency: Optional[Currency] = None,
+        customer_note: Optional[str] = None,
+        merchant_note: Optional[str] = None,
+    ) -> Response:
+        """Initiate a refund on your integration
 
-        Returns
-        -------
-        Response
+        Args:
+            transaction: Transaction reference or id
+            amount: Amount ( in kobo if currency is NGN, pesewas, if currency is
+                GHS, and cents, if currency is ZAR ) to be refunded to the
+                customer. Amount is optional(defaults to original
+                transaction amount) and cannot be more than the original
+                transaction amount
+            currency: Any value from the ``Currency`` enum
+            customer_note: Customer reason
+            merchant_note: Merchant reason
+
+        Returns:
             A named tuple containing the response gotten from paystack's server.
         """
 
-        payload = {"phone": phone, "reference": reference}
-        url = self._url("/charge/submit_phone")
-        return self._handle_request("POST", url, payload)
+        if amount is not None:
+            amount = validate_amount(amount)
+        url = self._parse_url("/refund")
+        payload = {"transaction": transaction}
+        optional_params = [
+            ("amount", amount),
+            ("currency", currency),
+            ("customer_note", customer_note),
+            ("merchant_note", merchant_note),
+        ]
+        payload = add_to_payload(optional_params, payload)
+        return await self._handle_request(HTTPMethod.POST, url, payload)
 
-    def submit_birthday(self, date: str, reference: str) -> Response:
-        """Submit Birthday when requested
+    async def get_refunds(
+        self,
+        reference: Optional[str] = None,
+        currency: Optional[Currency] = None,
+        pagination: int = 50,
+        page: int = 1,
+        start_date: Optional[str] = None,
+        end_date: Optional[str] = None,
+    ) -> Response:
+        """Fetch refunds available on your integration.
 
-        Parameters
-        ----------
-        date: str
-            Birthday submitted by user. ISO Format e.g. 2016-09-21
-        reference: str
-            Reference for ongoing transaction
+        Args:
+            reference: Identifier for transaction to be refunded
+            currency: Any value from the ``Currency`` enum
+            pagination: Specifies how many records you want to retrieve per page.
+                If not specified we use a default value of 50.
+            page: Specifies exactly what refund you want to page.
+                If not specified we use a default value of 1.
+            start_date: A timestamp from which to start listing refund e.g. 2016-09-21
+            end_date: A timestamp at which to stop listing refund e.g. 2016-09-21
 
-        Returns
-        -------
-        Response
+        Returns:
             A named tuple containing the response gotten from paystack's server.
         """
 
-        payload = {"date": date, "reference": reference}
-        url = self._url("/charge/submit_birthday")
-        return self._handle_request("POST", url, payload)
+        url = self._parse_url(f"/refund?perPage={pagination}")
+        query_params = [
+            ("reference", reference),
+            ("currency", currency),
+            ("page", page),
+            ("start_date", start_date),
+            ("end_date", end_date),
+        ]
+        url = append_query_params(query_params, url)
+        return await self._handle_request(HTTPMethod.GET, url)
 
-    def set_address(
-            self,
-            address: str,
-            reference: str,
-            city: str,
-            state: str,
-            zipcode: str,
-    ) -> Response:
-        """Submit address to continue a charge
+    async def get_refund(self, reference: str) -> Response:
+        """Get details of a refund on your integration.
 
-        Parameters
-        ----------
-        address: str
-            Address submitted by user
-        reference: str
-            Reference for ongoing transaction
-        city: str
-            City submitted by user
-        state: str
-            State submitted by user
-        zipcode: str
-            Zipcode submitted by user
-
-        Returns
-        -------
-        Response
-            A named tuple containing the response gotten from paystack's server.
-        """
+        Args:
+            reference: Identifier for transaction to be refunded
 
-        payload = {
-            "address": address,
-            "reference": reference,
-            "city": city,
-            "state": state,
-            "zipcode": zipcode,
-        }
-        url = self._url("/charge/submit_address")
-        return self._handle_request("POST", url, payload)
-
-    def check_pending_charge(self, reference: str) -> Response:
-        """
-        When you get "pending" as a charge status or if there was an
-        exception when calling any of the /charge endpoints, wait 10
-        seconds or more, then make a check to see if its status has changed.
-        Don't call too early as you may get a lot more pending than you should.
-
-        Parameters
-        ----------
-        reference: str
-            The reference to check
-
-        Returns
-        -------
-        Response
+        Returns:
             A named tuple containing the response gotten from paystack's server.
         """
 
-        url = self._url(f"/charge/{reference}")
-        return self._handle_request("GET", url)
+        url = self._parse_url(f"/refund/{reference}")
+        return await self._handle_request(HTTPMethod.GET, url)
```

### Comparing `pypaystack2-1.1.3/pypaystack2/api/customers.py` & `pypaystack2-2.0.0/pypaystack2/api/products.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,297 +1,305 @@
-from typing import Any, Optional
+from typing import Optional
 
-from ..baseapi import BaseAPI, Response
-from ..errors import InvalidDataError
-from ..utils import (
+from pypaystack2.baseapi import BaseAPI, BaseAsyncAPI
+from pypaystack2.errors import InvalidDataError
+from pypaystack2.utils import (
+    Currency,
     add_to_payload,
     append_query_params,
-    Identification,
-    Country,
-    RiskAction,
+    HTTPMethod,
+    Response,
 )
 
 
-class Customer(BaseAPI):
-    """Provides a wrapper for paystack Customer API
+class Product(BaseAPI):
+    """Provides a wrapper for paystack Products API
 
-    The Customers API allows you to create and manage customers on your integration.
-    https://paystack.com/docs/api/#customer
+    The Products API allows you to create and manage inventories on your integration.
+    https://paystack.com/docs/api/#product
     """
 
     def create(
         self,
-        email: str,
-        first_name: Optional[str] = None,
-        last_name: Optional[str] = None,
-        phone: Optional[str] = None,
-        metadata: Optional[dict[str, Any]] = None,
+        name: str,
+        description: str,
+        price: int,
+        currency: Currency,
+        unlimited: Optional[bool] = None,
+        quantity: Optional[int] = None,
     ) -> Response:
-        """Create a customer on your integration
+        """Create a product on your integration
 
-        Parameters
-        ----------
-        email: str
-            Customer's email address
-        first_name: Optional[str]
-            Customer's first name
-        last_name: Optional[str]
-            Customer's last name
-        phone: Optional[str]
-            Customer's phone number
-        metadata: Optional[dict[str,Any]]
-            A dictionary that you can attach to the customer. It can be used
-            to store additional information in a structured format.
-
-        Returns
-        -------
-        Response
+        Args:
+            name: Name of product
+            description: A description for this product
+            price: Price should be in kobo if currency is ``Currency.NGN``, pesewas,
+                if currency is ``Currency.GHS``, and cents, if currency is ``Currency.ZAR``
+            currency: Any value from the ``Currency`` enum
+            unlimited: Set to ``True`` if the product has unlimited stock.
+                Leave as ``False`` if the product has limited stock
+            quantity: Number of products in stock. Use if unlimited is ``False``
+
+        Returns:
             A named tuple containing the response gotten from paystack's server.
 
-        Note
-        ----
-        The `first_name`, `last_name` and `phone` are optional parameters. However,
-        when creating a customer that would be assigned a Dedicated Virtual
-        Account and your business catgeory falls under Betting, Financial
-        services, and General Service, then these parameters become compulsory.
+        Raises:
+            InvalidDataError: When unlimited is set to True and quantity has a value.
         """
 
-        url = self._url("/customer/")
+        if unlimited is True and quantity is not None:
+            raise InvalidDataError(
+                "You can't have unlimited set to True and have a quantity value."
+            )
+
+        url = self._parse_url("/product")
+
         payload = {
-            "email": email,
+            "name": name,
+            "description": description,
+            "price": price,
+            "currency": currency,
         }
-        optional_params = (
-            ("first_name", first_name),
-            ("last_name", last_name),
-            (
-                "phone",
-                phone,
-            ),
-            ("metadata", metadata),
-        )
+        optional_params = [
+            ("unlimited", unlimited),
+            ("quantity", quantity),
+        ]
         payload = add_to_payload(optional_params, payload)
-        return self._handle_request("POST", url, payload)
+        return self._handle_request(HTTPMethod.POST, url, payload)
 
-    def get_customers(
+    def get_products(
         self,
+        page: int = 1,
+        pagination: int = 50,
         start_date: Optional[str] = None,
         end_date: Optional[str] = None,
-        page=1,
-        pagination: int = 50,
     ) -> Response:
-        """Fetches customers available on your integration.
+        """Fetches products available on your integration.
+
+        Args:
+            page: Specifies exactly what page you want to retrieve.
+                If not specified we use a default value of 1.
+            pagination: Specifies how many records you want to retrieve per page.
+                If not specified we use a default value of 50.
+            start_date: A timestamp from which to start listing product e.g. 2016-09-24T00:00:05.000Z, 2016-09-21
+            end_date: timestamp at which to stop listing product e.g. 2016-09-24T00:00:05.000Z, 2016-09-21
 
-        Parameters
-        ----------
-        start_date: Optional[str]
-            A timestamp from which to start listing customers
-            e.g. 2016-09-24T00:00:05.000Z, 2016-09-21
-        end_date: Optional[str]
-            A timestamp at which to stop listing customers
-            e.g. 2016-09-24T00:00:05.000Z, 2016-09-21
-        page: int
-            Specify exactly what page you want to retrieve.
-            If not specify we use a default value of 1.
-        pagination: int
-            Specify how many records you want to retrieve per page.
-            If not specify we use a default value of 50.
-
-        Returns
-        -------
-        Response
+        Returns:
             A named tuple containing the response gotten from paystack's server.
         """
 
+        url = self._parse_url("/product?perPage=" + str(pagination))
         query_params = [
             ("page", page),
-            ("from", start_date),
-            ("to", end_date),
+            ("start_date", start_date),
+            ("end_date", end_date),
         ]
-        url = self._url(f"/customer/?perPage={pagination}")
         url = append_query_params(query_params, url)
-        return self._handle_request("GET", url)
+        return self._handle_request(HTTPMethod.GET, url)
+
+    def get_product(self, id: str) -> Response:
+        """Get details of a product on your integration.
 
-    def get_customer(self, email_or_code: str) -> Response:
-        """Get details of a customer on your integration.
+        Args:
+            id: The product ``ID`` you want to fetch
 
-        Parameters
-        ----------
-        email_or_code: str
-            An email or customer code for the customer you want to fetch
-
-        Returns
-        -------
-        Response
+        Returns:
             A named tuple containing the response gotten from paystack's server.
         """
 
-        url = self._url(f"/customer/{email_or_code}/")
-        return self._handle_request("GET", url)
+        url = self._parse_url(f"/product/{id}")
+        return self._handle_request(HTTPMethod.GET, url)
 
     def update(
         self,
-        code: str,
-        first_name: str,
-        last_name: str,
-        phone: Optional[str] = None,
-        metadata: Optional[dict[str, Any]] = None,
+        id: str,
+        name: str,
+        description: str,
+        price: int,
+        currency: Currency,
+        unlimited: Optional[bool] = None,
+        quantity: Optional[int] = None,
     ) -> Response:
-        """Update a customer's details on your integration
+        """Update a product details on your integration
 
-        Parameters
-        ----------
-        code: str
-            Customer's code
-        first_name: str
-            Customer's first name
-        last_name: str
-            Customer's last name
-        phone: Optional[str]
-            Customer's phone number
-        metadata: Optional[dict[str, Any]]
-            A dictionary that you can attach to the customer. It can be used
-            to store additional information in a structured format.
-
-        Returns
-        -------
-        Response
+        Args:
+            id: Product ID
+            name: Name of product
+            description: A description for this product
+            price: Price should be in kobo if currency is ``Currency.NGN``, pesewas,
+                if currency is GHS, and cents, if currency is ``Currency.ZAR``
+            currency: Any value from the ``Currency`` enum
+            unlimited: Set to ``True`` if the product has unlimited stock.
+                Leave as ``False`` if the product has limited stock
+            quantity: Number of products in stock. Use if unlimited is ``False``
+
+        Returns:
             A named tuple containing the response gotten from paystack's server.
+
+        Raises:
+            InvalidDataError: When unlimited is set to True and quantity has a value.
         """
 
-        url = self._url(f"/customer/{code}/")
+        if unlimited is True and quantity is not None:
+            raise InvalidDataError(
+                "You can't have unlimited set to True and quantity have a value."
+            )
+        url = self._parse_url(f"/product/{id}")
         payload = {
-            "first_name": first_name,
-            "last_name": last_name,
+            "name": name,
+            "description": description,
+            "price": price,
+            "currency": currency,
         }
-
         optional_params = [
-            (
-                "phone",
-                phone,
-            ),
-            ("metadata", metadata),
+            ("unlimited", unlimited),
+            ("quantity", quantity),
         ]
         payload = add_to_payload(optional_params, payload)
-        return self._handle_request("PUT", url, payload)
+        return self._handle_request(HTTPMethod.PUT, url, payload)
+
+
+class AsyncProduct(BaseAsyncAPI):
+    """Provides a wrapper for paystack Products API
 
-    def validate(
+    The Products API allows you to create and manage inventories on your integration.
+    https://paystack.com/docs/api/#product
+    """
+
+    async def create(
         self,
-        code: str,
-        first_name: str,
-        last_name: str,
-        identification_type: Identification,
-        identification_number: str,
-        country: Country,
-        bvn: str,
-        bank_code: Optional[str] = None,
-        account_number: Optional[str] = None,
-        middle_name: Optional[str] = None,
+        name: str,
+        description: str,
+        price: int,
+        currency: Currency,
+        unlimited: Optional[bool] = None,
+        quantity: Optional[int] = None,
     ) -> Response:
-        """Validate a customer's identity
+        """Create a product on your integration
+
+        Args:
+            name: Name of product
+            description: A description for this product
+            price: Price should be in kobo if currency is ``Currency.NGN``, pesewas,
+                if currency is ``Currency.GHS``, and cents, if currency is ``Currency.ZAR``
+            currency: Any value from the ``Currency`` enum
+            unlimited: Set to ``True`` if the product has unlimited stock.
+                Leave as ``False`` if the product has limited stock
+            quantity: Number of products in stock. Use if unlimited is ``False``
 
-        Parameters
-        ----------
-        code: str
-            Customer's code
-        first_name: str
-            Customer's first name
-        last_name: str
-            Customer's last name
-        identification_type: Identification
-            Enum of Identification e.g `Identification.BVN`
-        identification_number: str
-        country: Country
-            Enum of Country e.g `Country.NIGERIA`
-        bvn: str
-            Customer's Bank Verification Number
-        bank_code: Optional[str]
-            You can get the list of Bank Codes by calling the
-            Miscellaneous API `get_banks` method. (required if type is bank_account)
-        account_number: Optional[str]
-            Customer's bank account number. (required if type is bank_account)
-        middle_name: Optional[str]
-            Customer's middle name
-
-        Returns
-        -------
-        Response
+        Returns:
             A named tuple containing the response gotten from paystack's server.
+
+        Raises:
+            InvalidDataError: When unlimited is set to True and quantity has a value.
         """
 
-        if identification_type == Identification.BANK_ACCOUNT:
-            if bank_code is None:
-                raise InvalidDataError(
-                    "`bank_code` is required if identification type is `Identification.BANK_ACCOUNT`"
-                )
-            if account_number is None:
-                raise InvalidDataError(
-                    "`account_number` is required if identification type is `Identification.BANK_ACCOUNT`"
-                )
+        if unlimited is True and quantity is not None:
+            raise InvalidDataError(
+                "You can't have unlimited set to True and have a quantity value."
+            )
+
+        url = self._parse_url("/product")
 
-        url = self._url(f"/customer/{code}/identification")
         payload = {
-            "first_name": first_name,
-            "last_name": last_name,
-            "type": identification_type,
-            "value": identification_number,
-            "country": country,
-            "bvn": bvn,
+            "name": name,
+            "description": description,
+            "price": price,
+            "currency": currency,
         }
-        optional_params = (
-            ("bank_code", bank_code),
-            ("account_number", account_number),
-            ("middle_name", middle_name),
-        )
+        optional_params = [
+            ("unlimited", unlimited),
+            ("quantity", quantity),
+        ]
         payload = add_to_payload(optional_params, payload)
-        return self._handle_request("POST", url, payload)
+        return await self._handle_request(HTTPMethod.POST, url, payload)
 
-    def flag(
+    async def get_products(
         self,
-        customer: str,
-        risk_action: Optional[RiskAction] = None,
+        page: int = 1,
+        pagination: int = 50,
+        start_date: Optional[str] = None,
+        end_date: Optional[str] = None,
     ) -> Response:
-        """Whitelist or blacklist a customer on your integration
+        """Fetches products available on your integration.
+
+        Args:
+            page: Specifies exactly what page you want to retrieve.
+                If not specified we use a default value of 1.
+            pagination: Specifies how many records you want to retrieve per page.
+                If not specified we use a default value of 50.
+            start_date: A timestamp from which to start listing product e.g. 2016-09-24T00:00:05.000Z, 2016-09-21
+            end_date: timestamp at which to stop listing product e.g. 2016-09-24T00:00:05.000Z, 2016-09-21
 
-        Parameters
-        ----------
-        customer: str
-            Customer's code, or email address
-        risk_action: Optional[RiskAction]
-            One of the possible risk actions from the
-            RiskAction enum e.g `RiskAction.DEFAULT`
-
-        Returns
-        -------
-        Response
+        Returns:
             A named tuple containing the response gotten from paystack's server.
         """
 
-        url = self._url("/customer/set_risk_action")
-        payload = {
-            "customer": customer,
-        }
-        optional_params = (("risk_action", risk_action),)
-        payload = add_to_payload(optional_params, payload)
-        return self._handle_request("POST", url, payload)
+        url = self._parse_url("/product?perPage=" + str(pagination))
+        query_params = [
+            ("page", page),
+            ("start_date", start_date),
+            ("end_date", end_date),
+        ]
+        url = append_query_params(query_params, url)
+        return await self._handle_request(HTTPMethod.GET, url)
+
+    async def get_product(self, id: str) -> Response:
+        """Get details of a product on your integration.
 
-    def deactivate(
+        Args:
+            id: The product ``ID`` you want to fetch
+
+        Returns:
+            A named tuple containing the response gotten from paystack's server.
+        """
+
+        url = self._parse_url(f"/product/{id}")
+        return await self._handle_request(HTTPMethod.GET, url)
+
+    async def update(
         self,
-        auth_code: str,
+        id: str,
+        name: str,
+        description: str,
+        price: int,
+        currency: Currency,
+        unlimited: Optional[bool] = None,
+        quantity: Optional[int] = None,
     ) -> Response:
-        """Deactivate an authorization when the card needs to be forgotten
+        """Update a product details on your integration
 
-        Parameters
-        ----------
-        auth_code: str
-            Authorization code to be deactivated
-
-        Returns
-        -------
-        Response
+        Args:
+            id: Product ID
+            name: Name of product
+            description: A description for this product
+            price: Price should be in kobo if currency is ``Currency.NGN``, pesewas,
+                if currency is GHS, and cents, if currency is ``Currency.ZAR``
+            currency: Any value from the ``Currency`` enum
+            unlimited: Set to ``True`` if the product has unlimited stock.
+                Leave as ``False`` if the product has limited stock
+            quantity: Number of products in stock. Use if unlimited is ``False``
+
+        Returns:
             A named tuple containing the response gotten from paystack's server.
+
+        Raises:
+            InvalidDataError: When unlimited is set to True and quantity has a value.
         """
 
-        url = self._url("/customer/deactivate_authorization")
+        if unlimited is True and quantity is not None:
+            raise InvalidDataError(
+                "You can't have unlimited set to True and quantity have a value."
+            )
+        url = self._parse_url(f"/product/{id}")
         payload = {
-            "authorization_code": auth_code,
+            "name": name,
+            "description": description,
+            "price": price,
+            "currency": currency,
         }
-        return self._handle_request("POST", url, payload)
+        optional_params = [
+            ("unlimited", unlimited),
+            ("quantity", quantity),
+        ]
+        payload = add_to_payload(optional_params, payload)
+        return await self._handle_request(HTTPMethod.PUT, url, payload)
```

### Comparing `pypaystack2-1.1.3/pypaystack2/api/invoices.py` & `pypaystack2-2.0.0/pypaystack2/api/payment_pages.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,319 +1,323 @@
-from typing import Any, Optional
+from typing import Optional
 
-from ..baseapi import BaseAPI, Response
-from ..utils import (
-    Currency,
-    InvoiceStatus,
-    add_to_payload,
-    append_query_params,
-    validate_amount,
-)
 
+from pypaystack2.baseapi import BaseAPI, BaseAsyncAPI
+from pypaystack2.utils import add_to_payload, append_query_params, HTTPMethod, Response
 
-class Invoice(BaseAPI):
-    """Provides a wrapper for paystack Invoices API
 
-    The Invoices API allows you to issue out and manage payment requests.
-    https://paystack.com/docs/api/#invoice
+class PaymentPage(BaseAPI):
+    """Provides a wrapper for paystack Payment Pages API
+
+    The Payment Pages API provides a quick and secure way to collect payment for products.
+    https://paystack.com/docs/api/#page
     """
 
     def create(
         self,
-        customer: str,
-        amount: int,
-        due_date: Optional[str] = None,
+        name: str,
         description: Optional[str] = None,
-        line_items: Optional[list[dict[str, Any]]] = None,
-        tax: Optional[list[dict[str, Any]]] = None,
-        currency: Optional[Currency] = None,
-        send_notification: Optional[bool] = None,
-        draft: Optional[bool] = None,
-        has_invoice: Optional[bool] = None,
-        invoice_number: Optional[int] = None,
-        split_code: Optional[str] = None,
+        amount: Optional[int] = None,
+        slug: Optional[str] = None,
+        metadata: Optional[str] = None,
+        redirect_url: Optional[str] = None,
+        custom_fields: Optional[list] = None,
     ) -> Response:
-        """Create an invoice for payment on your integration
+        """Create a payment page on your integration
 
-        Parameters
-        ----------
-        customer: str
-            Customer id or code
-        amount: int
-            Payment request amount. It should be used when line items and
-            tax values aren't specified.
-        due_date: Optional[str]
-            ISO 8601 representation of request due date
-        description: Optional[str]
-            A short description of the payment request
-        line_items: Optional[list[dict[str,Any]]]
-            List of line items int the format [{"name":"item 1", "amount":2000, "quantity": 1}]
-        tax: Optional[list[dict[str,Any]]]
-            List of taxes to be charged in the format [{"name":"VAT", "amount":2000}]
-        currency: Optional[Currency]
-            Any value from Currency enum. default ``Currency.NGN``
-        send_notification: Optional[bool]
-            Indicates whether Paystack sends an email notification to customer. Defaults to ``True``
-        draft: Optional[bool]
-            Indicate if request should be saved as draft. Defaults to ``False`` and overrides
-            send_notification
-        has_invoice: Optional[bool]
-            Set to ``True`` to create a draft invoice (adds an auto incrementing invoice number
-            if none is provided) even if there are no line_items or tax passed
-        invoice_number: Optional[int]
-            Numeric value of invoice. Invoice will start from 1 and auto increment from there.
-            This field is to help override whatever value Paystack decides. Auto increment for
-            subsequent invoices continue from this point.
-        split_code: Optional[str]
-            The split code of the transaction split. e.g. SPL_98WF13Eb3w
-
-        Returns
-        -------
-        Response
+        Args:
+            name: Name of page
+            description: A description for this page
+            amount: Amount should be in kobo if currency is ``Currency.NGN``, pesewas, if
+                currency is ``Currency.GHS``, and cents, if currency is ``Currency.ZAR``
+            slug: URL slug you would like to be associated with this page.
+                Page will be accessible at ``https://paystack.com/pay/[slug]``
+            metadata: Extra data to configure the payment page including subaccount,
+                logo image, transaction charge
+            redirect_url: If you would like Paystack to redirect someplace upon
+                successful payment, specify the URL here.
+            custom_fields: If you would like to accept custom fields,
+                specify them here.
+
+        Returns:
             A named tuple containing the response gotten from paystack's server.
         """
 
-        url = self._url("/paymentrequest")
+        url = self._parse_url("/page")
 
-        payload = {"customer": customer, "amount": amount}
+        payload = {"name": name}
         optional_params = [
-            ("due_date", due_date),
             ("description", description),
-            ("line_items", line_items),
-            ("tax", tax),
-            ("currency", currency),
-            ("send_notification", send_notification),
-            ("draft", draft),
-            ("has_invoice", has_invoice),
-            ("invoice_number", invoice_number),
-            ("split_code", split_code),
+            ("amount", amount),
+            ("slug", slug),
+            ("metadata", metadata),
+            ("redirect_url", redirect_url),
+            ("custom_fields", custom_fields),
         ]
         payload = add_to_payload(optional_params, payload)
-        return self._handle_request("POST", url, payload)
+        return self._handle_request(HTTPMethod.POST, url, payload)
 
-    def get_invoices(
+    def get_pages(
         self,
-        customer: str,
-        status: InvoiceStatus,
-        currency: Currency,
-        include_archive=False,
-        page=1,
-        pagination=50,
+        page: int = 1,
+        pagination: int = 50,
         start_date: Optional[str] = None,
         end_date: Optional[str] = None,
     ) -> Response:
-        """Fetches the invoice available on your integration.
+        """Fetch payment pages available on your integration.
+
+        Args:
+            page: Specifies exactly what page you want to retrieve.
+                If not specified we use a default value of 1.
+            pagination: Specifies how many records you want to retrieve per page.
+                If not specified we use a default value of 50.
+            start_date: A timestamp from which to start listing page e.g. 2016-09-24T00:00:05.000Z, 2016-09-21
+            end_date: A timestamp at which to stop listing page e.g. 2016-09-24T00:00:05.000Z, 2016-09-21
 
-        Parameters
-        ----------
-        customer: str
-            Filter by customer ID
-        status: InvoiceStatus
-            Filter by invoice status. Any value from enum of ``InvoiceStatus``
-        currency: Currency
-            Filter by currency. Any value from enum of ``Currency``
-        include_archive: bool
-            Show archived invoices.
-        page: int
-            Specify exactly what invoice you want to page. If not specify we use a
-            default value of 1.
-        pagination: int
-            Specify how many records you want to retrieve per page. If not specify
-            we use a default value of 50.
-        start_date: Optional[str]
-            A timestamp from which to start listing invoice
-            e.g. 2016-09-24T00:00:05.000Z, 2016-09-21
-        end_date: Optional[str]
-            A timestamp at which to stop listing invoice
-            e.g. 2016-09-24T00:00:05.000Z, 2016-09-21
-
-        Returns
-        -------
-        Response
+        Returns:
             A named tuple containing the response gotten from paystack's server.
         """
 
-        url = self._url(f"/paymentrequest?perPage={pagination}")
+        url = self._parse_url("/page?perPage=" + str(pagination))
         query_params = [
-            ("customer", customer),
-            ("status", status),
-            ("currency", currency),
-            ("include_archive", include_archive),
             ("page", page),
             ("start_date", start_date),
             ("end_date", end_date),
         ]
         url = append_query_params(query_params, url)
-        return self._handle_request("GET", url)
+        return self._handle_request(HTTPMethod.GET, url)
 
-    def get_invoice(self, id_or_code: str) -> Response:
-        """Get details of an invoice on your integration.
+    def get_page(self, id_or_slug: str) -> Response:
+        """Get details of a payment page on your integration.
 
-        Parameters
-        ----------
-        id_or_code: str
-            The invoice ID or code you want to fetch
+        Args:
+            id_or_slug: The page ``ID`` or ``slug`` you want to fetch
 
-        Returns
-        -------
-        Response
+        Returns:
             A named tuple containing the response gotten from paystack's server.
         """
 
-        url = self._url(f"/paymentrequest/{id_or_code}")
-        return self._handle_request("GET", url)
+        url = self._parse_url(f"/page/{id_or_slug}")
+        return self._handle_request(HTTPMethod.GET, url)
 
-    def verify_invoice(self, code: str) -> Response:
-        """Verify details of an invoice on your integration.
+    def update(
+        self,
+        id_or_slug: str,
+        name: str,
+        description: str,
+        amount: int,
+        active: Optional[bool] = None,
+    ) -> Response:
+        """Get details of a payment page on your integration.
 
-        Parameters
-        ----------
-        code: str
-            Invoice code
+        Args:
+            id_or_slug: The page ``ID`` or ``slug`` you want to fetch
+            name: Name of page
+            description: A description for the page
+            amount: Default amount you want to accept using this page.
+                If none is set, customer is free to provide any amount
+                of their choice. The latter scenario is useful for
+                accepting donations
+            active: Set to ``False`` to deactivate page url
 
-        Returns
-        -------
-        Response
+        Returns:
             A named tuple containing the response gotten from paystack's server.
         """
 
-        url = self._url(f"/paymentrequest/verify/{code}")
-        return self._handle_request("GET", url)
+        url = self._parse_url(f"/page/{id_or_slug}")
+        payload = {
+            "name": name,
+            "description": description,
+        }
+        optional_params = [
+            ("amount", amount),
+            ("active", active),
+        ]
+        payload = add_to_payload(optional_params, payload)
+        return self._handle_request(HTTPMethod.PUT, url, payload)
 
-    def send_notification(self, code: str) -> Response:
-        """Send notification of an invoice to your customers
+    def check_slug_available(self, slug: str) -> Response:
+        """Check the availability of a slug for a payment page.
 
-        Parameters
-        ----------
-        code: str
-            Invoice code
+        Args:
+            slug: URL slug to be confirmed
 
-        Returns
-        -------
-        Response
+        Returns:
             A named tuple containing the response gotten from paystack's server.
         """
 
-        url = self._url(f"/paymentrequest/notify/{code}")
-        return self._handle_request("POST", url)
+        url = self._parse_url(f"/page/check_slug_availability/{slug}")
+        return self._handle_request(HTTPMethod.GET, url)
 
-    def get_total(self) -> Response:
-        """Get invoice metrics for dashboard
+    def add_products(self, id: str, products: list[int]) -> Response:
+        """Add products to a payment page
 
-        Returns
-        -------
-        Response
+        Args:
+            id: ID of the payment page
+            products: Ids of all the products
+
+        Returns:
             A named tuple containing the response gotten from paystack's server.
         """
 
-        url = self._url("/paymentrequest/totals")
-        return self._handle_request("GET", url)
+        url = self._parse_url(f"/page/{id}/product")
+        payload = {"product": products}
+        return self._handle_request(HTTPMethod.POST, url, payload)
+
+
+class AsyncPaymentPage(BaseAsyncAPI):
+    """Provides a wrapper for paystack Payment Pages API
 
-    def finalize_invoice(self, code: str) -> Response:
-        """Finalize a Draft Invoice
+    The Payment Pages API provides a quick and secure way to collect payment for products.
+    https://paystack.com/docs/api/#page
+    """
+
+    async def create(
+        self,
+        name: str,
+        description: Optional[str] = None,
+        amount: Optional[int] = None,
+        slug: Optional[str] = None,
+        metadata: Optional[str] = None,
+        redirect_url: Optional[str] = None,
+        custom_fields: Optional[list] = None,
+    ) -> Response:
+        """Create a payment page on your integration
 
-        Parameters
-        ----------
-        code: str
-            Invoice Code
+        Args:
+            name: Name of page
+            description: A description for this page
+            amount: Amount should be in kobo if currency is ``Currency.NGN``, pesewas, if
+                currency is ``Currency.GHS``, and cents, if currency is ``Currency.ZAR``
+            slug: URL slug you would like to be associated with this page.
+                Page will be accessible at ``https://paystack.com/pay/[slug]``
+            metadata: Extra data to configure the payment page including subaccount,
+                logo image, transaction charge
+            redirect_url: If you would like Paystack to redirect someplace upon
+                successful payment, specify the URL here.
+            custom_fields: If you would like to accept custom fields,
+                specify them here.
 
-        Returns
-        -------
-        Response
+        Returns:
             A named tuple containing the response gotten from paystack's server.
         """
 
-        url = self._url(f"/paymentrequest/finalize/{code}")
-        return self._handle_request("POST", url)
+        url = self._parse_url("/page")
 
-    def update_invoice(
+        payload = {"name": name}
+        optional_params = [
+            ("description", description),
+            ("amount", amount),
+            ("slug", slug),
+            ("metadata", metadata),
+            ("redirect_url", redirect_url),
+            ("custom_fields", custom_fields),
+        ]
+        payload = add_to_payload(optional_params, payload)
+        return await self._handle_request(HTTPMethod.POST, url, payload)
+
+    async def get_pages(
         self,
-        id_or_code: str,
-        customer: str,
-        amount: int,
-        due_date: Optional[str] = None,
-        description: Optional[str] = None,
-        line_items: Optional[list[dict[str, Any]]] = None,
-        tax: Optional[list[dict[str, Any]]] = None,
-        currency: Optional[Currency] = None,
-        send_notification: Optional[bool] = None,
-        draft: Optional[bool] = None,
-        invoice_number: Optional[int] = None,
-        split_code: Optional[str] = None,
-    ):
-        """Update an invoice details on your integration
-
-        Parameters
-        ----------
-        id_or_code: str
-            Invoice ID or slug
-        customer: str
-            Customer id or code
-        amount: int
-            Payment request amount. Only useful if line items and tax values are ignored.
-            method will throw a friendly warning in the response if neither is available.
-        due_date: Optional[str]
-            ISO 8601 representation of request due date
-        description: Optional[str]
-            A short description of the payment request
-        line_items: Optional[list[dict[str,Any]]]
-            List of line items in the format [{"name":"item 1", "amount":2000}]
-        tax: Optional[list[dict[str,Any]]]
-            List of taxes to be charged in the format [{"name":"VAT", "amount":2000}]
-        currency: Optional[Currency]
-            Specify the currency of the invoice. Any value from the ``Currency`` enum
-        send_notification: Optional[bool]
-            Indicates whether Paystack sends an email notification to customer. Defaults to ``True``
-        draft: Optional[bool]
-            Indicate if request should be saved as draft. Defaults to false and overrides
-            send_notification
-        invoice_number: Optional[int]
-            Numeric value of invoice. Invoice will start from 1 and auto increment from there.
-            This field is to help override whatever value Paystack decides. Auto increment for
-            subsequent invoices continue from this point.
-        split_code: Optional[str]
-            The split code of the transaction split. e.g. SPL_98WF13Eb3w
-
-        Returns
-        -------
-        Response
+        page: int = 1,
+        pagination: int = 50,
+        start_date: Optional[str] = None,
+        end_date: Optional[str] = None,
+    ) -> Response:
+        """Fetch payment pages available on your integration.
+
+        Args:
+            page: Specifies exactly what page you want to retrieve.
+                If not specified we use a default value of 1.
+            pagination: Specifies how many records you want to retrieve per page.
+                If not specified we use a default value of 50.
+            start_date: A timestamp from which to start listing page e.g. 2016-09-24T00:00:05.000Z, 2016-09-21
+            end_date: A timestamp at which to stop listing page e.g. 2016-09-24T00:00:05.000Z, 2016-09-21
+
+        Returns:
             A named tuple containing the response gotten from paystack's server.
         """
 
-        amount = validate_amount(amount)
+        url = self._parse_url("/page?perPage=" + str(pagination))
+        query_params = [
+            ("page", page),
+            ("start_date", start_date),
+            ("end_date", end_date),
+        ]
+        url = append_query_params(query_params, url)
+        return await self._handle_request(HTTPMethod.GET, url)
 
-        url = self._url(f"/paymentrequest/{id_or_code}")
+    async def get_page(self, id_or_slug: str) -> Response:
+        """Get details of a payment page on your integration.
+
+        Args:
+            id_or_slug: The page ``ID`` or ``slug`` you want to fetch
+
+        Returns:
+            A named tuple containing the response gotten from paystack's server.
+        """
+
+        url = self._parse_url(f"/page/{id_or_slug}")
+        return await self._handle_request(HTTPMethod.GET, url)
+
+    async def update(
+        self,
+        id_or_slug: str,
+        name: str,
+        description: str,
+        amount: int,
+        active: Optional[bool] = None,
+    ) -> Response:
+        """Get details of a payment page on your integration.
+
+        Args:
+            id_or_slug: The page ``ID`` or ``slug`` you want to fetch
+            name: Name of page
+            description: A description for the page
+            amount: Default amount you want to accept using this page.
+                If none is set, customer is free to provide any amount
+                of their choice. The latter scenario is useful for
+                accepting donations
+            active: Set to ``False`` to deactivate page url
+
+        Returns:
+            A named tuple containing the response gotten from paystack's server.
+        """
+
+        url = self._parse_url(f"/page/{id_or_slug}")
         payload = {
-            "customer": customer,
-            "amount": amount,
+            "name": name,
+            "description": description,
         }
         optional_params = [
-            ("due_date", due_date),
-            ("description", description),
-            ("line_items", line_items),
-            ("tax", tax),
-            ("currency", currency),
-            ("send_notification", send_notification),
-            ("draft", draft),
-            ("invoice_number", invoice_number),
-            ("split_code", split_code),
+            ("amount", amount),
+            ("active", active),
         ]
         payload = add_to_payload(optional_params, payload)
-        return self._handle_request("PUT", url, payload)
+        return await self._handle_request(HTTPMethod.PUT, url, payload)
+
+    async def check_slug_available(self, slug: str) -> Response:
+        """Check the availability of a slug for a payment page.
+
+        Args:
+            slug: URL slug to be confirmed
+
+        Returns:
+            A named tuple containing the response gotten from paystack's server.
+        """
+
+        url = self._parse_url(f"/page/check_slug_availability/{slug}")
+        return await self._handle_request(HTTPMethod.GET, url)
 
-    def archive_invoice(self, code: str):
-        """Used to archive an invoice. Invoice will no longer be fetched
-        on list or returned on verify.
+    async def add_products(self, id: str, products: list[int]) -> Response:
+        """Add products to a payment page
 
-        Parameters
-        ----------
-        code: str
-            Invoice ID
+        Args:
+            id: ID of the payment page
+            products: Ids of all the products
 
-         Returns
-        -------
-        Response
+        Returns:
             A named tuple containing the response gotten from paystack's server.
         """
 
-        url = self._url(f"/paymentrequest/archive/{code}")
-        return self._handle_request("POST", url)
+        url = self._parse_url(f"/page/{id}/product")
+        payload = {"product": products}
+        return await self._handle_request(HTTPMethod.POST, url, payload)
```

### Comparing `pypaystack2-1.1.3/pypaystack2/api/payment_pages.py` & `pypaystack2-2.0.0/pypaystack2/api/settlements.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,204 +1,158 @@
 from typing import Optional
 
+from pypaystack2.baseapi import BaseAPI, BaseAsyncAPI
+from pypaystack2.utils import (
+    append_query_params,
+    HTTPMethod,
+    Response,
+)
 
-from pypaystack2.baseapi import BaseAPI, Response
-from pypaystack2.utils import add_to_payload, append_query_params
 
+class Settlement(BaseAPI):
+    """Provides a wrapper for paystack Settlement API
 
-class Page(BaseAPI):
-    """Provides a wrapper for paystack Payment Pages API
-
-    The Payment Pages API provides a quick and secure way to collect payment for products.
-    https://paystack.com/docs/api/#page
+    The Settlements API allows you gain insights into payouts made by Paystack to your bank account.
+    https://paystack.com/docs/api/#settlement
     """
 
-    def create(
+    def get_settlements(
         self,
-        name: str,
-        description: Optional[str] = None,
-        amount: Optional[int] = None,
-        slug: Optional[str] = None,
-        metadata: Optional[str] = None,
-        redirect_url: Optional[str] = None,
-        custom_fields: Optional[list] = None,
+        page: int = 1,
+        pagination: int = 50,
+        start_date: Optional[str] = None,
+        end_date: Optional[str] = None,
+        subaccount: Optional[str] = None,
     ) -> Response:
-        """Create a payment page on your integration
+        """Fetch settlements made to your settlement accounts.
 
-        Parameters
-        ----------
-        name: str
-            Name of page
-        description: Optional[str]
-            A description for this page
-        amount: Optional[int]
-            Amount should be in kobo if currency is ``Currency.NGN``, pesewas, if
-            currency is ``Currency.GHS``, and cents, if currency is ``Currency.ZAR``
-        slug: Optional[str]
-            URL slug you would like to be associated with this page.
-            Page will be accessible at ``https://paystack.com/pay/[slug]``
-        metadata: Optional[str]
-            Extra data to configure the payment page including subaccount,
-            logo image, transaction charge
-        redirect_url: Optional[str]
-            If you would like Paystack to redirect someplace upon
-            successful payment, specify the URL here.
-        custom_fields: Optional[list]
-            If you would like to accept custom fields,
-            specify them here.
-
-        Returns
-        -------
-        Response
+        Args:
+            page: Specifies exactly what page you want to retrieve.
+                If not specified we use a default value of 1.
+            pagination: Specifies how many records you want to retrieve per page.
+                If not specified we use a default value of 50.
+            start_date: A timestamp from which to start listing settlements e.g. 2016-09-24T00:00:05.000Z, 2016-09-21
+            end_date: A timestamp at which to stop listing settlements e.g. 2016-09-24T00:00:05.000Z, 2016-09-21
+            subaccount: Provide a subaccount ID to export only settlements for that subaccount.
+                Set to ``none`` to export only transactions for the account.
+
+        Returns:
             A named tuple containing the response gotten from paystack's server.
         """
 
-        url = self._url("/page")
-
-        payload = {"name": name}
-        optional_params = [
-            ("description", description),
-            ("amount", amount),
-            ("slug", slug),
-            ("metadata", metadata),
-            ("redirect_url", redirect_url),
-            ("custom_fields", custom_fields),
+        url = self._parse_url(f"/settlement?perPage={pagination}")
+        query_params = [
+            ("subaccount", subaccount),
+            ("page", page),
+            ("start_date", start_date),
+            ("end_date", end_date),
         ]
-        payload = add_to_payload(optional_params, payload)
-        return self._handle_request("POST", url, payload)
+        url = append_query_params(query_params, url)
+        return self._handle_request(HTTPMethod.GET, url)
 
-    def get_pages(
+    def get_settlement_transactions(
         self,
-        page=1,
-        pagination=50,
+        id: str,
+        pagination: int = 50,
+        page: int = 1,
         start_date: Optional[str] = None,
         end_date: Optional[str] = None,
     ) -> Response:
-        """Fetch payment pages available on your integration.
+        """Get the transactions that make up a particular settlement
+
+        Args:
+            id: The settlement ID in which you want to fetch its transactions
+            pagination: Specifies how many records you want to retrieve per page. If not specified we
+                use a default value of 50.
+            page: Specifies exactly what page you want to retrieve. If not specified we use a default value of 1.
+            start_date: A timestamp from which to start listing settlement transactions
+                e.g. 2016-09-24T00:00:05.000Z, 2016-09-21
+            end_date: A timestamp at which to stop listing settlement transactions
+                e.g. 2016-09-24T00:00:05.000Z, 2016-09-21
 
-        Parameters
-        ----------
-        page: int
-            Specify exactly what page you want to retrieve.
-            If not specify we use a default value of 1.
-        pagination:int
-            Specify how many records you want to retrieve per page.
-            If not specify we use a default value of 50.
-        start_date: Optional[str]
-            A timestamp from which to start listing page
-            e.g. 2016-09-24T00:00:05.000Z, 2016-09-21
-        end_date: Optional[str]
-            A timestamp at which to stop listing page
-            e.g. 2016-09-24T00:00:05.000Z, 2016-09-21
-
-        Returns
-        -------
-        Response
+        Returns:
             A named tuple containing the response gotten from paystack's server.
         """
 
-        url = self._url("/page?perPage=" + str(pagination))
+        url = self._parse_url(f"/settlement/{id}/transactions?perPage={pagination}")
         query_params = [
             ("page", page),
             ("start_date", start_date),
             ("end_date", end_date),
         ]
         url = append_query_params(query_params, url)
-        return self._handle_request("GET", url)
+        return self._handle_request(HTTPMethod.GET, url)
 
-    def get_page(self, id_or_slug: str):
-        """Get details of a payment page on your integration.
 
-        Parameters
-        ----------
-        id_or_slug: str
-            The page ``ID`` or ``slug`` you want to fetch
-
-        Returns
-        -------
-        Response
-            A named tuple containing the response gotten from paystack's server.
-        """
+class AsyncSettlement(BaseAsyncAPI):
+    """Provides a wrapper for paystack Settlement API
 
-        url = self._url(f"/page/{id_or_slug}")
-        return self._handle_request("GET", url)
+    The Settlements API allows you gain insights into payouts made by Paystack to your bank account.
+    https://paystack.com/docs/api/#settlement
+    """
 
-    def update(
+    async def get_settlements(
         self,
-        id_or_slug: str,
-        name: str,
-        description: str,
-        amount: int,
-        active: Optional[bool] = None,
+        page: int = 1,
+        pagination: int = 50,
+        start_date: Optional[str] = None,
+        end_date: Optional[str] = None,
+        subaccount: Optional[str] = None,
     ) -> Response:
-        """Get details of a payment page on your integration.
+        """Fetch settlements made to your settlement accounts.
 
-        Parameters
-        ----------
-        id_or_slug: str
-            The page ``ID`` or ``slug`` you want to fetch
-        name: str
-            Name of page
-        description: str
-            A description for the page
-        amount: int
-            Default amount you want to accept using this page.
-            If none is set, customer is free to provide any amount
-            of their choice. The latter scenario is useful for
-            accepting donations
-        active: Optional[bool]
-            Set to ``False`` to deactivate page url
-
-        Returns
-        -------
-        Response
+        Args:
+            page: Specifies exactly what page you want to retrieve.
+                If not specified we use a default value of 1.
+            pagination: Specifies how many records you want to retrieve per page.
+                If not specified we use a default value of 50.
+            start_date: A timestamp from which to start listing settlements e.g. 2016-09-24T00:00:05.000Z, 2016-09-21
+            end_date: A timestamp at which to stop listing settlements e.g. 2016-09-24T00:00:05.000Z, 2016-09-21
+            subaccount: Provide a subaccount ID to export only settlements for that subaccount.
+                Set to ``none`` to export only transactions for the account.
+
+        Returns:
             A named tuple containing the response gotten from paystack's server.
         """
 
-        url = self._url(f"/page/{id_or_slug}")
-        payload = {
-            "name": name,
-            "description": description,
-        }
-        optional_params = [
-            ("amount", amount),
-            ("active", active),
+        url = self._parse_url(f"/settlement?perPage={pagination}")
+        query_params = [
+            ("subaccount", subaccount),
+            ("page", page),
+            ("start_date", start_date),
+            ("end_date", end_date),
         ]
-        payload = add_to_payload(optional_params, payload)
-        return self._handle_request("PUT", url, payload)
-
-    def check_slug_available(self, slug: str) -> Response:
-        """Check the availability of a slug for a payment page.
-
-        Parameters
-        ----------
-        slug: str
-            URL slug to be confirmed
-
-        Returns
-        -------
-        Response
-            A named tuple containing the response gotten from paystack's server.
-        """
+        url = append_query_params(query_params, url)
+        return await self._handle_request(HTTPMethod.GET, url)
 
-        url = self._url(f"/page/check_slug_availability/{slug}")
-        return self._handle_request("GET", url)
+    async def get_settlement_transactions(
+        self,
+        id: str,
+        pagination: int = 50,
+        page: int = 1,
+        start_date: Optional[str] = None,
+        end_date: Optional[str] = None,
+    ) -> Response:
+        """Get the transactions that make up a particular settlement
 
-    def add_products(self, id: str, products: list[int]):
-        """Add products to a payment page
+        Args:
+            id: The settlement ID in which you want to fetch its transactions
+            pagination: Specifies how many records you want to retrieve per page. If not specified we
+                use a default value of 50.
+            page: Specifies exactly what page you want to retrieve. If not specified we use a default value of 1.
+            start_date: A timestamp from which to start listing settlement transactions
+                e.g. 2016-09-24T00:00:05.000Z, 2016-09-21
+            end_date: A timestamp at which to stop listing settlement transactions
+                e.g. 2016-09-24T00:00:05.000Z, 2016-09-21
 
-        Parameters
-        ----------
-        id: str
-            Id of the payment page
-        products: list[int]
-            Ids of all the products
-
-        Returns
-        -------
-        Response
+        Returns:
             A named tuple containing the response gotten from paystack's server.
         """
 
-        url = self._url(f"/page/{id}/product")
-        payload = {"product": products}
-        return self._handle_request("POST", url, payload)
+        url = self._parse_url(f"/settlement/{id}/transactions?perPage={pagination}")
+        query_params = [
+            ("page", page),
+            ("start_date", start_date),
+            ("end_date", end_date),
+        ]
+        url = append_query_params(query_params, url)
+        return await self._handle_request(HTTPMethod.GET, url)
```

### Comparing `pypaystack2-1.1.3/pypaystack2/api/transactions.py` & `pypaystack2-2.0.0/pypaystack2/api/transactions.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,101 +1,82 @@
-from typing import Any, Optional
+from typing import Optional
 
-from pypaystack2.baseapi import BaseAPI, Response
+from pypaystack2.baseapi import BaseAPI, BaseAsyncAPI
 from pypaystack2.errors import InvalidDataError
 from pypaystack2.utils import (
     Bearer,
     Channel,
     Currency,
     TransactionStatus,
     add_to_payload,
     append_query_params,
     validate_amount,
+    HTTPMethod,
+    Response,
 )
 
 
 class Transaction(BaseAPI):
     """Provides a wrapper for paystack Transactions API
 
-    The Transactions API allows you create and manage payments on your integration.
+    The Transactions API allows you to create and manage payments on your integration.
     https://paystack.com/docs/api/#transaction
     """
 
     def initialize(
         self,
         amount: int,
         email: str,
         currency: Optional[Currency] = None,
         reference: Optional[str] = None,
         callback_url: Optional[str] = None,
         plan: Optional[str] = None,
         invoice_limit: Optional[int] = None,
-        metadata: Optional[dict[str, Any]] = None,
+        metadata: Optional[dict] = None,
         channels: Optional[list[Channel]] = None,
         split_code: Optional[str] = None,
         subaccount: Optional[str] = None,
         transfer_charge: Optional[int] = None,
         bearer: Optional[Bearer] = None,
     ) -> Response:
         """Initialize a transaction from your backend
 
-        Parameters
-        ----------
-        amount: int
-            Amount should be in kobo if currency is ``Currency.NGN``, pesewas,
-            if currency is ``Currency.GHS``, and cents, if currency is ``Currency.ZAR``
-        email: str
-            Customer's email address
-        currency: Optional[Currency]
-            Any value from the ``Currency`` enum.
-        reference: Optional[str]
-            Unique transaction reference. Only ``-, ., =`` and alphanumeric characters allowed.
-        callback_url: Optional[str]
-            Fully qualified url, e.g. ``https://example.com/`` . Use this to override the callback url
-            provided on the dashboard for this transaction
-        plan: Optional[str]
-            If transaction is to create a subscription to a predefined plan, provide plan code here.
-            This would invalidate the value provided in ``amount``
-        invoice_limit: Optional[int]
-            Number of times to charge customer during subscription to plan
-        metadata: Optional[dict[str,Any]]
-            A dictionary of additional info. check out this link
-            for more information.
-            https://paystack.com/docs/payments/metadata
-        channels: Optional[list[Channel]]
-            A list of ``Channel`` enum values to control what channels you want to make available
-            to the user to make a payment with
-        split_code: Optional[str]
-            The split code of the transaction split.
-            e.g. SPL_98WF13Eb3w
-        subaccount: Optional[str]
-            The code for the subaccount that owns the payment.
-            e.g. ACCT_8f4s1eq7ml6rlzj
-        transfer_charge: Optional[int]
-            An amount used to override the split configuration for a single split payment. If set,
-            the amount specified goes to the main account regardless of the split configuration.
-        bearer: Optional[Bearer]
-            Any value from the ``Bearer`` enum. Who bears Paystack charges?
-
-        Returns
-        -------
-        Response
-            A named tuple containing the response gotten from paystack's server.
-
-        Raises
-        ------
-        InvalidDataError
-            When email is not provided.
+        Args:
+            amount: Amount should be in kobo if currency is ``Currency.NGN``, pesewas,
+                if currency is ``Currency.GHS``, and cents, if currency is ``Currency.ZAR``
+            email: Customer's email address
+            currency: Any value from the ``Currency`` enum.
+            reference: Unique transaction reference. Only ``-, ., =`` and alphanumeric characters allowed.
+            callback_url: Fully qualified url, e.g. ``https://example.com/`` . Use this to override the callback url
+                provided on the dashboard for this transaction
+            plan: If transaction is to create a subscription to a predefined plan, provide plan code here.
+                This would invalidate the value provided in ``amount``
+            invoice_limit: Number of times to charge customer during subscription to plan
+            metadata: A dictionary of additional info. check out this link
+                for more information. https://paystack.com/docs/payments/metadata
+            channels: A list of ``Channel`` enum values to control what channels you want to make available
+                to the user to make a payment with
+            split_code: The split code of the transaction split. e.g. SPL_98WF13Eb3w
+            subaccount: The code for the subaccount that owns the payment. e.g. ACCT_8f4s1eq7ml6rlzj
+            transfer_charge: An amount used to override the split configuration for a single split payment. If set,
+                the amount specified goes to the main account regardless of the split configuration.
+            bearer: Any value from the ``Bearer`` enum. Who bears Paystack charges?
+
+        Returns:
+            A named tuple containing the response gotten from paystack's server.
+
+        Raises:
+            InvalidDataError: When email is not provided.
         """
         amount = validate_amount(amount)
 
         if not email:
             raise InvalidDataError("Customer's Email is required for initialization")
 
-        url = self._url("/transaction/initialize")
+        url = self._parse_url("/transaction/initialize")
         payload = {
             "email": email,
             "amount": amount,
         }
 
         optional_params = [
             ("currency", currency),
@@ -108,176 +89,143 @@
             ("split_code", split_code),
             ("subaccount", subaccount),
             ("transfer_charge", transfer_charge),
             ("bearer", bearer),
         ]
         payload = add_to_payload(optional_params, payload)
 
-        return self._handle_request("POST", url, payload)
+        return self._handle_request(HTTPMethod.POST, url, payload)
 
     def verify(self, reference: str) -> Response:
         """Confirm the status of a transaction
 
-        Parameters
-        ----------
-        reference: str
-            The transaction reference used to intiate the transaction
-
-        Returns
-        -------
-        Response
+        Args:
+            reference: The transaction reference used to intiate the transaction
+
+        Returns:
             A named tuple containing the response gotten from paystack's server.
         """
 
         reference = str(reference)
-        url = self._url(f"/transaction/verify/{reference}")
-        return self._handle_request("GET", url)
+        url = self._parse_url(f"/transaction/verify/{reference}")
+        return self._handle_request(HTTPMethod.GET, url)
 
     def get_transactions(
         self,
         customer: Optional[int] = None,
         start_date: Optional[str] = None,
         end_date: Optional[str] = None,
         status: Optional[TransactionStatus] = None,
         page: Optional[int] = None,
         amount: Optional[int] = None,
-        pagination=50,
+        pagination: int = 50,
     ) -> Response:
         """Fetch transactions carried out on your integration.
 
-        Parameters
-        ----------
-        customer: Optional[int]
-            Specify an ID for the customer whose transactions you want to retrieve
-        start_date: Optional[str]
-            A timestamp from which to start listing transaction
-            e.g. 2016-09-24T00:00:05.000Z, 2016-09-21
-        end_date: Optional[str]
-            A timestamp at which to stop listing transaction
-            e.g. 2016-09-24T00:00:05.000Z, 2016-09-21
-        status: Optional[TransactionStatus]
-            Filter transactions by status. any value from the
-            ``TransactionStatus`` enum
-        page: Optional[int]
-            Specify exactly what page you want to retrieve.
-            If not specify we use a default value of 1.
-        amount: Optional[int]
-            Filter transactions by amount. Specify the amount (in kobo if currency is
-            ``Currency.NGN``, pesewas, if currency is ``Currency.GHS``, and cents, if
-            currency is ``Currency.ZAR``)
-        pagination: int
-            Specify how many records you want to retrieve per page. If not specify we
-            use a default value of 50.
-
-        Returns
-        -------
-        Response
+        Args:
+            customer: Specify an ID for the customer whose transactions you want to retrieve
+            start_date: A timestamp from which to start listing transaction e.g. 2016-09-24T00:00:05.000Z, 2016-09-21
+            end_date: A timestamp at which to stop listing transaction e.g. 2016-09-24T00:00:05.000Z, 2016-09-21
+            status: Filter transactions by status. any value from the ``TransactionStatus`` enum
+            page: Specify exactly what page you want to retrieve.
+                If not specified, we use a default value of 1.
+            amount: Optional[int]
+                Filter transactions by amount. Specify the amount (in kobo if currency is
+                ``Currency.NGN``, pesewas, if currency is ``Currency.GHS``, and cents, if
+                currency is ``Currency.ZAR``)
+            pagination: Specifies how many records you want to retrieve per page. If not specified, we
+                use a default value of 50.
+
+        Returns:
             A named tuple containing the response gotten from paystack's server.
         """
 
-        url = self._url(f"/transaction/?perPage={pagination}")
+        url = self._parse_url(f"/transaction/?perPage={pagination}")
         query_params = [
             ("page", page),
             ("customer", customer),
             ("status", status),
             ("from", start_date),
             ("to", end_date),
             ("amount", amount),
         ]
         url = append_query_params(query_params, url)
 
-        return self._handle_request("GET", url)
+        return self._handle_request(HTTPMethod.GET, url)
 
     def get_transaction(self, id: str) -> Response:
         """Get details of a transaction carried out on your integration.
 
-        Parameters
-        ----------
-        id: str
-            An ID for the transaction to fetch
+        Args:
+            id: An ID for the transaction to fetch
 
-        Returns
-        -------
-        Response
+        Returns:
             A named tuple containing the response gotten from paystack's server.
         """
 
-        url = self._url(f"/transaction/{id}/")
-        return self._handle_request("GET", url)
+        url = self._parse_url(f"/transaction/{id}/")
+        return self._handle_request(HTTPMethod.GET, url)
 
     def charge(
         self,
         amount: int,
         email: str,
         auth_code: str,
         reference: Optional[str] = None,
         currency: Optional[Currency] = None,
-        metadata: Optional[dict[str, Any]] = None,
+        metadata: Optional[dict] = None,
         channels: Optional[list[Channel]] = None,
         subaccount: Optional[str] = None,
         transaction_charge: Optional[int] = None,
         bearer: Optional[Bearer] = None,
         queue: bool = False,
     ) -> Response:
         """
         All authorizations marked as reusable can be charged with this
         endpoint whenever you need to receive payments.
 
-        Parameters
-        ----------
-        amount: int
-        email: str
-            Customer's email address
-        auth_code: str
-            Valid authorization code to charge
-        reference: Optional[str]
-            Unique transaction reference. Only ``-, ., =`` and alphanumeric
-            characters allowed.
-        currency: Optional[Currency]
-            Currency in which amount should be charged. Any value from the
-            ``Currency`` enum.
-        metadata: Optional[dict[str,Any]]
-            Add a custom_fields attribute which has an array of objects if
-            you would like the fields to be added to your transaction when
-            displayed on the dashboard.
-            Sample: ``{"custom_fields":[{"display_name":"Cart ID",
-            "variable_name": "cart_id","value": "8393"}]}``
-        channels: Optional[list[Channel]]
-            A list of ``Channel`` enum values to control what channels you want to make available
-            to the user to make a payment with
-        subaccount: Optional[str]
-            The code for the subaccount that owns the payment. e.g. ACCT_8f4s1eq7ml6rlzj
-        transaction_charge: Optional[int]
-            A flat fee to charge the subaccount for this transaction (in kobo if currency is NGN,
-            pesewas, if currency is GHS, and cents, if currency is ZAR). This overrides the split
-            percentage set when the subaccount was created. Ideally, you will need to use this if
-            you are splitting in flat rates (since subaccount creation only allows for percentage split).
-            e.g. 7000 for a 70 naira
-        bearer: Optional[Bearer]
-            Who bears Paystack charges? any value from the ``Beaer`` enum
-        queue: bool
-            If you are making a scheduled charge call, it is a good idea to queue them so the processing
-            system does not get overloaded causing transaction processing errors. Set ``queue=True`` to
-            take advantage of our queued charging.
-
-        Returns
-        -------
-        Response
+        Args:
+            amount: amount to charge.
+            email: Customer's email address
+            auth_code: Valid authorization code to charge
+            reference: Unique transaction reference. Only ``-, ., =`` and alphanumeric
+                characters allowed.
+            currency: Currency in which amount should be charged. Any value from the
+                ``Currency`` enum.
+            metadata: Add a custom_fields attribute which has an array of objects if
+                you would like the fields to be added to your transaction when
+                displayed on the dashboard.
+                Sample: ``{"custom_fields":[{"display_name":"Cart ID",
+                "variable_name": "cart_id","value": "8393"}]}``
+            channels: A list of ``Channel`` enum values to control what channels you want to make available
+                to the user to make a payment with
+            subaccount: The code for the subaccount that owns the payment. e.g. ACCT_8f4s1eq7ml6rlzj
+            transaction_charge: A flat fee to charge the subaccount for this transaction (in kobo if currency is NGN,
+                pesewas, if currency is GHS, and cents, if currency is ZAR). This overrides the split
+                percentage set when the subaccount was created. Ideally, you will need to use this if
+                you are splitting in flat rates (since subaccount creation only allows for percentage split).
+                e.g., 7000 for a 70 naira
+            bearer: Who bears Paystack charges? any value from the ``Beaer`` enum
+            queue: If you are making a scheduled charge call, it is a good idea to queue them so the processing
+                system does not get overloaded causing transaction processing errors. Set ``queue=True`` to
+                take advantage of our queued charging.
+
+        Returns:
             A named tuple containing the response gotten from paystack's server.
         """
 
         amount = validate_amount(amount)
 
         if not email:
             raise InvalidDataError("Customer's Email is required to charge")
 
         if not auth_code:
             raise InvalidDataError("Customer's Auth code is required to charge")
 
-        url = self._url("/transaction/charge_authorization")
+        url = self._parse_url("/transaction/charge_authorization")
         payload = {
             "authorization_code": auth_code,
             "email": email,
             "amount": amount,
         }
         optional_params = [
             ("reference", reference),
@@ -287,353 +235,535 @@
             ("subaccount", subaccount),
             ("transaction_charge", transaction_charge),
             ("bearer", bearer),
             ("queue", queue),
         ]
         payload = add_to_payload(optional_params, payload)
 
-        return self._handle_request("POST", url, payload)
-
-    def check_authorization(
-        self,
-        amount: int,
-        email: str,
-        auth_code: str,
-        currency: Optional[Currency] = None,
-    ) -> Response:
-        """All Mastercard and Visa authorizations can be checked with
-        this endpoint to know if they have funds for the payment you seek.
-
-        This method should be used when you do not know the exact amount
-        to charge a card when rendering a service. It should be used to
-        check if a card has enough funds based on a maximum range value.
-
-        It is well suited:
-            - Ride hailing services
-            - Logistics services
-
-        You shouldn't use this method to check a card for sufficient
-        funds if you are going to charge the user immediately. This is
-        because we hold funds when this endpoint is called which can lead
-        to an insufficient funds error.
-
-        Parameters
-        ----------
-        amount: int
-            Amount should be in kobo if currency is ``Currency.NGN``, pesewas, if currency is
-            ``Currency.GHS``, and cents, if currency is ``Currency.ZAR``
-        email: str
-            Customer's email address
-        auth_code: str
-            Valid authorization code to charge
-        currency: Optional[Currency]
-            Currency in which amount should be charged. Any value from the ``Currency`` enum.
-
-        Returns
-        -------
-        Response
-            A named tuple containing the response gotten from paystack's server.
-
-        Note
-        ----
-        This feature is only available to businesses in Nigeria.
-        """
-        amount = validate_amount(amount)
-
-        if not email:
-            raise InvalidDataError("Customer's Email is required to charge")
-
-        if not auth_code:
-            raise InvalidDataError("Customer's Auth code is required to charge")
-
-        url = self._url("/transaction/check_authorization")
-        payload = {
-            "authorization_code": auth_code,
-            "email": email,
-            "amount": amount,
-        }
-        optional_params = [
-            ("currency", currency),
-        ]
-        payload = add_to_payload(optional_params, payload)
-
-        return self._handle_request("POST", url, payload)
+        return self._handle_request(HTTPMethod.POST, url, payload)
 
     def get_timeline(self, id_or_ref: str) -> Response:
         """View the timeline of a transaction
 
-        Parameters
-        ----------
-        id_or_ref: str
-            The ID or the reference of the transaction
+        Args:
+            id_or_ref: The ID or the reference of the transaction
 
-        Returns
-        -------
-        Response
+        Returns:
             A named tuple containing the response gotten from paystack's server.
         """
 
-        url = self._url(f"/transaction/timeline/{id_or_ref}")
-        return self._handle_request("GET", url)
+        url = self._parse_url(f"/transaction/timeline/{id_or_ref}")
+        return self._handle_request(HTTPMethod.GET, url)
 
     def totals(
         self,
         page: Optional[int] = None,
         start_date: Optional[str] = None,
         end_date: Optional[str] = None,
-        pagination=50,
-    ):
+        pagination: int = 50,
+    ) -> Response:
         """Total amount received on your account
 
-        Parameters
-        ----------
-        page: Optional[int]
-            Specify exactly what page you want to retrieve.
-            If not specify we use a default value of 1.
-        start_date: Optional[str]
-            A timestamp from which to start listing transaction
-            e.g. 2016-09-24T00:00:05.000Z, 2016-09-21
-        end_date: Optional[str]
-            A timestamp at which to stop listing transaction
-            e.g. 2016-09-24T00:00:05.000Z, 2016-09-21
-        pagination: int
-            Specify how many records you want to retrieve per page.
-            If not specify we use a default value of 50.
-
-        Returns
-        -------
-        Response
+        Args:
+            page: Specifies exactly what page you want to retrieve.
+                If not specified, we use a default value of 1.
+            start_date: A timestamp from which to start listing transaction e.g. 2016-09-24T00:00:05.000Z, 2016-09-21
+            end_date: A timestamp at which to stop listing transaction e.g. 2016-09-24T00:00:05.000Z, 2016-09-21
+            pagination: Specifies how many records you want to retrieve per page.
+                If not specified, we use a default value of 50.
+
+        Returns:
             A named tuple containing the response gotten from paystack's server.
         """
 
-        url = self._url(f"/transaction/totals/?perPage={pagination}")
-        url = url + f"&page={page}" if page else url
-        url = url + f"&from={start_date}" if start_date else url
-        url = url + f"&page={end_date}" if end_date else url
-        return self._handle_request("GET", url)
+        url = self._parse_url(f"/transaction/totals/?perPage={pagination}")
+        query_params = [
+            ("page", page),
+            ("from", start_date),
+            ("to", end_date),
+        ]
+        url = append_query_params(query_params, url)
+        return self._handle_request(HTTPMethod.GET, url)
 
     def export(
         self,
         page: Optional[int] = None,
         start_date: Optional[str] = None,
         end_date: Optional[str] = None,
         customer: Optional[int] = None,
         status: Optional[TransactionStatus] = None,
         currency: Optional[Currency] = None,
         amount: Optional[int] = None,
         settled: Optional[bool] = None,
         settlement: Optional[int] = None,
         payment_page: Optional[int] = None,
-        pagination=50,
+        pagination: int = 50,
     ) -> Response:
         """Fetch transactions carried out on your integration.
 
-        Parameters
-        ----------
-        page: Optional[int]
-            Specify exactly what page you want to retrieve.
-            If not specify we use a default value of 1.
-        start_date: Optional[str]
-            A timestamp from which to start listing transaction
-            e.g. 2016-09-24T00:00:05.000Z, 2016-09-21
-        end_date: Optional[str]
-            A timestamp at which to stop listing transaction
-            e.g. 2016-09-24T00:00:05.000Z, 2016-09-21
-        customer: Optional[int]
-            Specify an ID for the customer whose transactions you
-            want to retrieve
-        status: Optional[TransactionStatus]
-            Filter transactions by status. Any value from the
-            ``TransactionStatus`` enum
-        currency: Optional[Currency]
-            Specify the transaction currency to export. Any value
-            from the ``Currency`` enum
-        amount: Optional[int]
-            Filter transactions by amount. Specify the amount, in
-            kobo if currency is ``Currency.NGN``, pesewas, if currency
-            is ``Currency.GHS``, and cents, if currency is ``Currency.ZAR``
-        settled: Optional[bool]
-            Set to ``True`` to export only settled transactions. ``False`` for
-            pending transactions. Leave undefined to export all transactions
-        settlement: Optional[int]
-            An ID for the settlement whose transactions we should export
-        payment_page: Optional[int]
-            Specify a payment page's id to export only transactions conducted on said page
-        pagination: int
-            Specify how many records you want to retrieve per page.
-            If not specify we use a default value of 50.
-
-        Returns
-        -------
-        Response
+        Args:
+            page: Specifies exactly what page you want to retrieve.
+                If not specified, we use a default value of 1.
+            start_date: A timestamp from which to start listing transaction e.g. 2016-09-24T00:00:05.000Z, 2016-09-21
+            end_date: A timestamp at which to stop listing transaction e.g. 2016-09-24T00:00:05.000Z, 2016-09-21
+            customer: Specify an ID for the customer whose transactions you want to retrieve
+            status: Filter transactions by status. Any value from the ``TransactionStatus`` enum
+            currency: Specify the transaction currency to export. Any value from the ``Currency`` enum
+            amount: Filter transactions by amount. Specify the amount, in
+                kobo if currency is ``Currency.NGN``, pesewas, if currency
+                is ``Currency.GHS``, and cents, if currency is ``Currency.ZAR``
+            settled: Set to ``True`` to export only settled transactions. ``False`` for
+                pending transactions. Leave undefined to export all transaction
+            settlement: An ID for the settlement whose transactions we should export
+            payment_page: Optional[int]
+                Specify a payment page's id to export only transactions conducted on said page
+            pagination: int
+                Specifies how many records you want to retrieve per page.
+                If not specified, we use a default value of 50.
+
+        Returns:
             A named tuple containing the response gotten from paystack's server.
         """
 
         if amount:
             amount = validate_amount(amount)
-        url = self._url(f"/transaction/export/?perPage={pagination}")
+        url = self._parse_url(f"/transaction/export/?perPage={pagination}")
         query_params = [
             ("page", page),
             ("from", start_date),
             ("to", end_date),
             ("customer", customer),
             ("status", status),
             ("currency", currency),
             ("settled", settled),
             ("settlement", settlement),
             ("payment_page", payment_page),
         ]
         url = append_query_params(query_params, url)
-        return self._handle_request("GET", url)
+        return self._handle_request(HTTPMethod.GET, url)
 
     def partial_debit(
         self,
         auth_code: str,
         currency: Currency,
         amount: int,
         email: str,
         reference: Optional[str] = None,
         at_least: Optional[int] = None,
-    ):
+    ) -> Response:
         """Retrieve part of a payment from a customer
 
-        Parameters
-        ----------
-        auth_code: str
-            Authorization Code
-        currency: Currency
-            Specify the currency you want to debit. Any value
-            from the ``Currency`` enum.
-        amount: int
-            Amount should be in kobo if currency is ``Currency.NGN``, pesewas,
-            if currency is ``Currency.GHS``, and cents, if currency is ``Currency.ZAR``
-        email: str
-            Customer's email address (attached to the authorization code)
-        reference: Optional[str]
-            Unique transaction reference. Only `-, ., =`
-             and alphanumeric characters allowed.
-        at_least: Optional[int]
-            Minimum amount to charge
-
-        Returns
-        -------
-        Response
-            A named tuple containing the response gotten from paystack's server.
-
-        Raises
-        ------
-        InvalidDataError
-            - When Customer's email is not provided.
-            - When Customer's auth code is not provided.
+        Args:
+            auth_code: Authorization Code
+            currency: Specify the currency you want to debit. Any value
+                from the ``Currency`` enum.
+            amount: Amount should be in kobo if currency is ``Currency.NGN``, pesewas,
+                if currency is ``Currency.GHS``, and cents, if currency is ``Currency.ZAR``
+            email: Customer's email address (attached to the authorization code)
+            reference: Unique transaction reference. Only `-, ., =`
+                 and alphanumeric characters allowed.
+            at_least: Minimum amount to charge
+
+        Returns:
+            A named tuple containing the response gotten from paystack's server.
+
+        Raises:
+            InvalidDataError: When Customer's email is not provided. When Customer's auth code is not provided.
         """
         amount = validate_amount(amount)
         if at_least:
             at_least = validate_amount(at_least)
 
         if not email:
             raise InvalidDataError("Customer's Email is required to charge")
 
         if not auth_code:
             raise InvalidDataError("Customer's Auth code is required to charge")
 
-        url = self._url("/transaction/partial_debit")
+        url = self._parse_url("/transaction/partial_debit")
         payload = {
             "authorization_code": auth_code,
             "currency": currency,
             "amount": amount,
             "email": email,
         }
         optional_params = [("reference", reference), ("at_least", at_least)]
         payload = add_to_payload(optional_params, payload)
 
-        return self._handle_request("POST", url, payload)
+        return self._handle_request(HTTPMethod.POST, url, payload)
 
-    def get_transfer_banks(self):
-        # TODO: Deprecate. it's available in Miscellaneous API
-        """Fetch transfer banks
 
-        Returns
-        -------
-        Response
+class AsyncTransaction(BaseAsyncAPI):
+    """Provides a wrapper for paystack Transactions API
+
+    The Transactions API allows you to create and manage payments on your integration.
+    https://paystack.com/docs/api/#transaction
+    """
+
+    async def initialize(
+        self,
+        amount: int,
+        email: str,
+        currency: Optional[Currency] = None,
+        reference: Optional[str] = None,
+        callback_url: Optional[str] = None,
+        plan: Optional[str] = None,
+        invoice_limit: Optional[int] = None,
+        metadata: Optional[dict] = None,
+        channels: Optional[list[Channel]] = None,
+        split_code: Optional[str] = None,
+        subaccount: Optional[str] = None,
+        transfer_charge: Optional[int] = None,
+        bearer: Optional[Bearer] = None,
+    ) -> Response:
+        """Initialize a transaction from your backend
+
+        Args:
+            amount: Amount should be in kobo if currency is ``Currency.NGN``, pesewas,
+                if currency is ``Currency.GHS``, and cents, if currency is ``Currency.ZAR``
+            email: Customer's email address
+            currency: Any value from the ``Currency`` enum.
+            reference: Unique transaction reference. Only ``-, ., =`` and alphanumeric characters allowed.
+            callback_url: Fully qualified url, e.g. ``https://example.com/`` . Use this to override the callback url
+                provided on the dashboard for this transaction
+            plan: If transaction is to create a subscription to a predefined plan, provide plan code here.
+                This would invalidate the value provided in ``amount``
+            invoice_limit: Number of times to charge customer during subscription to plan
+            metadata: A dictionary of additional info. check out this link
+                for more information. https://paystack.com/docs/payments/metadata
+            channels: A list of ``Channel`` enum values to control what channels you want to make available
+                to the user to make a payment with
+            split_code: The split code of the transaction split. e.g. SPL_98WF13Eb3w
+            subaccount: The code for the subaccount that owns the payment. e.g. ACCT_8f4s1eq7ml6rlzj
+            transfer_charge: An amount used to override the split configuration for a single split payment. If set,
+                the amount specified goes to the main account regardless of the split configuration.
+            bearer: Any value from the ``Bearer`` enum. Who bears Paystack charges?
+
+        Returns:
             A named tuple containing the response gotten from paystack's server.
 
-        Note
-        ----
-        Deprecation Notice
-            it's available in Miscellaneous API wrapper. may be removed in future release
+        Raises:
+            InvalidDataError: When email is not provided.
+        """
+        amount = validate_amount(amount)
+
+        if not email:
+            raise InvalidDataError("Customer's Email is required for initialization")
+
+        url = self._parse_url("/transaction/initialize")
+        payload = {
+            "email": email,
+            "amount": amount,
+        }
+
+        optional_params = [
+            ("currency", currency),
+            ("reference", reference),
+            ("callback_url", callback_url),
+            ("plan", plan),
+            ("invoice_limit", invoice_limit),
+            ("metadata", metadata),
+            ("channels", channels),
+            ("split_code", split_code),
+            ("subaccount", subaccount),
+            ("transfer_charge", transfer_charge),
+            ("bearer", bearer),
+        ]
+        payload = add_to_payload(optional_params, payload)
+
+        return await self._handle_request(HTTPMethod.POST, url, payload)
+
+    async def verify(self, reference: str) -> Response:
+        """Confirm the status of a transaction
+
+        Args:
+            reference: The transaction reference used to intiate the transaction
+
+        Returns:
+            A named tuple containing the response gotten from paystack's server.
         """
 
-        url = self._url("/bank")
-        return self._handle_request("GET", url)
+        reference = str(reference)
+        url = self._parse_url(f"/transaction/verify/{reference}")
+        return await self._handle_request(HTTPMethod.GET, url)
 
-    def create_transfer_customer(
-        self, bank_code: str, account_number: int, account_name: str
+    async def get_transactions(
+        self,
+        customer: Optional[int] = None,
+        start_date: Optional[str] = None,
+        end_date: Optional[str] = None,
+        status: Optional[TransactionStatus] = None,
+        page: Optional[int] = None,
+        amount: Optional[int] = None,
+        pagination: int = 50,
     ) -> Response:
-        # TODO: Deprecate. it's available in TransferReceipt API
-        """Create a transfer customer
+        """Fetch transactions carried out on your integration.
 
-        Parameters
-        ----------
-        bank_code
-        account_number
-        account_name
+        Args:
+            customer: Specify an ID for the customer whose transactions you want to retrieve
+            start_date: A timestamp from which to start listing transaction e.g. 2016-09-24T00:00:05.000Z, 2016-09-21
+            end_date: A timestamp at which to stop listing transaction e.g. 2016-09-24T00:00:05.000Z, 2016-09-21
+            status: Filter transactions by status. any value from the ``TransactionStatus`` enum
+            page: Specify exactly what page you want to retrieve.
+                If not specified, we use a default value of 1.
+            amount: Optional[int]
+                Filter transactions by amount. Specify the amount (in kobo if currency is
+                ``Currency.NGN``, pesewas, if currency is ``Currency.GHS``, and cents, if
+                currency is ``Currency.ZAR``)
+            pagination: Specifies how many records you want to retrieve per page. If not specified, we
+                use a default value of 50.
 
-        Returns
-        -------
-        Response
+        Returns:
             A named tuple containing the response gotten from paystack's server.
+        """
 
-        Note
-        -----
-        Deprecation Notice
-            it's available in TransferReceipt API wrapper. may be removed in future release
+        url = self._parse_url(f"/transaction/?perPage={pagination}")
+        query_params = [
+            ("page", page),
+            ("customer", customer),
+            ("status", status),
+            ("from", start_date),
+            ("to", end_date),
+            ("amount", amount),
+        ]
+        url = append_query_params(query_params, url)
+
+        return await self._handle_request(HTTPMethod.GET, url)
+
+    async def get_transaction(self, id: str) -> Response:
+        """Get details of a transaction carried out on your integration.
+
+        Args:
+            id: An ID for the transaction to fetch
+
+        Returns:
+            A named tuple containing the response gotten from paystack's server.
         """
-        url = self._url("/transferrecipient")
+
+        url = self._parse_url(f"/transaction/{id}/")
+        return await self._handle_request(HTTPMethod.GET, url)
+
+    async def charge(
+        self,
+        amount: int,
+        email: str,
+        auth_code: str,
+        reference: Optional[str] = None,
+        currency: Optional[Currency] = None,
+        metadata: Optional[dict] = None,
+        channels: Optional[list[Channel]] = None,
+        subaccount: Optional[str] = None,
+        transaction_charge: Optional[int] = None,
+        bearer: Optional[Bearer] = None,
+        queue: bool = False,
+    ) -> Response:
+        """
+        All authorizations marked as reusable can be charged with this
+        endpoint whenever you need to receive payments.
+
+        Args:
+            amount: amount to charge.
+            email: Customer's email address
+            auth_code: Valid authorization code to charge
+            reference: Unique transaction reference. Only ``-, ., =`` and alphanumeric
+                characters allowed.
+            currency: Currency in which amount should be charged. Any value from the
+                ``Currency`` enum.
+            metadata: Add a custom_fields attribute which has an array of objects if
+                you would like the fields to be added to your transaction when
+                displayed on the dashboard.
+                Sample: ``{"custom_fields":[{"display_name":"Cart ID",
+                "variable_name": "cart_id","value": "8393"}]}``
+            channels: A list of ``Channel`` enum values to control what channels you want to make available
+                to the user to make a payment with
+            subaccount: The code for the subaccount that owns the payment. e.g. ACCT_8f4s1eq7ml6rlzj
+            transaction_charge: A flat fee to charge the subaccount for this transaction (in kobo if currency is NGN,
+                pesewas, if currency is GHS, and cents, if currency is ZAR). This overrides the split
+                percentage set when the subaccount was created. Ideally, you will need to use this if
+                you are splitting in flat rates (since subaccount creation only allows for percentage split).
+                e.g., 7000 for a 70 naira
+            bearer: Who bears Paystack charges? any value from the ``Beaer`` enum
+            queue: If you are making a scheduled charge call, it is a good idea to queue them so the processing
+                system does not get overloaded causing transaction processing errors. Set ``queue=True`` to
+                take advantage of our queued charging.
+
+        Returns:
+            A named tuple containing the response gotten from paystack's server.
+        """
+
+        amount = validate_amount(amount)
+
+        if not email:
+            raise InvalidDataError("Customer's Email is required to charge")
+
+        if not auth_code:
+            raise InvalidDataError("Customer's Auth code is required to charge")
+
+        url = self._parse_url("/transaction/charge_authorization")
         payload = {
-            "type": "nuban",
-            "currency": "NGN",
-            "bank_code": bank_code,
-            "account_number": account_number,
-            "name": account_name,
+            "authorization_code": auth_code,
+            "email": email,
+            "amount": amount,
         }
-        return self._handle_request("POST", url, payload)
+        optional_params = [
+            ("reference", reference),
+            ("currency", currency),
+            ("metadata", metadata),
+            ("channels", channels),
+            ("subaccount", subaccount),
+            ("transaction_charge", transaction_charge),
+            ("bearer", bearer),
+            ("queue", queue),
+        ]
+        payload = add_to_payload(optional_params, payload)
+
+        return await self._handle_request(HTTPMethod.POST, url, payload)
+
+    async def get_timeline(self, id_or_ref: str) -> Response:
+        """View the timeline of a transaction
+
+        Args:
+            id_or_ref: The ID or the reference of the transaction
+
+        Returns:
+            A named tuple containing the response gotten from paystack's server.
+        """
+
+        url = self._parse_url(f"/transaction/timeline/{id_or_ref}")
+        return await self._handle_request(HTTPMethod.GET, url)
+
+    async def totals(
+        self,
+        page: Optional[int] = None,
+        start_date: Optional[str] = None,
+        end_date: Optional[str] = None,
+        pagination: int = 50,
+    ) -> Response:
+        """Total amount received on your account
+
+        Args:
+            page: Specifies exactly what page you want to retrieve.
+                If not specified, we use a default value of 1.
+            start_date: A timestamp from which to start listing transaction e.g. 2016-09-24T00:00:05.000Z, 2016-09-21
+            end_date: A timestamp at which to stop listing transaction e.g. 2016-09-24T00:00:05.000Z, 2016-09-21
+            pagination: Specifies how many records you want to retrieve per page.
+                If not specified, we use a default value of 50.
+
+        Returns:
+            A named tuple containing the response gotten from paystack's server.
+        """
 
-    def transfer(
+        url = self._parse_url(f"/transaction/totals/?perPage={pagination}")
+        query_params = [
+            ("page", page),
+            ("from", start_date),
+            ("to", end_date),
+        ]
+        url = append_query_params(query_params, url)
+        return await self._handle_request(HTTPMethod.GET, url)
+
+    async def export(
+        self,
+        page: Optional[int] = None,
+        start_date: Optional[str] = None,
+        end_date: Optional[str] = None,
+        customer: Optional[int] = None,
+        status: Optional[TransactionStatus] = None,
+        currency: Optional[Currency] = None,
+        amount: Optional[int] = None,
+        settled: Optional[bool] = None,
+        settlement: Optional[int] = None,
+        payment_page: Optional[int] = None,
+        pagination: int = 50,
+    ) -> Response:
+        """Fetch transactions carried out on your integration.
+
+        Args:
+            page: Specifies exactly what page you want to retrieve.
+                If not specified, we use a default value of 1.
+            start_date: A timestamp from which to start listing transaction e.g. 2016-09-24T00:00:05.000Z, 2016-09-21
+            end_date: A timestamp at which to stop listing transaction e.g. 2016-09-24T00:00:05.000Z, 2016-09-21
+            customer: Specify an ID for the customer whose transactions you want to retrieve
+            status: Filter transactions by status. Any value from the ``TransactionStatus`` enum
+            currency: Specify the transaction currency to export. Any value from the ``Currency`` enum
+            amount: Filter transactions by amount. Specify the amount, in
+                kobo if currency is ``Currency.NGN``, pesewas, if currency
+                is ``Currency.GHS``, and cents, if currency is ``Currency.ZAR``
+            settled: Set to ``True`` to export only settled transactions. ``False`` for
+                pending transactions. Leave undefined to export all transaction
+            settlement: An ID for the settlement whose transactions we should export
+            payment_page: Optional[int]
+                Specify a payment page's id to export only transactions conducted on said page
+            pagination: int
+                Specifies how many records you want to retrieve per page.
+                If not specified, we use a default value of 50.
+
+        Returns:
+            A named tuple containing the response gotten from paystack's server.
+        """
+
+        if amount:
+            amount = validate_amount(amount)
+        url = self._parse_url(f"/transaction/export/?perPage={pagination}")
+        query_params = [
+            ("page", page),
+            ("from", start_date),
+            ("to", end_date),
+            ("customer", customer),
+            ("status", status),
+            ("currency", currency),
+            ("settled", settled),
+            ("settlement", settlement),
+            ("payment_page", payment_page),
+        ]
+        url = append_query_params(query_params, url)
+        return await self._handle_request(HTTPMethod.GET, url)
+
+    async def partial_debit(
         self,
-        recipient_code: str,
+        auth_code: str,
+        currency: Currency,
         amount: int,
-        reason: str,
+        email: str,
         reference: Optional[str] = None,
+        at_least: Optional[int] = None,
     ) -> Response:
-        # TODO: Deprecate. it's available in Transfer API
-        """Initiates transfer to a customer
+        """Retrieve part of a payment from a customer
 
-        Parameters
-        ----------
-        recipient_code
-        amount
-        reason
-        reference
-
-        Returns
-        -------
-        Response
-            A named tuple containing the response gotten from paystack's server.
-
-        Note
-        ----
-        Deprecation Notice
-            it's available in Transfer API wrapper. may be removed in future release
+        Args:
+            auth_code: Authorization Code
+            currency: Specify the currency you want to debit. Any value
+                from the ``Currency`` enum.
+            amount: Amount should be in kobo if currency is ``Currency.NGN``, pesewas,
+                if currency is ``Currency.GHS``, and cents, if currency is ``Currency.ZAR``
+            email: Customer's email address (attached to the authorization code)
+            reference: Unique transaction reference. Only `-, ., =`
+                 and alphanumeric characters allowed.
+            at_least: Minimum amount to charge
+
+        Returns:
+            A named tuple containing the response gotten from paystack's server.
+
+        Raises:
+            InvalidDataError: When Customer's email is not provided. When Customer's auth code is not provided.
         """
         amount = validate_amount(amount)
-        url = self._url("/transfer")
+        if at_least:
+            at_least = validate_amount(at_least)
+
+        if not email:
+            raise InvalidDataError("Customer's Email is required to charge")
+
+        if not auth_code:
+            raise InvalidDataError("Customer's Auth code is required to charge")
+
+        url = self._parse_url("/transaction/partial_debit")
         payload = {
+            "authorization_code": auth_code,
+            "currency": currency,
             "amount": amount,
-            "reason": reason,
-            "recipient": recipient_code,
-            "source": "balance",
-            "currency": "NGN",
+            "email": email,
         }
-        if reference:
-            payload.update({"reference": reference})
+        optional_params = [("reference", reference), ("at_least", at_least)]
+        payload = add_to_payload(optional_params, payload)
 
-        return self._handle_request("POST", url, payload)
+        return await self._handle_request(HTTPMethod.POST, url, payload)
```

### Comparing `pypaystack2-1.1.3/pypaystack2/api/transfers.py` & `pypaystack2-2.0.0/pypaystack2/api/apple_pay.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,176 +1,113 @@
-from typing import Optional
+from pypaystack2.baseapi import BaseAPI, BaseAsyncAPI
+from pypaystack2.utils import HTTPMethod, Response
 
-from pypaystack2.baseapi import BaseAPI, Response
-from pypaystack2.utils import (
-    Currency,
-    add_to_payload,
-    append_query_params,
-    validate_amount,
-)
-
-
-class Transfer(BaseAPI):
-    """Provides a wrapper for paystack Transfers API
-
-    The Transfers API allows you to automate sending money on your integration
-    https://paystack.com/docs/api/#transfer
-
-    Note
-    ----
-    This feature is only available to businesses in Nigeria and Ghana.
+
+class ApplePay(BaseAPI):
+    """Provides a wrapper for paystack Apple Pay API
+
+    The Apple Pay API allows you register your application's top-level domain or subdomain.
+    [Visit paystack api doc](https://paystack.com/docs/api/apple-pay/)
     """
 
-    def initiate(
-        self,
-        amount: int,
-        recipient: str,
-        reason: Optional[str] = None,
-        currency: Optional[Currency] = None,
-        reference: Optional[str] = None,
-        source="balance",
-    ) -> Response:
-        """
-        amount: int
-        recipient: str
-        reason: Optional[str]
-        currency: Optional[Currency]
-        reference: Optional[str]
-        source: str
-
-        Returns
-        -------
-        Response
-            A named tuple containing the response gotten from paystack's server.
-        """
-        amount = validate_amount(amount)
+    def register_domain(self, domain_name: str) -> Response:
+        """Register a top-level domain or subdomain for your Apple Pay integration.
 
-        url = self._url("/transfer")
+        This method can only be called with one domain or subdomain at a time.
 
-        payload = {
-            "amount": amount,
-            "recipient": recipient,
-            "source": source,
-        }
-        optional_params = [
-            ("reason", reason),
-            ("reference", reference),
-            ("currency", currency),
-        ]
-        payload = add_to_payload(optional_params, payload)
-        return self._handle_request("POST", url, payload)
-
-    def finalize(
-        self,
-        transfer_code: str,
-        otp: str,
-    ) -> Response:
-        """
-        Parameters
-        ----------
-        transfer_code: str
-        otp: str
-
-        Returns
-        -------
-        Response
+
+        Args:
+            domain_name: Domain name to be registered.
+
+        Returns:
             A named tuple containing the response gotten from paystack's server.
         """
 
-        url = self._url("/transfer/finalize_transfer")
-
+        url = self._parse_url("/apple-pay/domain")
         payload = {
-            "transfer_code": transfer_code,
-            "otp": otp,
+            "domainName": domain_name,
         }
-        return self._handle_request("POST", url, payload)
+        return self._handle_request(HTTPMethod.POST, url, payload)
 
-    def bulk_transfer(self, transfers: list, source="balance") -> Response:
-        """
+    def get_domains(self) -> Response:
+        """Fetches all registered domains on your integration.
 
-        Parameters
-        ----------
-        transfers: list
-        source: str
+        Returns an empty array if no domains have been added.
 
-        Returns
-        -------
-        Response
+        Returns:
             A named tuple containing the response gotten from paystack's server.
         """
 
-        url = self._url("/transfer/bulk")
+        url = self._parse_url("/apple-pay/domain")
+        return self._handle_request(HTTPMethod.GET, url)
+
+    def unregister_domain(self, domain_name: str) -> Response:
+        """Unregister a top-level domain or subdomain previously used for your Apple Pay integration.
+
+        Returns:
+            A named tuple containing the response gotten from paystack's server.
+        """
 
+        url = self._parse_url("/apple-pay/domain")
         payload = {
-            "transfers": transfers,
-            "source": source,
+            "domainName": domain_name,
         }
-        return self._handle_request("POST", url, payload)
+        # return self._handle_request(HTTPMethod.DELETE, url, payload)
+        raise NotImplementedError(
+            "The package `httpx` which PyPaystack uses to make REST "
+            "API calls does not allow HTTPMethod.DELETE have a body"
+        )
 
-    def get_transfers(
-        self,
-        customer: str,
-        page=1,
-        pagination=50,
-        start_date: Optional[str] = None,
-        end_date: Optional[str] = None,
-    ) -> Response:
-        """
 
-        Parameters
-        ----------
-        customer: str
-        page: int
-        pagination: int
-        start_date: Optional[str]
-        end_date: Optional[str]
+class AsyncApplePay(BaseAsyncAPI):
+    """Provides a wrapper for paystack Apple Pay API
+
+    The Apple Pay API allows you register your application's top-level domain or subdomain.
+    [Visit paystack api doc](https://paystack.com/docs/api/apple-pay/)
+    """
+
+    async def register_domain(self, domain_name: str) -> Response:
+        """Register a top-level domain or subdomain for your Apple Pay integration.
 
-        Returns
-        -------
-        Response
+        This method can only be called with one domain or subdomain at a time.
+
+        Args:
+            domain_name: Domain name to be registered.
+
+        Returns:
             A named tuple containing the response gotten from paystack's server.
         """
-        url = self._url(f"/transfer?perPage={pagination}")
-        query_params = [
-            ("customer", customer),
-            ("page", page),
-            ("from", start_date),
-            ("to", end_date),
-        ]
-        url = append_query_params(query_params, url)
-        return self._handle_request("GET", url)
 
-    def get_transfer(
-        self,
-        id_or_code: str,
-    ) -> Response:
-        """
+        url = self._parse_url("/apple-pay/domain")
+        payload = {
+            "domainName": domain_name,
+        }
+        return await self._handle_request(HTTPMethod.POST, url, payload)
 
-        Parameters
-        ----------
-        id_or_code: str
+    async def get_domains(self) -> Response:
+        """Fetches all registered domains on your integration.
 
-        Returns
-        -------
-        Response
+        Returns an empty array if no domains have been added.
+
+        Returns:
             A named tuple containing the response gotten from paystack's server.
         """
-        url = self._url(f"/transfer/{id_or_code}")
-        return self._handle_request("GET", url)
 
-    def verify(
-        self,
-        reference: str,
-    ) -> Response:
-        """
+        url = self._parse_url("/apple-pay/domain")
+        return await self._handle_request(HTTPMethod.GET, url)
 
-        Parameters
-        ----------
-        reference: str
+    async def unregister_domain(self, domain_name: str) -> Response:
+        """Unregister a top-level domain or subdomain previously used for your Apple Pay integration.
 
-        Returns
-        -------
-        Response
+        Returns:
             A named tuple containing the response gotten from paystack's server.
         """
-        url = self._url(f"/transfer/verify/{reference}")
-        return self._handle_request("GET", url)
+
+        url = self._parse_url("/apple-pay/domain")
+        payload = {
+            "domainName": domain_name,
+        }
+        # return await self._handle_request(HTTPMethod.DELETE, url, payload)
+        raise NotImplementedError(
+            "The package `httpx` which PyPaystack uses to make REST "
+            "API calls does not allow HTTPMethod.DELETE have a body"
+        )
```

### Comparing `pypaystack2-1.1.3/pyproject.toml` & `pypaystack2-2.0.0/pyproject.toml`

 * *Files 27% similar despite different names*

```diff
@@ -1,31 +1,32 @@
 [tool.poetry]
 name = "pypaystack2"
-version = "1.1.3"
-description = "A developer friendly [Paystack](https://paystack.com/) API wrapper."
+version = "2.0.0"
+description = "A developer-friendly API wrapper."
 authors = ["Gbenga Adeyi <adeyigbenga005@gmail.com>"]
 readme = "README.md"
 packages = [{ include = "pypaystack2" }]
-keywords = ["paystack-python", "pypaystack", "paystack"]
+keywords = ["paystack-python", "pypaystack", "paystack", "paystackapi"]
 license = "MIT"
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
 ]
 
 [tool.poetry.dependencies]
 python = "^3.7"
-requests = "^2.28.2"
+httpx = "^0.24.0"
 
 [tool.poetry.group.dev.dependencies]
 python-dotenv = "^0.21.0"
 mkdocs = "^1.4.2"
 mkdocs-material = "^8.5.11"
 typer = "^0.7.0"
-mkdocstrings = { version = "^0.19.1", extras = ["python"], optional = true }
+mkdocstrings = {extras = ["python"], version = "^0.21.2"}
 pytest = "^7.2.0"
 black = "^22.12.0"
+tomli = "^2.0.1"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

