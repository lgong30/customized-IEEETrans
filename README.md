# Customized IEEETrans

This repo provides customized version of `IEEEtrans.cls` and 
`IEEEtran.bst`.

For `IEEEtrans.cls`, the major customizations are:
+ changing the style of multiple citations in a single place from `], [` to `, ` (_i.e.,_ removing 
`]` and `[`). For example, `[1], [5], [8]` ==> `[1, 5, 8]`. Similarly, 
`]--[` to `--`. For example, `[1]-[5]` ==> `[1-5]`.

For `IEEEtrans.bst`, the major customizations are:
+ disabling the feature of 
using a horizontal line to represent authors, if a reference happens to have the same author(s) as its previous one. 
+ disabling the feature of showing pages for conference paper, _i.e.,_ `@inproceedings`.


Other customizations might also be very useful.

- forcing to show full name in all references (useful when using in resume): change [line 132 of IEEEtran.bst](https://github.com/lgong30/customized-IEEETrans/blob/master/IEEEtran.bst#L132) to  
  
  ```TeX
  FUNCTION {default.name.format.string}{ "{ff}{vv~}{ll}{, jj}" }
  % original: FUNCTION {default.name.format.string}{ "{f.~}{vv~}{ll}{, jj}" }
  ```

