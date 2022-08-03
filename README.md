# Kiosk User Interface

## Install Docker
```
$ apt update
$ apt install docker.io -y
```

## Image Pulling
```
docker pull rjsdnfk9/ksk_tomcat:1.0
docker pull rjsdnfk9/ksk_mysql:1.0
```

## Running & Execute tomcat
```
$ docker run --name tomcat rjsdnfk9/ksk_tomcat:1.0
```

## Running & Execute MySQL
```
$ docker run --name mysql rjsdnfk9/ksk_mysql:1.0
$ docker exec -it mysql /bin/bash
```
### In the MySQL Contatiner
```
$ mysql -u root -p
$ {private_password} 
$ use ksk;
$ select * from clothes;
```

## Clothes Table
+--------------+-----------------+-----------------------------------------------------+-----------------------------------------------------------------------------------+---------+-------+---------+-----------+
| category     | brand           | name                                                | img                                                                               | price   | stock | color   | readcount |
+--------------+-----------------+-----------------------------------------------------+-----------------------------------------------------------------------------------+---------+-------+---------+-----------+
| neat_sweater | 5252            | 1701 KNIT PULLOVER                                  | https://image.msscdn.net/images/goods_img/20200924/1623269/1623269_1_500.jpg      | 89,000  |    38 | cream   |         0 |
| t-shirts     | 5252            | 2021 SIGNATURE T-SHIRTS                             | https://image.msscdn.net/images/goods_img/20210318/1853315/1853315_2_500.png      | 39,000  |     4 | cream   |         0 |
| t-shirts     | 5252            | 2021 SIGNATURE T-SHIRTS BLACK                       | https://image.msscdn.net/images/goods_img/20210318/1853316/1853316_1_500.png      | 39,000  |     3 | black   |         0 |
| t-shirts     | 5252            | 2021 SIGNATURE T-SHIRTS GREEN                       | https://image.msscdn.net/images/goods_img/20210318/1853313/1853313_1_500.png      | 39,000  |     5 | green   |         0 |
| t-shirts     | 5252            | 2021 SIGNATURE T-SHIRTS NAVY                        | https://image.msscdn.net/images/goods_img/20210318/1853314/1853314_1_500.png      | 39,000  |     6 | navy    |         0 |
| t-shirts     | 5252            | 2021 SIGNATURE T-SHIRTS PINK                        | https://image.msscdn.net/images/goods_img/20210318/1853307/1853307_1_500.png      | 39,000  |     6 | pink    |         0 |
| t-shirts     | 5252            | 2021 SIGNATURE T-SHIRTS PURPLE                      | https://image.msscdn.net/images/goods_img/20210318/1853308/1853308_1_500.png      | 39,000  |     8 | purple  |         0 |
| t-shirts     | 5252            | 2021 SIGNATURE T-SHIRTS WHITE                       | https://image.msscdn.net/images/goods_img/20210318/1853317/1853317_1_500.png      | 39,000  |     3 | white   |         0 |
| shirts       | ROMANTIC CROWN  | 21C BOYS RUGBY SHIRT_BLUE                           | https://image.msscdn.net/images/goods_img/20190812/1116304/1116304_1_500.jpg      | 62,000  |    46 | blue    |         0 |
| t-shirts     | NIKE            | ACADEMY SHORT SLEEVE                                | https://image.msscdn.net/images/goods_img/20200710/1512338/1512338_1_500.jpg      | 22,700  |    12 | black   |         0 |
| t-shirts     | ROMANTIC CROWN  | AMUR TIGER TEE_BLACK                                | https://image.msscdn.net/images/goods_img/20210330/1870166/1870166_2_500.jpg      | 34,000  |     3 | black   |         0 |
| t-shirts     | THISISNEVERTHAT | ARC LOGO TEE WINE                                   | https://image.msscdn.net/images/goods_img/20210319/1854526/1854526_1_500.jpg      | 27,300  |     8 | wine    |         0 |
| shirts       | ROMANTIC CROWN  | ARCH LOGO TIE DYE SHIRT_SKY BLUE                    | https://image.msscdn.net/images/goods_img/20200417/1408601/1408601_1_500.jpg      | 68,000  |    12 | skyblue |         0 |
| shirts       | PLAC            | BASIC DENIM SHIRTS MID WASHED                       | https://image.msscdn.net/images/prd_img/20210803/2046875/detail_2046875_2_500.jpg | 89,000  |    59 | blue    |         0 |
| shirts       | LAFUDGESTORE    | CITYBOY BIG OVER COLLAR SHIRTS CREAM STRIPE         | https://image.msscdn.net/images/goods_img/20210614/1994685/1994685_1_500.jpg      | 56,000  |    19 | cream   |         0 |
| shirts       | LAFUDGESTORE    | CITYBOY BIG OVER LINEN SHIRTS NAVY                  | https://image.msscdn.net/images/goods_img/20210518/1956629/1956629_1_500.jpg      | 47,000  |    26 | navy    |         0 |
| shirts       | LAFUDGESTORE    | CITYBOY BIG OVER OXFORD COLLAR SHORT SHIRTS         | https://image.msscdn.net/images/goods_img/20210614/1994665/1994665_1_500.jpg      | 45,000  |    13 | blue    |         0 |
| shirts       | LAFUDGESTORE    | CITYBOY BIG OVER OXFORD COLLAR SHORT SHIRTS SKYBLUE | https://image.msscdn.net/images/goods_img/20210614/1994669/1994669_1_500.jpg      | 45,000  |    11 | skyblue |         0 |
| shirts       | LAFUDGESTORE    | CITYBOY BIGOVER LINEN SHIRTS                        | https://image.msscdn.net/images/goods_img/20210518/1956618/1956618_1_500.jpg      | 47,000  |    22 | blue    |         0 |
| neat_sweater | 5252            | CLASSIC LOGO TWIST KNIT PULLOVER GREY               | https://image.msscdn.net/images/goods_img/20200810/1543748/1543748_2_500.png      | 82,000  |    42 | grey    |         0 |
| shirts       | LAFUDGESTORE    | CLASSIC OVER BAND COLLAR SHIRTS GREY CHECK          | https://image.msscdn.net/images/goods_img/20210426/1921503/1921503_1_500.jpg      | 47,000  |    19 | grey    |         0 |
| neat_sweater | ROMANTIC CROWN  | COLOR WAVE KNITTED POLO SHIRTS_NAVY                 | https://image.msscdn.net/images/goods_img/20200810/1542738/1542738_1_500.jpg      | 72,000  |    49 | navy    |         0 |
| shirts       | ROMANTIC CROWN  | CONSTELLATION SHIRT_NAVY                            | https://image.msscdn.net/images/goods_img/20210304/1827106/1827106_1_500.jpg      | 78,000  |    15 | navy    |         0 |
| shirts       | ROMANTIC CROWN  | CONSTELLATION SHIRT_OATMEAL                         | https://image.msscdn.net/images/goods_img/20210304/1827110/1827110_1_500.jpg      | 78,000  |    32 | oatmeal |         0 |
| shirts       | ROMANTIC CROWN  | CORDUROY WIDE SHIRT_YELLOW                          | https://image.msscdn.net/images/goods_img/20191007/1177978/1177978_1_500.jpg      | 78,000  |    44 | yellow  |         0 |
| t-shirts     | THISISNEVERTHAT | DREAMING TEE WHITE                                  | https://image.msscdn.net/images/goods_img/20210415/1901067/1901067_1_500.jpg      | 29,400  |     6 | white   |         0 |
| neat_sweater | ROMANTIC CROWN  | E.D.V Reverse Knit Crewneck_Yellow                  | https://image.msscdn.net/images/prd_img/20190221/960804/detail_960804_2_500.jpg   | 72,000  |    55 | yellow  |         0 |
| t-shirts     | 5252            | E.T FULL MOON T-SHIRTS BLACK                        | https://image.msscdn.net/images/goods_img/20210524/1964819/1964819_1_500.png      | 45,000  |     6 | black   |         0 |
| t-shirts     | ROMANTIC CROWN  | FIELD REFEREE JERSEY_YELLOW                         | https://image.msscdn.net/images/goods_img/20200427/1422643/1422643_1_500.jpg      | 38,000  |     8 | yellow  |         0 |
| shirts       | LAFUDGESTORE    | FRENCH OVER SLIT SHIRTS SEERSUCKER GREEN            | https://image.msscdn.net/images/goods_img/20210426/1921492/1921492_1_500.jpg      | 45,000  |    24 | green   |         0 |
| neat_sweater | ROMANTIC CROWN  | GNAC CABLE KNIT POLO_BUTTER                         | https://image.msscdn.net/images/goods_img/20200203/1287627/1287627_1_500.jpg      | 48,000  |    79 | yellow  |         0 |
| neat_sweater | 5252            | GRADATION BASIC KNIT PULLOVER CORAL                 | https://image.msscdn.net/images/goods_img/20200810/1543743/1543743_2_500.png      | 102,000 |    33 | coral   |         0 |
| t-shirts     | NIKE            | JORDAN DRI-FIT SHORT SLEEVE                         | https://image.msscdn.net/images/goods_img/20210820/2073105/2073105_1_500.jpg      | 46,300  |     7 | black   |         0 |
| shirts       | ROMANTIC CROWN  | Life Belt Bowling Shirts_Yellow                     | https://image.msscdn.net/images/goods_img/20190520/1049785/1049785_1_500.jpg      | 65,000  |     5 | yellow  |         0 |
| t-shirts     | ROMANTIC CROWN  | LIFE IS ROMANTIC TEE_BLACK                          | https://image.msscdn.net/images/goods_img/20200327/1372401/1372401_1_500.jpg      | 34,000  |     7 | black   |         0 |
| shirts       | ROMANTIC CROWN  | MODERN LAUREL SHIRT_LIGHT GREEN                     | https://image.msscdn.net/images/goods_img/20200812/1547076/1547076_5_500.jpg      | 72,000  |    32 | green   |         0 |
| neat_sweater | LAFUDGESTORE    | MOHAIR CLUB KNIT VEST CAMEL                         | https://image.msscdn.net/images/goods_img/20210813/2064510/2064510_2_500.jpg      | 56,000  |    14 | beige   |         0 |
| neat_sweater | LAFUDGESTORE    | MOHAIR CLUB KNIT VEST DARK NAVY                     | https://image.msscdn.net/images/goods_img/20210813/2064511/2064511_2_500.jpg      | 56,000  |    19 | navy    |         0 |
| neat_sweater | LAFUDGESTORE    | MOHAIR CLUB KNIT VEST SEA GREEN                     | https://image.msscdn.net/images/goods_img/20210813/2064509/2064509_2_500.jpg      | 56,000  |    14 | green   |         0 |
| neat_sweater | 5252            | OIOI LOGO KNIT GREEN                                | https://image.msscdn.net/images/goods_img/20210817/2065875/2065875_1_500.png      | 79,000  |    21 | green   |         0 |
| neat_sweater | 5252            | OIOI LOGO KNIT GREY                                 | https://image.msscdn.net/images/goods_img/20210817/2065880/2065880_1_500.png      | 79,000  |    26 | grey    |         0 |
| neat_sweater | 5252            | OIOI LOGO KNIT IVORY                                | https://image.msscdn.net/images/goods_img/20210817/2065882/2065882_1_500.png      | 79,000  |    18 | ivory   |         0 |
| shirts       | PLAC            | OVERSIZED SHIRTS WHITE                              | https://image.msscdn.net/images/prd_img/20210309/1835799/detail_1835799_2_500.jpg | 79,000  |    15 | white   |         0 |
| shirts       | PLAC            | PADDING CHECK SHIRTS GREY                           | https://image.msscdn.net/images/prd_img/20201118/1694319/detail_1694319_2_500.jpg | 139,000 |    39 | grey    |         0 |
| neat_sweater | 5252            | PARADISE JACQUARD KNIT CREAM                        | https://image.msscdn.net/images/goods_img/20210129/1769259/1769259_1_500.png      | 94,000  |    39 | cream   |         0 |
| neat_sweater | 5252            | PARADISE JACQUARD KNIT PINK                         | https://image.msscdn.net/images/goods_img/20210129/1769253/1769253_1_500.png      | 94,000  |    50 | pink    |         0 |
| neat_sweater | ROMANTIC CROWN  | RC CLUB KNIT POLO_LIGHT WHITE                       | https://image.msscdn.net/images/goods_img/20210812/2061764/2061764_2_500.jpg      | 84,000  |    35 | white   |         0 |
| neat_sweater | ROMANTIC CROWN  | RC CLUB KNIT POLO_LIGHT YELLOW                      | https://image.msscdn.net/images/goods_img/20210812/2061765/2061765_2_500.jpg      | 84,000  |    45 | yellow  |         0 |
| shirts       | ROMANTIC CROWN  | RC CLUB OXFORD SHIRT_LIGHT YELLOW                   | https://image.msscdn.net/images/goods_img/20210730/2045155/2045155_2_500.jpg      | 72,000  |    12 | yellow  |         0 |
| shirts       | ROMANTIC CROWN  | RC CLUB OXFORD SHIRT_SKY BLUE                       | https://image.msscdn.net/images/goods_img/20210730/2045154/2045154_2_500.jpg      | 72,000  |     8 | skyblue |         0 |
| shirts       | ROMANTIC CROWN  | RC CLUB STRIPE SHIRT_BLUE                           | https://image.msscdn.net/images/prd_img/20210730/2045153/detail_2045153_3_500.jpg | 72,000  |    10 | blue    |         0 |
| neat_sweater | ROMANTIC CROWN  | RMTC CLUB COLLAR KNIT NAVY                          | https://image.msscdn.net/images/goods_img/20210113/1747266/1747266_1_500.jpg      | 78,000  |    39 | navy    |         0 |
| t-shirts     | ROMANTIC CROWN  | RMTC STRIPED TEE_OATMEAL                            | https://image.msscdn.net/images/goods_img/20200406/1386499/1386499_4_500.jpg      | 42,000  |     9 | oatmeal |         0 |
| t-shirts     | ROMANTIC CROWN  | RMTCRW LOGO TEE_NAVY                                | https://image.msscdn.net/images/goods_img/20200327/1372407/1372407_1_500.jpg      | 34,000  |     3 | navy    |         0 |
| t-shirts     | ROMANTIC CROWN  | RMTCRW LOGO TEE_WHITE                               | https://image.msscdn.net/images/goods_img/20200327/1372405/1372405_1_500.jpg      | 34,000  |     3 | white   |         0 |
| neat_sweater | ROMANTIC CROWN  | RUNNING TRACK JACQUARD KNIT_YELLOW                  | https://image.msscdn.net/images/goods_img/20200113/1268882/1268882_1_500.jpg      | 85,000  |    53 | yellow  |         0 |
| t-shirts     | NIKE            | SB LOGO SKATE SHORT SLEEVE                          | https://image.msscdn.net/images/goods_img/20210716/2031049/2031049_1_500.jpg      | 38,900  |     5 | black   |         0 |
| shirts       | ROMANTIC CROWN  | SIGNATURE CLUB SHIRT_WHITE                          | https://image.msscdn.net/images/goods_img/20210811/2057467/2057467_2_500.jpg      | 72,000  |    18 | white   |         0 |
| neat_sweater | LAFUDGESTORE    | SKASHI OVER PK COLLAR KNIT NAVY                     | https://image.msscdn.net/images/goods_img/20210531/1976397/1976397_1_500.jpg      | 69,000  |     9 | navy    |         0 |
| t-shirts     | ROMANTIC CROWN  | SLOGAN LIST LOGO TEE_LIGHT YELLOW                   | https://image.msscdn.net/images/goods_img/20210414/1897545/1897545_2_500.jpg      | 34,000  |    18 | yellow  |         0 |
| t-shirts     | THISISNEVERTHAT | SP-LOGO STRIPED TEE NAVY/GREY                       | https://image.msscdn.net/images/goods_img/20200318/1356522/1356522_1_500.jpg      | 21,000  |    26 | grey    |         0 |
| neat_sweater | ROMANTIC CROWN  | SUNDAY SYNDROME SCRIBBLE LOGO KNITWEAR_GREY         | https://image.msscdn.net/images/goods_img/20201019/1653872/1653872_1_500.jpg      | 68,000  |    38 | grey    |         0 |
| neat_sweater | 5252            | TURTLE NECK HEAVY KNIT NAVY                         | https://image.msscdn.net/images/goods_img/20191010/1183063/1183063_2_500.jpg      | 98,000  |    55 | navy    |         0 |
| neat_sweater | PLAC            | TURTLENECK KNIT BEIGE                               | https://image.msscdn.net/images/prd_img/20201118/1694326/detail_1694326_2_500.jpg | 69,000  |    50 | beige   |         0 |
| neat_sweater | PLAC            | TURTLENECK KNIT GREY                                | https://image.msscdn.net/images/prd_img/20201118/1694327/detail_1694327_2_500.jpg | 69,000  |    42 | grey    |         0 |
| neat_sweater | ROMANTIC CROWN  | WOMANS V NECK KNITWEAR_BLACK                        | https://image.msscdn.net/images/prd_img/20200812/1547050/detail_1547050_4_500.jpg | 82,000  |    43 | black   |         0 |
+--------------+-----------------+-----------------------------------------------------+-----------------------------------------------------------------------------------+---------+-------+---------+-----------+
