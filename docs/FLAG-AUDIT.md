# Flag audit - IJF April 2026

See [the complete v0.7 audit](RELEASE-AUDIT.md) for Excel differences, uncovered entries and release checks.

## Result

- Compared all 206 country entries in the reference manual.
- Bundled the rendered horizontal and vertical illustrations for 205 catalog entries, including the country-specific emblem variants.
- 50 additional catalog entries are outside this manual. Version 0.7 supplements 16 with the original workbook artwork in both views; 34 retain the base artwork and rotation fallback. They are not described as IJF-verified.
- The unified Korea entry (COR) is present in the manual but is not part of the current app catalog.
- Replaced the generic Taiwan national artwork used for TPE with the Chinese Taipei event flag.
- No changes are made to tournament files or medal ordering.

[Reference manual](https://78884ca60822a34fb0e6-082b8fd5551e97bc65e327988b444396.ssl.cf3.rackcdn.com/up/2026/04/IJF_Flag_Manual_-_01_04_2026_--1776074839.pdf)

Source SHA-256: `411186e50c34b433f72bf56fb24e61604149cfe8a51caf0c5757db8aea5a607d`

The bundled PNGs are crops of rendered flag illustrations, not reproductions of the manual pages. The source artwork is raster, so large-screen sharpness is limited by that source resolution. Country codes and asset hashes are recorded in `Assets/vertical-reference.json`.

## Three-letter code corrections

| Country | Previous | IJF reference |
| --- | --- | --- |
| Faroe Islands | FAR | FRO |
| French Polynesia | FPO | PYF |
| Guadeloupe | GUD | GLP |
| Lebanon | LIB | LBN |
| Marshall Islands | MSH | MHL |
| Montenegro | MGO | MNE |
| New Caledonia | NCD | NCL |
| Norfolk Island | NFI | NFK |
| Northern Mariana Islands | NMA | NMI |

## Covered country entries

| Code | Country | Reference page |
| --- | --- | --- |
| AFG | Afghanistan | 17 |
| ALB | Albania | 17 |
| ALG | Algeria | 17 |
| ASA | American Samoa | 17 |
| AND | Andorra | 18 |
| ANG | Angola | 18 |
| ARG | Argentina | 18 |
| ARM | Armenia | 18 |
| ARU | Aruba | 19 |
| AUS | Australia | 19 |
| AUT | Austria | 19 |
| AZE | Azerbaijan | 19 |
| BAH | Bahamas | 20 |
| BRN | Bahrain | 20 |
| BAN | Bangladesh | 20 |
| BAR | Barbados | 20 |
| BLR | Belarus | 21 |
| BEL | Belgium | 21 |
| BIZ | Belize | 21 |
| BEN | Benin | 21 |
| BHU | Bhutan | 22 |
| BOL | Bolivia | 22 |
| BIH | Bosnia and Herzegovina | 22 |
| BOT | Botswana | 22 |
| BRA | Brazil | 23 |
| BRU | Brunei | 23 |
| BUL | Bulgaria | 23 |
| BUR | Burkina Faso | 23 |
| BDI | Burundi | 24 |
| CAM | Cambodia | 24 |
| CMR | Cameroon | 24 |
| CAN | Canada | 24 |
| CPV | Cape Verde | 25 |
| CAY | Cayman Islands | 25 |
| CAF | Central African Republic | 25 |
| CHA | Chad | 25 |
| CHI | Chile | 26 |
| TPE | Chinese Taipei | 26 |
| COL | Colombia | 26 |
| COM | Comoros | 26 |
| CGO | Congo | 27 |
| COK | Cook Islands | 27 |
| CRC | Costa Rica | 27 |
| CIV | Côte d'Ivoire | 27 |
| CRO | Croatia | 28 |
| CUB | Cuba | 28 |
| CUW | Curaçao | 28 |
| CYP | Cyprus | 28 |
| CZE | Czechia | 29 |
| PRK | North Korea | 29 |
| COD | DR Congo | 29 |
| DEN | Denmark | 29 |
| DJI | Djibouti | 30 |
| DOM | Dominican Republic | 30 |
| ECU | Ecuador | 30 |
| EGY | Egypt | 30 |
| ESA | El Salvador | 31 |
| GEQ | Equatorial Guinea | 31 |
| EST | Estonia | 31 |
| SWZ | Kingdom of Eswatini | 31 |
| ETH | Ethiopia | 32 |
| FRO | Faroe Islands | 32 |
| FIJ | Fiji | 32 |
| FIN | Finland | 32 |
| FRA | France | 33 |
| PYF | French Polynesia | 33 |
| GAB | Gabon | 33 |
| GAM | Gambia | 33 |
| GEO | Georgia | 34 |
| GER | Germany | 34 |
| GHA | Ghana | 34 |
| GBR | Great Britain | 34 |
| GRE | Greece | 35 |
| GLP | Guadeloupe | 35 |
| GUM | Guam | 35 |
| GUA | Guatemala | 35 |
| GUI | Guinea | 36 |
| GBS | Guinea-Bissau | 36 |
| GUY | Guyana | 36 |
| HAI | Haiti | 36 |
| HON | Honduras | 37 |
| HKG | Hong Kong | 37 |
| HUN | Hungary | 37 |
| ISL | Iceland | 37 |
| IND | India | 38 |
| INA | Indonesia | 38 |
| IRQ | Iraq | 38 |
| IRL | Ireland | 38 |
| IRI | Iran | 39 |
| ISR | Israel | 39 |
| ITA | Italy | 39 |
| JAM | Jamaica | 39 |
| JPN | Japan | 40 |
| JOR | Jordan | 40 |
| KAZ | Kazakhstan | 40 |
| KEN | Kenya | 40 |
| KIR | Kiribati | 41 |
| KOS | Kosovo | 41 |
| KUW | Kuwait | 41 |
| KGZ | Kyrgyzstan | 42 |
| LAO | Laos | 42 |
| LAT | Latvia | 42 |
| LBN | Lebanon | 42 |
| LES | Lesotho | 43 |
| LBR | Liberia | 43 |
| LBA | Libya | 43 |
| LIE | Liechtenstein | 43 |
| LTU | Lithuania | 44 |
| LUX | Luxembourg | 44 |
| MAC | Macao | 44 |
| MAD | Madagascar | 44 |
| MAW | Malawi | 45 |
| MAS | Malaysia | 45 |
| MLI | Mali | 45 |
| MLT | Malta | 45 |
| MHL | Marshall Islands | 46 |
| MTN | Mauritania | 46 |
| MRI | Mauritius | 46 |
| MEX | Mexico | 46 |
| MON | Monaco | 47 |
| MGL | Mongolia | 47 |
| MNE | Montenegro | 47 |
| MAR | Morocco | 47 |
| MOZ | Mozambique | 48 |
| MYA | Myanmar | 48 |
| NAM | Namibia | 48 |
| NRU | Nauru | 48 |
| NEP | Nepal | 49 |
| NED | Netherlands | 49 |
| NCL | New Caledonia | 49 |
| NZL | New Zealand | 50 |
| NCA | Nicaragua | 50 |
| NIG | Niger | 50 |
| NGR | Nigeria | 50 |
| NIU | Niue | 51 |
| NFK | Norfolk Island | 51 |
| MKD | North Macedonia | 51 |
| NMI | Northern Mariana Islands | 51 |
| NOR | Norway | 52 |
| PAK | Pakistan | 52 |
| PLW | Palau | 52 |
| PLE | Palestine | 52 |
| PAN | Panama | 53 |
| PNG | Papua New Guinea | 53 |
| PAR | Paraguay | 53 |
| CHN | China (People's Republic of China) | 53 |
| PER | Peru | 54 |
| PHI | Philippines | 54 |
| POL | Poland | 54 |
| POR | Portugal | 54 |
| PUR | Puerto Rico | 55 |
| QAT | Qatar | 55 |
| KOR | South Korea | 55 |
| MDA | Moldova | 55 |
| REU | Réunion | 56 |
| ROU | Romania | 56 |
| RUS | Russia | 56 |
| RWA | Rwanda | 56 |
| LCA | Saint Lucia | 57 |
| SAM | Samoa | 57 |
| SMR | San Marino | 57 |
| STP | Sao Tome and Principe | 57 |
| KSA | Saudi Arabia | 58 |
| SEN | Senegal | 58 |
| SRB | Serbia | 58 |
| SEY | Seychelles | 58 |
| SLE | Sierra Leone | 59 |
| SIN | Singapore | 59 |
| SXM | Sint Maarten (Dutch part) | 59 |
| SVK | Slovakia | 59 |
| SLO | Slovenia | 60 |
| SOL | Solomon Islands | 60 |
| SOM | Somalia | 60 |
| RSA | South Africa | 60 |
| SSD | South Sudan | 61 |
| ESP | Spain | 61 |
| SRI | Sri Lanka | 61 |
| SUD | Sudan | 61 |
| SUR | Suriname | 62 |
| SWE | Sweden | 62 |
| SUI | Switzerland | 62 |
| SYR | Syria | 62 |
| TJK | Tajikistan | 63 |
| THA | Thailand | 63 |
| TLS | Timor-Leste | 63 |
| TOG | Togo | 63 |
| TGA | Tonga | 64 |
| TTO | Trinidad and Tobago | 64 |
| TUN | Tunisia | 64 |
| TUR | Türkiye | 64 |
| TKM | Turkmenistan | 65 |
| UGA | Uganda | 65 |
| UKR | Ukraine | 65 |
| UAE | United Arab Emirates | 65 |
| TAN | Tanzania | 66 |
| USA | United States | 66 |
| URU | Uruguay | 66 |
| UZB | Uzbekistan | 66 |
| VAN | Vanuatu | 67 |
| VEN | Venezuela | 67 |
| VIE | Vietnam | 67 |
| ISV | Virgin Islands, U.S. | 67 |
| YEM | Yemen | 68 |
| ZAM | Zambia | 68 |
| ZIM | Zimbabwe | 68 |

## Entries not covered by this manual

| Code | Country |
| --- | --- |
| AIA | Anguilla |
| ATA | Antarctica |
| ANT | Antigua and Barbuda |
| BER | Bermuda |
| BVT | Bouvet Island |
| IOT | British Indian Ocean Territory |
| AHO | Caribbean Netherlands |
| CXR | Christmas Island |
| CCK | Cocos (Keeling) Islands |
| DMA | Dominica |
| ENG | England |
| ERI | Eritrea |
| EUR | Europe |
| FLK | Falkland Islands (Malvinas) |
| FGU | French Guiana |
| ATF | French Southern Territories |
| GIB | Gibraltar |
| GRL | Greenland |
| GRN | Grenada |
| GGY | Guernsey |
| HMD | Heard Island and McDonald Islands |
| VAT | Holy See (Vatican City State) |
| IMN | Isle of Man |
| JEY | Jersey |
| MDV | Maldives |
| MRT | Martinique |
| MAY | Mayotte |
| FSM | Micronesia |
| MNT | Montserrat |
| NIR | Northern Ireland |
| OMA | Oman |
| PCN | Pitcairn |
| BLM | Saint Barthélemy |
| HEL | Saint Helena, Ascension and Tristan da Cunha |
| SKN | Saint Kitts and Nevis |
| MAF | Saint Martin |
| SPM | Saint Pierre and Miquelon |
| VIN | Saint Vincent and the Grenadines |
| SCO | Scotland |
| SGS | South Georgia and the South Sandwich Islands |
| SJM | Svalbard and Jan Mayen Islands |
| TKL | Tokelau |
| TKS | Turks and Caicos Islands |
| TUV | Tuvalu |
| UMI | US Minor Outlying Islands |
| IVB | Virgin Islands, British |
| WAL | Wales |
| WAF | Wallis and Futuna Islands |
| ESH | Western Sahara |
| ALA | Åland Islands |
