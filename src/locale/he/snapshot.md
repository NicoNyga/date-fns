# Hebrew (he) locale

## `format` and `parse`

| Title                           | Token string | Date                     | `format` result                                    | `parse` result           |
| ------------------------------- | ------------ | ------------------------ | -------------------------------------------------- | ------------------------ |
| Calendar year                   | yo           | 1987-02-11T12:13:14.015Z | 1987                                               | 1987-01-01T00:00:00.000Z |
|                                 |              | 0005-01-01T12:13:14.015Z | חמישית                                             | Invalid Date             |
| Local week-numbering year       | Yo           | 1987-02-11T12:13:14.015Z | 1987                                               | 1986-12-28T00:00:00.000Z |
|                                 |              | 0005-01-01T12:13:14.015Z | חמישית                                             | Invalid Date             |
| Quarter (formatting)            | Qo           | 2019-01-01T12:13:14.015Z | ראשון                                              | 2019-01-01T00:00:00.000Z |
|                                 |              | 2019-04-01T12:13:14.015Z | שני                                                | 2019-04-01T00:00:00.000Z |
|                                 | QQQ          | 2019-01-01T12:13:14.015Z | Q1                                                 | 2019-01-01T00:00:00.000Z |
|                                 |              | 2019-04-01T12:13:14.015Z | Q2                                                 | 2019-04-01T00:00:00.000Z |
|                                 | QQQQ         | 2019-01-01T12:13:14.015Z | רבעון 1                                            | 2019-01-01T00:00:00.000Z |
|                                 |              | 2019-04-01T12:13:14.015Z | רבעון 2                                            | 2019-04-01T00:00:00.000Z |
|                                 | QQQQQ        | 2019-01-01T12:13:14.015Z | 1                                                  | 2019-01-01T00:00:00.000Z |
|                                 |              | 2019-04-01T12:13:14.015Z | 2                                                  | 2019-04-01T00:00:00.000Z |
| Quarter (stand-alone)           | qo           | 2019-01-01T12:13:14.015Z | ראשון                                              | 2019-01-01T00:00:00.000Z |
|                                 |              | 2019-04-01T12:13:14.015Z | שני                                                | 2019-04-01T00:00:00.000Z |
|                                 | qqq          | 2019-01-01T12:13:14.015Z | Q1                                                 | 2019-01-01T00:00:00.000Z |
|                                 |              | 2019-04-01T12:13:14.015Z | Q2                                                 | 2019-04-01T00:00:00.000Z |
|                                 | qqqq         | 2019-01-01T12:13:14.015Z | רבעון 1                                            | 2019-01-01T00:00:00.000Z |
|                                 |              | 2019-04-01T12:13:14.015Z | רבעון 2                                            | 2019-04-01T00:00:00.000Z |
| Month (formatting)              | Mo           | 2019-02-11T12:13:14.015Z | שני                                                | 2019-02-01T00:00:00.000Z |
|                                 |              | 2019-07-10T12:13:14.015Z | שביעי                                              | 2019-07-01T00:00:00.000Z |
|                                 | MMM          | 2019-02-11T12:13:14.015Z | פבר׳                                               | 2019-02-01T00:00:00.000Z |
|                                 |              | 2019-07-10T12:13:14.015Z | יולי                                               | 2019-07-01T00:00:00.000Z |
|                                 | MMMM         | 2019-02-11T12:13:14.015Z | פברואר                                             | 2019-02-01T00:00:00.000Z |
|                                 |              | 2019-07-10T12:13:14.015Z | יולי                                               | 2019-07-01T00:00:00.000Z |
|                                 | MMMMM        | 2019-02-11T12:13:14.015Z | 2                                                  | 2019-02-01T00:00:00.000Z |
|                                 |              | 2019-07-10T12:13:14.015Z | 7                                                  | 2019-07-01T00:00:00.000Z |
| Month (stand-alone)             | Lo           | 2019-02-11T12:13:14.015Z | שני                                                | 2019-02-01T00:00:00.000Z |
|                                 |              | 2019-07-10T12:13:14.015Z | שביעי                                              | 2019-07-01T00:00:00.000Z |
|                                 | LLL          | 2019-02-11T12:13:14.015Z | פבר׳                                               | 2019-02-01T00:00:00.000Z |
|                                 |              | 2019-07-10T12:13:14.015Z | יולי                                               | 2019-07-01T00:00:00.000Z |
|                                 | LLLL         | 2019-02-11T12:13:14.015Z | פברואר                                             | 2019-02-01T00:00:00.000Z |
|                                 |              | 2019-07-10T12:13:14.015Z | יולי                                               | 2019-07-01T00:00:00.000Z |
|                                 | LLLLL        | 2019-02-11T12:13:14.015Z | 2                                                  | 2019-02-01T00:00:00.000Z |
|                                 |              | 2019-07-10T12:13:14.015Z | 7                                                  | 2019-07-01T00:00:00.000Z |
| Local week of year              | wo           | 2019-01-01T12:13:14.015Z | ראשון                                              | 2018-12-30T00:00:00.000Z |
|                                 |              | 2019-12-01T12:13:14.015Z | 49                                                 | 2019-12-01T00:00:00.000Z |
| ISO week of year                | Io           | 2019-01-01T12:13:14.015Z | ראשון                                              | 2018-12-31T00:00:00.000Z |
|                                 |              | 2019-12-01T12:13:14.015Z | 48                                                 | 2019-11-25T00:00:00.000Z |
| Day of month                    | do           | 2019-02-11T12:13:14.015Z | 11                                                 | 2019-02-11T00:00:00.000Z |
|                                 |              | 2019-02-28T12:13:14.015Z | 28                                                 | 2019-02-28T00:00:00.000Z |
| Day of year                     | Do           | 2019-02-11T12:13:14.015Z | 42                                                 | 2019-02-11T00:00:00.000Z |
|                                 |              | 2019-12-31T12:13:14.015Z | 365                                                | 2019-12-31T00:00:00.000Z |
| Day of week (formatting)        | E            | 2019-02-11T12:13:14.015Z | יום ב׳                                             | 2019-02-11T00:00:00.000Z |
|                                 |              | 2019-02-15T12:13:14.015Z | יום ו׳                                             | 2019-02-15T00:00:00.000Z |
|                                 | EE           | 2019-02-11T12:13:14.015Z | יום ב׳                                             | 2019-02-11T00:00:00.000Z |
|                                 |              | 2019-02-15T12:13:14.015Z | יום ו׳                                             | 2019-02-15T00:00:00.000Z |
|                                 | EEE          | 2019-02-11T12:13:14.015Z | יום ב׳                                             | 2019-02-11T00:00:00.000Z |
|                                 |              | 2019-02-15T12:13:14.015Z | יום ו׳                                             | 2019-02-15T00:00:00.000Z |
|                                 | EEEE         | 2019-02-11T12:13:14.015Z | יום שני                                            | 2019-02-11T00:00:00.000Z |
|                                 |              | 2019-02-15T12:13:14.015Z | יום שישי                                           | 2019-02-15T00:00:00.000Z |
|                                 | EEEEE        | 2019-02-11T12:13:14.015Z | ב׳                                                 | 2019-02-11T00:00:00.000Z |
|                                 |              | 2019-02-15T12:13:14.015Z | ו׳                                                 | 2019-02-15T00:00:00.000Z |
|                                 | EEEEEE       | 2019-02-11T12:13:14.015Z | ב׳                                                 | 2019-02-11T00:00:00.000Z |
|                                 |              | 2019-02-15T12:13:14.015Z | ו׳                                                 | 2019-02-15T00:00:00.000Z |
| ISO day of week (formatting)    | io           | 2019-02-11T12:13:14.015Z | ראשון                                              | 2019-02-11T00:00:00.000Z |
|                                 |              | 2019-02-15T12:13:14.015Z | חמישי                                              | 2019-02-15T00:00:00.000Z |
|                                 | iii          | 2019-02-11T12:13:14.015Z | יום ב׳                                             | 2019-02-11T00:00:00.000Z |
|                                 |              | 2019-02-15T12:13:14.015Z | יום ו׳                                             | 2019-02-15T00:00:00.000Z |
|                                 | iiii         | 2019-02-11T12:13:14.015Z | יום שני                                            | 2019-02-11T00:00:00.000Z |
|                                 |              | 2019-02-15T12:13:14.015Z | יום שישי                                           | 2019-02-15T00:00:00.000Z |
|                                 | iiiii        | 2019-02-11T12:13:14.015Z | ב׳                                                 | 2019-02-11T00:00:00.000Z |
|                                 |              | 2019-02-15T12:13:14.015Z | ו׳                                                 | 2019-02-15T00:00:00.000Z |
|                                 | iiiiii       | 2019-02-11T12:13:14.015Z | ב׳                                                 | 2019-02-11T00:00:00.000Z |
|                                 |              | 2019-02-15T12:13:14.015Z | ו׳                                                 | 2019-02-15T00:00:00.000Z |
| Local day of week (formatting)  | eo           | 2019-02-11T12:13:14.015Z | שני                                                | 2019-02-11T00:00:00.000Z |
|                                 |              | 2019-02-15T12:13:14.015Z | שישי                                               | 2019-02-15T00:00:00.000Z |
|                                 | eee          | 2019-02-11T12:13:14.015Z | יום ב׳                                             | 2019-02-11T00:00:00.000Z |
|                                 |              | 2019-02-15T12:13:14.015Z | יום ו׳                                             | 2019-02-15T00:00:00.000Z |
|                                 | eeee         | 2019-02-11T12:13:14.015Z | יום שני                                            | 2019-02-11T00:00:00.000Z |
|                                 |              | 2019-02-15T12:13:14.015Z | יום שישי                                           | 2019-02-15T00:00:00.000Z |
|                                 | eeeee        | 2019-02-11T12:13:14.015Z | ב׳                                                 | 2019-02-11T00:00:00.000Z |
|                                 |              | 2019-02-15T12:13:14.015Z | ו׳                                                 | 2019-02-15T00:00:00.000Z |
|                                 | eeeeee       | 2019-02-11T12:13:14.015Z | ב׳                                                 | 2019-02-11T00:00:00.000Z |
|                                 |              | 2019-02-15T12:13:14.015Z | ו׳                                                 | 2019-02-15T00:00:00.000Z |
| Local day of week (stand-alone) | co           | 2019-02-11T12:13:14.015Z | שני                                                | 2019-02-11T00:00:00.000Z |
|                                 |              | 2019-02-15T12:13:14.015Z | שישי                                               | 2019-02-15T00:00:00.000Z |
|                                 | ccc          | 2019-02-11T12:13:14.015Z | יום ב׳                                             | 2019-02-11T00:00:00.000Z |
|                                 |              | 2019-02-15T12:13:14.015Z | יום ו׳                                             | 2019-02-15T00:00:00.000Z |
|                                 | cccc         | 2019-02-11T12:13:14.015Z | יום שני                                            | 2019-02-11T00:00:00.000Z |
|                                 |              | 2019-02-15T12:13:14.015Z | יום שישי                                           | 2019-02-15T00:00:00.000Z |
|                                 | ccccc        | 2019-02-11T12:13:14.015Z | ב׳                                                 | 2019-02-11T00:00:00.000Z |
|                                 |              | 2019-02-15T12:13:14.015Z | ו׳                                                 | 2019-02-15T00:00:00.000Z |
|                                 | cccccc       | 2019-02-11T12:13:14.015Z | ב׳                                                 | 2019-02-11T00:00:00.000Z |
|                                 |              | 2019-02-15T12:13:14.015Z | ו׳                                                 | 2019-02-15T00:00:00.000Z |
| AM, PM                          | a            | 2019-02-11T11:13:14.015Z | לפנה״צ                                             | 2019-02-11T00:00:00.000Z |
|                                 |              | 2019-02-11T14:13:14.015Z | אחה״צ                                              | 2019-02-11T12:00:00.000Z |
|                                 |              | 2019-02-11T19:13:14.015Z | אחה״צ                                              | 2019-02-11T12:00:00.000Z |
|                                 |              | 2019-02-11T02:13:14.015Z | לפנה״צ                                             | 2019-02-11T00:00:00.000Z |
|                                 | aa           | 2019-02-11T11:13:14.015Z | לפנה״צ                                             | 2019-02-11T00:00:00.000Z |
|                                 |              | 2019-02-11T14:13:14.015Z | אחה״צ                                              | 2019-02-11T12:00:00.000Z |
|                                 |              | 2019-02-11T19:13:14.015Z | אחה״צ                                              | 2019-02-11T12:00:00.000Z |
|                                 |              | 2019-02-11T02:13:14.015Z | לפנה״צ                                             | 2019-02-11T00:00:00.000Z |
|                                 | aaa          | 2019-02-11T11:13:14.015Z | לפנה״צ                                             | 2019-02-11T00:00:00.000Z |
|                                 |              | 2019-02-11T14:13:14.015Z | אחה״צ                                              | 2019-02-11T12:00:00.000Z |
|                                 |              | 2019-02-11T19:13:14.015Z | אחה״צ                                              | 2019-02-11T12:00:00.000Z |
|                                 |              | 2019-02-11T02:13:14.015Z | לפנה״צ                                             | 2019-02-11T00:00:00.000Z |
|                                 | aaaa         | 2019-02-11T11:13:14.015Z | לפנה״צ                                             | 2019-02-11T00:00:00.000Z |
|                                 |              | 2019-02-11T14:13:14.015Z | אחה״צ                                              | 2019-02-11T12:00:00.000Z |
|                                 |              | 2019-02-11T19:13:14.015Z | אחה״צ                                              | 2019-02-11T12:00:00.000Z |
|                                 |              | 2019-02-11T02:13:14.015Z | לפנה״צ                                             | 2019-02-11T00:00:00.000Z |
|                                 | aaaaa        | 2019-02-11T11:13:14.015Z | לפנה״צ                                             | 2019-02-11T00:00:00.000Z |
|                                 |              | 2019-02-11T14:13:14.015Z | אחה״צ                                              | 2019-02-11T12:00:00.000Z |
|                                 |              | 2019-02-11T19:13:14.015Z | אחה״צ                                              | 2019-02-11T12:00:00.000Z |
|                                 |              | 2019-02-11T02:13:14.015Z | לפנה״צ                                             | 2019-02-11T00:00:00.000Z |
| AM, PM, noon, midnight          | b            | 2019-02-11T11:13:14.015Z | לפנה״צ                                             | 2019-02-11T00:00:00.000Z |
|                                 |              | 2019-02-11T14:13:14.015Z | אחה״צ                                              | 2019-02-11T12:00:00.000Z |
|                                 |              | 2019-02-11T19:13:14.015Z | אחה״צ                                              | 2019-02-11T12:00:00.000Z |
|                                 |              | 2019-02-11T02:13:14.015Z | לפנה״צ                                             | 2019-02-11T00:00:00.000Z |
|                                 | bb           | 2019-02-11T11:13:14.015Z | לפנה״צ                                             | 2019-02-11T00:00:00.000Z |
|                                 |              | 2019-02-11T14:13:14.015Z | אחה״צ                                              | 2019-02-11T12:00:00.000Z |
|                                 |              | 2019-02-11T19:13:14.015Z | אחה״צ                                              | 2019-02-11T12:00:00.000Z |
|                                 |              | 2019-02-11T02:13:14.015Z | לפנה״צ                                             | 2019-02-11T00:00:00.000Z |
|                                 | bbb          | 2019-02-11T11:13:14.015Z | לפנה״צ                                             | 2019-02-11T00:00:00.000Z |
|                                 |              | 2019-02-11T14:13:14.015Z | אחה״צ                                              | 2019-02-11T12:00:00.000Z |
|                                 |              | 2019-02-11T19:13:14.015Z | אחה״צ                                              | 2019-02-11T12:00:00.000Z |
|                                 |              | 2019-02-11T02:13:14.015Z | לפנה״צ                                             | 2019-02-11T00:00:00.000Z |
|                                 | bbbb         | 2019-02-11T11:13:14.015Z | לפנה״צ                                             | 2019-02-11T00:00:00.000Z |
|                                 |              | 2019-02-11T14:13:14.015Z | אחה״צ                                              | 2019-02-11T12:00:00.000Z |
|                                 |              | 2019-02-11T19:13:14.015Z | אחה״צ                                              | 2019-02-11T12:00:00.000Z |
|                                 |              | 2019-02-11T02:13:14.015Z | לפנה״צ                                             | 2019-02-11T00:00:00.000Z |
|                                 | bbbbb        | 2019-02-11T11:13:14.015Z | לפנה״צ                                             | 2019-02-11T00:00:00.000Z |
|                                 |              | 2019-02-11T14:13:14.015Z | אחה״צ                                              | 2019-02-11T12:00:00.000Z |
|                                 |              | 2019-02-11T19:13:14.015Z | אחה״צ                                              | 2019-02-11T12:00:00.000Z |
|                                 |              | 2019-02-11T02:13:14.015Z | לפנה״צ                                             | 2019-02-11T00:00:00.000Z |
| Flexible day period             | B            | 2019-02-11T11:13:14.015Z | בבוקר                                              | 2019-02-11T04:00:00.000Z |
|                                 |              | 2019-02-11T14:13:14.015Z | אחר הצהריים                                        | 2019-02-11T12:00:00.000Z |
|                                 |              | 2019-02-11T19:13:14.015Z | בערב                                               | 2019-02-11T17:00:00.000Z |
|                                 |              | 2019-02-11T02:13:14.015Z | בלילה                                              | 2019-02-11T00:00:00.000Z |
|                                 | BB           | 2019-02-11T11:13:14.015Z | בבוקר                                              | 2019-02-11T04:00:00.000Z |
|                                 |              | 2019-02-11T14:13:14.015Z | אחר הצהריים                                        | 2019-02-11T12:00:00.000Z |
|                                 |              | 2019-02-11T19:13:14.015Z | בערב                                               | 2019-02-11T17:00:00.000Z |
|                                 |              | 2019-02-11T02:13:14.015Z | בלילה                                              | 2019-02-11T00:00:00.000Z |
|                                 | BBB          | 2019-02-11T11:13:14.015Z | בבוקר                                              | 2019-02-11T04:00:00.000Z |
|                                 |              | 2019-02-11T14:13:14.015Z | אחר הצהריים                                        | 2019-02-11T12:00:00.000Z |
|                                 |              | 2019-02-11T19:13:14.015Z | בערב                                               | 2019-02-11T17:00:00.000Z |
|                                 |              | 2019-02-11T02:13:14.015Z | בלילה                                              | 2019-02-11T00:00:00.000Z |
|                                 | BBBB         | 2019-02-11T11:13:14.015Z | בבוקר                                              | 2019-02-11T04:00:00.000Z |
|                                 |              | 2019-02-11T14:13:14.015Z | אחר הצהריים                                        | 2019-02-11T12:00:00.000Z |
|                                 |              | 2019-02-11T19:13:14.015Z | בערב                                               | 2019-02-11T17:00:00.000Z |
|                                 |              | 2019-02-11T02:13:14.015Z | בלילה                                              | 2019-02-11T00:00:00.000Z |
|                                 | BBBBB        | 2019-02-11T11:13:14.015Z | בבוקר                                              | 2019-02-11T04:00:00.000Z |
|                                 |              | 2019-02-11T14:13:14.015Z | בצהריים                                            | 2019-02-11T12:00:00.000Z |
|                                 |              | 2019-02-11T19:13:14.015Z | בערב                                               | 2019-02-11T17:00:00.000Z |
|                                 |              | 2019-02-11T02:13:14.015Z | בלילה                                              | 2019-02-11T00:00:00.000Z |
| Hour [1-12]                     | ho           | 2019-02-11T11:13:14.015Z | 11                                                 | 2019-02-11T11:00:00.000Z |
|                                 |              | 2019-02-11T23:13:14.015Z | 11                                                 | 2019-02-11T23:00:00.000Z |
| Hour [0-23]                     | Ho           | 2019-02-11T11:13:14.015Z | 11                                                 | 2019-02-11T11:00:00.000Z |
|                                 |              | 2019-02-11T23:13:14.015Z | 23                                                 | 2019-02-11T23:00:00.000Z |
| Hour [0-11]                     | Ko           | 2019-02-11T11:13:14.015Z | 11                                                 | 2019-02-11T11:00:00.000Z |
|                                 |              | 2019-02-11T23:13:14.015Z | 11                                                 | 2019-02-11T23:00:00.000Z |
| Hour [1-24]                     | ko           | 2019-02-11T11:13:14.015Z | 11                                                 | 2019-02-11T11:00:00.000Z |
|                                 |              | 2019-02-11T23:13:14.015Z | 23                                                 | 2019-02-11T23:00:00.000Z |
| Minute                          | mo           | 2019-01-01T12:01:14.015Z | ראשונה                                             | 2019-01-01T12:01:00.000Z |
|                                 |              | 2019-04-01T12:55:14.015Z | 55                                                 | 2019-04-01T12:55:00.000Z |
| Second                          | so           | 2019-01-01T12:13:01.015Z | ראשונה                                             | 2019-01-01T12:13:01.000Z |
|                                 |              | 2019-04-01T12:13:55.015Z | 55                                                 | 2019-04-01T12:13:55.000Z |
| Long localized date             | P            | 1987-02-11T12:13:14.015Z | 11.2.1987                                          | 1987-02-11T00:00:00.000Z |
|                                 |              | 1453-05-29T23:59:59.999Z | 29.5.1453                                          | 1453-05-29T00:00:00.000Z |
|                                 | PP           | 1987-02-11T12:13:14.015Z | 11 בפבר׳ 1987                                      | 1987-02-11T00:00:00.000Z |
|                                 |              | 1453-05-29T23:59:59.999Z | 29 במאי 1453                                       | 1453-05-29T00:00:00.000Z |
|                                 | PPP          | 1987-02-11T12:13:14.015Z | 11 בפברואר 1987                                    | 1987-02-11T00:00:00.000Z |
|                                 |              | 1453-05-29T23:59:59.999Z | 29 במאי 1453                                       | 1453-05-29T00:00:00.000Z |
|                                 | PPPP         | 1987-02-11T12:13:14.015Z | יום רביעי, 11 בפברואר 1987                         | 1987-02-11T00:00:00.000Z |
|                                 |              | 1453-05-29T23:59:59.999Z | יום ראשון, 29 במאי 1453                            | 1453-05-29T00:00:00.000Z |
| Long localized time             | p            | 1987-02-11T12:13:14.015Z | 12:13                                              | 1987-02-11T12:13:00.000Z |
|                                 |              | 1453-05-29T23:59:59.999Z | 23:59                                              | 1453-05-29T23:59:00.000Z |
|                                 | pp           | 1987-02-11T12:13:14.015Z | 12:13:14                                           | 1987-02-11T12:13:14.000Z |
|                                 |              | 1453-05-29T23:59:59.999Z | 23:59:59                                           | 1453-05-29T23:59:59.000Z |
|                                 | ppp          | 1987-02-11T12:13:14.015Z | 12:13:14 GMT+0                                     | Errored                  |
|                                 |              | 1453-05-29T23:59:59.999Z | 23:59:59 GMT+0                                     | Errored                  |
|                                 | pppp         | 1987-02-11T12:13:14.015Z | 12:13:14 GMT+00:00                                 | Errored                  |
|                                 |              | 1453-05-29T23:59:59.999Z | 23:59:59 GMT+00:00                                 | Errored                  |
| Combination of date and time    | Pp           | 1987-02-11T12:13:14.015Z | 11.2.1987, 12:13                                   | 1987-02-11T12:13:00.000Z |
|                                 |              | 1453-05-29T23:59:59.999Z | 29.5.1453, 23:59                                   | 1453-05-29T23:59:00.000Z |
|                                 | PPpp         | 1987-02-11T12:13:14.015Z | 11 בפבר׳ 1987, 12:13:14                            | 1987-02-11T12:13:14.000Z |
|                                 |              | 1453-05-29T23:59:59.999Z | 29 במאי 1453, 23:59:59                             | 1453-05-29T23:59:59.000Z |
|                                 | PPPppp       | 1987-02-11T12:13:14.015Z | 11 בפברואר 1987 בשעה 12:13:14 GMT+0                | Errored                  |
|                                 |              | 1453-05-29T23:59:59.999Z | 29 במאי 1453 בשעה 23:59:59 GMT+0                   | Errored                  |
|                                 | PPPPpppp     | 1987-02-11T12:13:14.015Z | יום רביעי, 11 בפברואר 1987 בשעה 12:13:14 GMT+00:00 | Errored                  |
|                                 |              | 1453-05-29T23:59:59.999Z | יום ראשון, 29 במאי 1453 בשעה 23:59:59 GMT+00:00    | Errored                  |

