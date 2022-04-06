# wrapped24px
an ERC721 wrapper for OpenSea Shared Storefront-based 24px tokens

This is the newer, slightly more gas optimized version. if you are looking for the original, check the [1.1.0](/yoyyyyo/wrapped24px/tree/1.1.0) tag.

Both of these contracts are currently deployed on Ethereum mainnet under these addresses:
| Name              | Address |
|-------------------|---------|
| Wrapped PixelCats | [0x91612c6e205d1597f2fe06e4e2344e0e643d7619](https://etherscan.io/address/0x91612c6e205d1597f2fe06e4e2344e0e643d7619) |
| Wrapped PixelApes | TBD |

## Gas comparison
Note: For single wrap/unwrap comparisons, the wrap/unwrapSingle functions were used for V2.
The simulations include the entire cost of a transaction, and not just a function call.

| Action         | V1 Gas units | V2 Gas units | Difference         |
|----------------|--------------|--------------|--------------------|
| Wrap 1 token   | 129 032      | 119 421      | 9 611 *(7.44 %)*   |
| Wrap 2 tokens  | 188 125      | 177 879      | 10 246 *(5.44 %)*  |
| Wrap 10 tokens | 660 870      | 598 892      | 61 978 *(9.37 %)*  |

| Action           | V1 Gas units | V2 Gas units | Difference         |
|------------------|--------------|--------------|--------------------|
| Unwrap 1 token   | 76 864       | 66 728       | 10 586 *(13.18 %)* |
| Unwrap 2 tokens  | 114 540      | 105 600      | 8 940 *(7.80 %)*   |
| Unwrap 10 tokens | 415 858      | 383 310      | 32 548 *(7.82 %)*  |