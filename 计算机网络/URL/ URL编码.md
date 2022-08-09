# URL 编码

## 示例1

原 url：

```
https://lf-dy-sourcecdn-tos.bytegecko.com/obj/byte-gurd-source/1325/gecko/resource/fe_pay_middle_page/pages/credit_card_sms/index.html?jump_schema=snssdk1128://webcast_lynxview?url=https://lf-dy-sourcecdn-tos.bytegecko.com/obj/byte-gurd-source/douyin/wallet/prod/fe_lynx_wallet/credit_card_repayment/template.js&support_exchange_theme=1&allow_exchange=0&hide_nav_bar=1&status_bar_color=black&trans_status_bar=1&enter_from=wallet_creditcard_repay_page&card_id=BID20220726195748297508868163
```

* part 1

```
https://lf-dy-sourcecdn-tos.bytegecko.com/obj/byte-gurd-source/1325/gecko/resource/fe_pay_middle_page/pages/credit_card_sms/index.html
```

* part 2

```
?jump_schema=snssdk1128://webcast_lynxview?url=https://lf-dy-sourcecdn-tos.bytegecko.com/obj/byte-gurd-source/douyin/wallet/prod/fe_lynx_wallet/credit_card_repayment/template.js&support_exchange_theme=1&allow_exchange=0&hide_nav_bar=1&status_bar_color=black&trans_status_bar=1&enter_from=wallet_creditcard_repay_page&card_id=BID20220726195748297508868163
```

* part 2.1 jump_schema=...

```
snssdk1128://webcast_lynxview?url=https://lf-dy-sourcecdn-tos.bytegecko.com/obj/byte-gurd-source/douyin/wallet/prod/fe_lynx_wallet/credit_card_repayment/template.js&support_exchange_theme=1&allow_exchange=0&hide_nav_bar=1&status_bar_color=black&trans_status_bar=1&enter_from=wallet_creditcard_repay_page&card_id=BID20220726195748297508868163
```

* part 2.1.1 url=...

```
url=https://lf-dy-sourcecdn-tos.bytegecko.com/obj/byte-gurd-source/douyin/wallet/prod/fe_lynx_wallet/credit_card_repayment/template.js
```

encode 步骤：

1. 先对 2.1.1 encode，得到:

```
https%3A%2F%2Flf-dy-sourcecdn-tos.bytegecko.com%2Fobj%2Fbyte-gurd-source%2Fdouyin%2Fwallet%2Fprod%2Ffe_lynx_wallet%2Fcredit_card_repayment%2Ftemplate.js
```

此时 part 2 为:

```
snssdk1128://webcast_lynxview?url=https%3A%2F%2Flf-dy-sourcecdn-tos.bytegecko.com%2Fobj%2Fbyte-gurd-source%2Fdouyin%2Fwallet%2Fprod%2Ffe_lynx_wallet%2Fcredit_card_repayment%2Ftemplate.js&support_exchange_theme=1&allow_exchange=0&hide_nav_bar=1&status_bar_color=black&trans_status_bar=1&enter_from=wallet_creditcard_repay_page&card_id=BID20220726195748297508868163
```

2. 对新得到的 part 2 encode，得到:

```
jump_schema=snssdk1128%3A%2F%2Fwebcast_lynxview%3Furl%3Dhttps%253A%252F%252Flf-dy-sourcecdn-tos.bytegecko.com%252Fobj%252Fbyte-gurd-source%252Fdouyin%252Fwallet%252Fprod%252Ffe_lynx_wallet%252Fcredit_card_repayment%252Ftemplate.js%26support_exchange_theme%3D1%26allow_exchange%3D0%26hide_nav_bar%3D1%26status_bar_color%3Dblack%26trans_status_bar%3D1%26enter_from%3Dwallet_creditcard_repay_page%26card_id%3DBID20220726195748297508868163
```

3. 所以正确 encode 后得到的 url 为:

```
https://lf-dy-sourcecdn-tos.bytegecko.com/obj/byte-gurd-source/1325/gecko/resource/fe_pay_middle_page/pages/credit_card_sms/index.html?jump_schema=snssdk1128%3A%2F%2Fwebcast_lynxview%3Furl%3Dhttps%253A%252F%252Flf-dy-sourcecdn-tos.bytegecko.com%252Fobj%252Fbyte-gurd-source%252Fdouyin%252Fwallet%252Fprod%252Ffe_lynx_wallet%252Fcredit_card_repayment%252Ftemplate.js%26support_exchange_theme%3D1%26allow_exchange%3D0%26hide_nav_bar%3D1%26status_bar_color%3Dblack%26trans_status_bar%3D1%26enter_from%3Dwallet_creditcard_repay_page%26card_id%3DBID20220726195748297508868163
```