## `formatDistance`

If now is January 1st, 2000, 00:00.

| Date                     | Result    | `includeSeconds: true` | `addSuffix: true` |
| ------------------------ | --------- | ---------------------- | ----------------- |
| 2006-01-01T00:00:00.000Z | כ־6 שנים  | כ־6 שנים               | בעוד כ־6 שנים     |
| 2005-01-01T00:00:00.000Z | כ־5 שנים  | כ־5 שנים               | בעוד כ־5 שנים     |
| 2004-01-01T00:00:00.000Z | כ־4 שנים  | כ־4 שנים               | בעוד כ־4 שנים     |
| 2003-01-01T00:00:00.000Z | כ־3 שנים  | כ־3 שנים               | בעוד כ־3 שנים     |
| 2002-01-01T00:00:00.000Z | כשנתיים   | כשנתיים                | בעוד כשנתיים      |
| 2001-06-01T00:00:00.000Z | יותר משנה | יותר משנה              | בעוד יותר משנה    |
| 2001-02-01T00:00:00.000Z | כשנה      | כשנה                   | בעוד כשנה         |
| 2001-01-01T00:00:00.000Z | כשנה      | כשנה                   | בעוד כשנה         |
| 2000-06-01T00:00:00.000Z | 5 חודשים  | 5 חודשים               | בעוד 5 חודשים     |
| 2000-03-01T00:00:00.000Z | חודשיים   | חודשיים                | בעוד חודשיים      |
| 2000-02-01T00:00:00.000Z | כחודש     | כחודש                  | בעוד כחודש        |
| 2000-01-15T00:00:00.000Z | 14 ימים   | 14 ימים                | בעוד 14 ימים      |
| 2000-01-02T00:00:00.000Z | יום       | יום                    | מחר               |
| 2000-01-01T06:00:00.000Z | כ־6 שעות  | כ־6 שעות               | בעוד כ־6 שעות     |
| 2000-01-01T01:00:00.000Z | כשעה      | כשעה                   | בעוד כשעה         |
| 2000-01-01T00:45:00.000Z | כשעה      | כשעה                   | בעוד כשעה         |
| 2000-01-01T00:30:00.000Z | 30 דקות   | 30 דקות                | בעוד 30 דקות      |
| 2000-01-01T00:15:00.000Z | 15 דקות   | 15 דקות                | בעוד 15 דקות      |
| 2000-01-01T00:01:00.000Z | דקה       | דקה                    | בעוד דקה          |
| 2000-01-01T00:00:25.000Z | פחות מדקה | חצי דקה                | בעוד פחות מדקה    |
| 2000-01-01T00:00:15.000Z | פחות מדקה | פחות מ־20 שניות        | בעוד פחות מדקה    |
| 2000-01-01T00:00:05.000Z | פחות מדקה | פחות מ־10 שניות        | בעוד פחות מדקה    |
| 2000-01-01T00:00:00.000Z | פחות מדקה | פחות מ־5 שניות         | לפני פחות מדקה    |
| 1999-12-31T23:59:55.000Z | פחות מדקה | פחות מ־10 שניות        | לפני פחות מדקה    |
| 1999-12-31T23:59:45.000Z | פחות מדקה | פחות מ־20 שניות        | לפני פחות מדקה    |
| 1999-12-31T23:59:35.000Z | פחות מדקה | חצי דקה                | לפני פחות מדקה    |
| 1999-12-31T23:59:00.000Z | דקה       | דקה                    | לפני דקה          |
| 1999-12-31T23:45:00.000Z | 15 דקות   | 15 דקות                | לפני 15 דקות      |
| 1999-12-31T23:30:00.000Z | 30 דקות   | 30 דקות                | לפני 30 דקות      |
| 1999-12-31T23:15:00.000Z | כשעה      | כשעה                   | לפני כשעה         |
| 1999-12-31T23:00:00.000Z | כשעה      | כשעה                   | לפני כשעה         |
| 1999-12-31T18:00:00.000Z | כ־6 שעות  | כ־6 שעות               | לפני כ־6 שעות     |
| 1999-12-30T00:00:00.000Z | יומיים    | יומיים                 | שלשום             |
| 1999-12-15T00:00:00.000Z | 17 ימים   | 17 ימים                | לפני 17 ימים      |
| 1999-12-01T00:00:00.000Z | כחודש     | כחודש                  | לפני כחודש        |
| 1999-11-01T00:00:00.000Z | חודשיים   | חודשיים                | לפני חודשיים      |
| 1999-06-01T00:00:00.000Z | 7 חודשים  | 7 חודשים               | לפני 7 חודשים     |
| 1999-01-01T00:00:00.000Z | כשנה      | כשנה                   | לפני כשנה         |
| 1998-12-01T00:00:00.000Z | כשנה      | כשנה                   | לפני כשנה         |
| 1998-06-01T00:00:00.000Z | יותר משנה | יותר משנה              | לפני יותר משנה    |
| 1998-01-01T00:00:00.000Z | כשנתיים   | כשנתיים                | לפני כשנתיים      |
| 1997-01-01T00:00:00.000Z | כ־3 שנים  | כ־3 שנים               | לפני כ־3 שנים     |
| 1996-01-01T00:00:00.000Z | כ־4 שנים  | כ־4 שנים               | לפני כ־4 שנים     |
| 1995-01-01T00:00:00.000Z | כ־5 שנים  | כ־5 שנים               | לפני כ־5 שנים     |
| 1994-01-01T00:00:00.000Z | כ־6 שנים  | כ־6 שנים               | לפני כ־6 שנים     |

