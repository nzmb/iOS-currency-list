# iOS-currency-list

Currency list is released in .plist format.

To use it in the project:

- add `Currency.plist` into project

- read pList file

```
+ (NSArray *)defaultCurrencyList {
    NSString * pListPath = [[NSBundle mainBundle] pathForResource:@"Currency" ofType:@"plist"];
    return [NSArray arrayWithContentsOfFile:pListPath];
}
```

__You will get result in `NSArray` with `NSDictionary` with `keys`:__
- code
- name

```
(
        {
        code = AED;
        name = "United Arab Emirates Dirham";
    },
        {
        code = AFN;
        name = "Afghanistan Afghani";
    },
        {
        code = ALL;
        name = "Albania Lek";
    },
        {
        code = AMD;
        name = "Armenia Dram";
    },
        {
        code = ANG;
        name = "Netherlands Antilles Guilder";
    },
        {
        code = AOA;
        name = "Angola Kwanza";
    },
        {
        code = ARS;
        name = "Argentina Peso";
    },
        {
        code = AUD;
        name = "Australia Dollar";
    },
...
```
