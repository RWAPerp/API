# trading orders

| Method | Path                                                                                                    | Auth                  |
| ------ | ------------------------------------------------------------------------------------------------------- | --------------------- |
| DELETE | [`/v1/algo/client/order`](/broken/pages/6ef8a2e4e7478ee41f151da251f4a3983bed5312)                       | RWA                   |
| GET    | [`/v1/algo/client/order/{client_order_id}`](/broken/pages/5202680c90eeb83b1312dcb5d7ac13b6d12ed8a8)     | RWA                   |
| DELETE | [`/v1/algo/order`](/broken/pages/2be1fbd55ec678830fd6b662524ce959c52d42ef)                              | RWA                   |
| POST   | [`/v1/algo/order`](/broken/pages/f37cf847433b20109336fe285d65903e2d97d0af)                              | RWA                   |
| PUT    | [`/v1/algo/order`](/broken/pages/76e4aa5031dd0d20afdaa7f7281d291eee1fb8b6)                              | RWA                   |
| GET    | [`/v1/algo/order/{order_id}`](/broken/pages/76baf5801463ab2dd320d3b3bdc8d4ce0e8c55eb)                   | RWA                   |
| GET    | [`/v1/algo/order/{order_id}/trades`](/broken/pages/cc63157d1504a7664d8a863bd9ae608dda0620d2)            | RWA                   |
| DELETE | [`/v1/algo/orders`](/broken/pages/b78f47c335316e25e8b21aaa201aef8e9f4b12c9)                             | RWA                   |
| GET    | [`/v1/algo/orders`](/broken/pages/6ac575bd9c88a5b5c0c43400fea1c16429a069e4)                             | RWA                   |
| DELETE | [`/v1/batch-order`](/broken/pages/b5bdf9846a0c1b3a4b58b93e0b782c5b0ff85a3c)                             | RWA (`trading` scope) |
| POST   | [`/v1/batch-order`](/broken/pages/26a7c86d4b0bf9070ef8bb564ff61f0a2fa1c03a)                             | RWA (`trading` scope) |
| DELETE | [`/v1/client/batch-order`](/broken/pages/5e989efc107d99a3e5385de67eed4406831dc3fd)                      | RWA (`trading` scope) |
| DELETE | [`/v1/client/order`](/broken/pages/36af33f833da81f2610afefa2bf78522c3ad8b17)                            | RWA (`trading` scope) |
| GET    | [`/v1/client/order/{client_order_id}`](/broken/pages/f8fd4f874b58a26abc49af46da32daef34fb9c40)          | RWA                   |
| GET    | [`/v1/client/orderly_key_ip_restriction`](/broken/pages/0d80541c2fc8115ee1bbf306ca90feea8862a183)       | RWA                   |
| POST   | [`/v1/client/reset_orderly_key_ip_restriction`](/broken/pages/bcfadfe9ee2836c354d9185d275f04005b284bcd) | RWA                   |
| POST   | [`/v1/client/set_orderly_key_ip_restriction`](/broken/pages/c7f7feba41d769c50ffcb06a5bc3edca31968609)   | RWA                   |
| DELETE | [`/v1/order`](/broken/pages/87119cc706b29d55960af96b51ec90a0dbb2052e)                                   | RWA (`trading` scope) |
| POST   | [`/v1/order`](/broken/pages/b9c230b473a4bbeaa9f6fa5ef5d82fbc83aa1bc1)                                   | RWA (`trading` scope) |
| PUT    | [`/v1/order`](/broken/pages/96be0534653963959e1cc2e6b25ca763e92ef3a6)                                   | RWA (`trading` scope) |
| POST   | [`/v1/order/cancel_all_after`](/broken/pages/e8cca95d12288bba73e28beb5ff4cae92bfd265a)                  | RWA                   |
| GET    | [`/v1/order/{order_id}`](/broken/pages/9df8ffcfac4617557ce38b415377f6637ef6e739)                        | RWA                   |
| GET    | [`/v1/order/{order_id}/trades`](/broken/pages/41dad33d38b36946e4159b6ffc128857c3be8006)                 | RWA                   |
| GET    | [`/v1/orderbook/{symbol}`](/broken/pages/72c8ee67f066aaa479fa1f3f57a578b9167c3ed5)                      | RWA                   |
| DELETE | [`/v1/orders`](/broken/pages/432f494e0f8db42bb2a44bc57ba457035c413f09)                                  | RWA (`trading` scope) |
| GET    | [`/v1/orders`](/broken/pages/c891c571483fb6bf046021301e2b28ab696b14f0)                                  | RWA                   |
| GET    | [`/v1/trade/{trade_id}`](/broken/pages/dec4d19fd6b6827de5bddd1c3fd3310195e741b6)                        | RWA                   |
| GET    | [`/v1/trades`](/broken/pages/7a65c3b0bd7266ee8419d804a9adaa27a349ff07)                                  | RWA                   |