## `formatDistanceStrict`

If now is January 1st, 2000, 00:00.

| Date                     | Result   | `addSuffix: true` | With forced unit (i.e. `hour`) |
| ------------------------ | -------- | ----------------- | ------------------------------ |
| 2006-01-01T00:00:00.000Z | 6 שנים   | בעוד 6 שנים       | 52608 שעות                     |
| 2005-01-01T00:00:00.000Z | 5 שנים   | בעוד 5 שנים       | 43848 שעות                     |
| 2004-01-01T00:00:00.000Z | 4 שנים   | בעוד 4 שנים       | 35064 שעות                     |
| 2003-01-01T00:00:00.000Z | 3 שנים   | בעוד 3 שנים       | 26304 שעות                     |
| 2002-01-01T00:00:00.000Z | שנתיים   | בעוד שנתיים       | 17544 שעות                     |
| 2001-06-01T00:00:00.000Z | שנה      | בעוד שנה          | 12408 שעות                     |
| 2001-02-01T00:00:00.000Z | שנה      | בעוד שנה          | 9528 שעות                      |
| 2001-01-01T00:00:00.000Z | שנה      | בעוד שנה          | 8784 שעות                      |
| 2000-06-01T00:00:00.000Z | 5 חודשים | בעוד 5 חודשים     | 3648 שעות                      |
| 2000-03-01T00:00:00.000Z | חודשיים  | בעוד חודשיים      | 1440 שעות                      |
| 2000-02-01T00:00:00.000Z | חודש     | בעוד חודש         | 744 שעות                       |
| 2000-01-15T00:00:00.000Z | 14 ימים  | בעוד 14 ימים      | 336 שעות                       |
| 2000-01-02T00:00:00.000Z | יום      | מחר               | 24 שעות                        |
| 2000-01-01T06:00:00.000Z | 6 שעות   | בעוד 6 שעות       | 6 שעות                         |
| 2000-01-01T01:00:00.000Z | שעה      | בעוד שעה          | שעה                            |
| 2000-01-01T00:45:00.000Z | 45 דקות  | בעוד 45 דקות      | שעה                            |
| 2000-01-01T00:30:00.000Z | 30 דקות  | בעוד 30 דקות      | שעה                            |
| 2000-01-01T00:15:00.000Z | 15 דקות  | בעוד 15 דקות      | 0 שעות                         |
| 2000-01-01T00:01:00.000Z | דקה      | בעוד דקה          | 0 שעות                         |
| 2000-01-01T00:00:25.000Z | 25 שניות | בעוד 25 שניות     | 0 שעות                         |
| 2000-01-01T00:00:15.000Z | 15 שניות | בעוד 15 שניות     | 0 שעות                         |
| 2000-01-01T00:00:05.000Z | 5 שניות  | בעוד 5 שניות      | 0 שעות                         |
| 2000-01-01T00:00:00.000Z | 0 שניות  | לפני 0 שניות      | 0 שעות                         |
| 1999-12-31T23:59:55.000Z | 5 שניות  | לפני 5 שניות      | 0 שעות                         |
| 1999-12-31T23:59:45.000Z | 15 שניות | לפני 15 שניות     | 0 שעות                         |
| 1999-12-31T23:59:35.000Z | 25 שניות | לפני 25 שניות     | 0 שעות                         |
| 1999-12-31T23:59:00.000Z | דקה      | לפני דקה          | 0 שעות                         |
| 1999-12-31T23:45:00.000Z | 15 דקות  | לפני 15 דקות      | 0 שעות                         |
| 1999-12-31T23:30:00.000Z | 30 דקות  | לפני 30 דקות      | שעה                            |
| 1999-12-31T23:15:00.000Z | 45 דקות  | לפני 45 דקות      | שעה                            |
| 1999-12-31T23:00:00.000Z | שעה      | לפני שעה          | שעה                            |
| 1999-12-31T18:00:00.000Z | 6 שעות   | לפני 6 שעות       | 6 שעות                         |
| 1999-12-30T00:00:00.000Z | יומיים   | שלשום             | 48 שעות                        |
| 1999-12-15T00:00:00.000Z | 17 ימים  | לפני 17 ימים      | 408 שעות                       |
| 1999-12-01T00:00:00.000Z | חודש     | לפני חודש         | 744 שעות                       |
| 1999-11-01T00:00:00.000Z | חודשיים  | לפני חודשיים      | 1464 שעות                      |
| 1999-06-01T00:00:00.000Z | 7 חודשים | לפני 7 חודשים     | 5136 שעות                      |
| 1999-01-01T00:00:00.000Z | שנה      | לפני שנה          | 8760 שעות                      |
| 1998-12-01T00:00:00.000Z | שנה      | לפני שנה          | 9504 שעות                      |
| 1998-06-01T00:00:00.000Z | שנתיים   | לפני שנתיים       | 13896 שעות                     |
| 1998-01-01T00:00:00.000Z | שנתיים   | לפני שנתיים       | 17520 שעות                     |
| 1997-01-01T00:00:00.000Z | 3 שנים   | לפני 3 שנים       | 26280 שעות                     |
| 1996-01-01T00:00:00.000Z | 4 שנים   | לפני 4 שנים       | 35064 שעות                     |
| 1995-01-01T00:00:00.000Z | 5 שנים   | לפני 5 שנים       | 43824 שעות                     |
| 1994-01-01T00:00:00.000Z | 6 שנים   | לפני 6 שנים       | 52584 שעות                     |

## `formatRelative`

If now is January 1st, 2000, 00:00.

| Date                     | Result                 |
| ------------------------ | ---------------------- |
| 2000-01-10T00:00:00.000Z | 10.1.2000              |
| 2000-01-05T00:00:00.000Z | יום רביעי בשעה 0:00    |
| 2000-01-02T00:00:00.000Z | מחר בשעה 0:00          |
| 2000-01-01T00:00:00.000Z | היום בשעה 0:00         |
| 1999-12-31T00:00:00.000Z | אתמול בשעה 0:00        |
| 1999-12-27T00:00:00.000Z | יום שני שעבר בשעה 0:00 |
| 1999-12-21T00:00:00.000Z | 21.12.1999             |