# Offline anthem library — 0.10

Reviewed and retrieved on 27 October 2026.

## Coverage

The application includes **146 instrumental recordings** for its 255-entry country/delegation catalog. **109 entries have no bundled recording**. Missing countries remain selectable for local MP3/WAV imports; the app never substitutes another country's anthem. A no-gold ceremony has no automatic anthem.

Acquisition: **93 source-matched mirror downloads**, **6 local conversions from original audio**, **1 archived original Navy recording**, and **46 Commons MP3 downloads**. `Assets/Anthems/catalog.json` contains original page URLs, download/mirror URLs, performer, licensing metadata and SHA-256 for each file. Original audio hashes are retained for local conversions. The public-domain mirror index is an acquisition source; its country assignments were reviewed rather than accepted automatically.

The original Commons file metadata identifies public-domain U.S. Navy Band performances. Individual source pages retain the composition and performance rights information. The UWW archive is not bundled. These recordings are references and are not labelled as IJF-approved or event-approved. No musical arrangement, duration or event eligibility is inferred from the app's flag audit. Confirm the chosen event recording by listening before the ceremony.

## Corrected and withheld mappings

| Discovery issue | Resolution |
| --- | --- |
| USA entry pointed to a Hungarian anthem | Reject that audio. Use the instrumental Star-Spangled Banner from the original Navy source archived in 2004 and linked on its Commons file page. |
| Oman entry pointed to Desteapta-te, romane! | Assign the Romanian source to ROU. OMA has no bundled recording. |
| Dominica entry pointed to the Dominican Republic anthem | Keep that source with DOM and obtain a separate, correctly identified Dominica recording for DMA. |
| Historical or context-sensitive candidates for AFG, SYR and MTN | Leave these entries without a bundled recording pending confirmation of the required current event version. |

## Validation

Every bundled file was fully decoded with FFmpeg; duration and non-silent signal were checked. Mirrored file durations were also compared with their source index. The Windows test host separately opens each recording in the actual WPF audio decoder, checks its duration, validates every SHA-256 and exercises local MP3/WAV playback and the operator controls with volume zero. These checks detect corrupt, incomplete or silent files; they do not replace listening to verify the musical version required by an organiser.

## Included recordings

| Code | Country | Duration | Acquisition | Original recording source |
| --- | --- | ---: | --- | --- |
| ALB | Albania | 1:06 | Commons MP3 | [Recording page](https://commons.wikimedia.org/wiki/File:Hymni_i_Flamurit_instrumental.ogg) |
| ALG | Algeria | 1:18 | Commons MP3 | [Recording page](https://commons.wikimedia.org/wiki/File:Algerian_national_anthem,_performed_by_the_United_States_Navy_Band.flac) |
| ANG | Angola | 2:05 | Commons MP3 | [Recording page](https://commons.wikimedia.org/wiki/File:Independ%C3%AAncia_total_%28instrumental%29.ogg) |
| ANT | Antigua and Barbuda | 1:01 | Commons MP3 | [Recording page](https://commons.wikimedia.org/wiki/File:Antigua_and_Barbuda_National_Anthem.ogg) |
| ARG | Argentina | 3:33 | Commons MP3 | [Recording page](https://commons.wikimedia.org/wiki/File:Himno_Nacional_Argentino_instrumental.ogg) |
| ARM | Armenia | 0:28 | Commons MP3 | [Recording page](https://commons.wikimedia.org/wiki/File:Mer_Hayrenik_instrumental.ogg) |
| ARU | Aruba | 2:07 | Commons MP3 | [Recording page](https://commons.wikimedia.org/wiki/File:Aruba_Dushi_Tera_instrumental.ogg) |
| AUS | Australia | 0:54 | Commons MP3 | [Recording page](https://commons.wikimedia.org/wiki/File:U.S._Navy_Band,_Advance_Australia_Fair_%28instrumental%29.ogg) |
| AUT | Austria | 1:30 | Commons MP3 | [Recording page](https://commons.wikimedia.org/wiki/File:Land_der_Berge_Land_am_Strome_instrumental.ogg) |
| AZE | Azerbaijan | 2:12 | Commons MP3 | [Recording page](https://commons.wikimedia.org/wiki/File:National_Anthem_of_the_Republic_of_Azerbaijan_instrumental.ogg) |
| BAH | Bahamas | 1:15 | Commons MP3 | [Recording page](https://commons.wikimedia.org/wiki/File:March_On_Bahamaland_instrumental.ogg) |
| BAN | Bangladesh | 2:15 | Commons MP3 | [Recording page](https://commons.wikimedia.org/wiki/File:Amar_Sonar_Bangla_instrumental_by_US_Navy_Band.oga) |
| BAR | Barbados | 1:19 | Commons MP3 | [Recording page](https://commons.wikimedia.org/wiki/File:United_States_Navy_Band_-_In_Plenty_and_In_Time_of_Need.ogg) |
| BEL | Belgium | 1:03 | Commons MP3 | [Recording page](https://commons.wikimedia.org/wiki/File:La_Braban%C3%A7onne.oga) |
| BEN | Benin | 1:08 | Commons MP3 | [Recording page](https://commons.wikimedia.org/wiki/File:L%27Aube_Nouvelle.ogg) |
| BIZ | Belize | 2:42 | Commons MP3 | [Recording page](https://commons.wikimedia.org/wiki/File:Land_of_the_Free_instrumental.ogg) |
| BLR | Belarus | 1:56 | Commons MP3 | [Recording page](https://commons.wikimedia.org/wiki/File:My_Belarusy.ogg) |
| BOL | Bolivia | 1:41 | Commons MP3 | [Recording page](https://commons.wikimedia.org/wiki/File:Himno_Nacional_de_Bolivia_instrumental.ogg) |
| BOT | Botswana | 0:57 | Commons MP3 | [Recording page](https://commons.wikimedia.org/wiki/File:United_States_Navy_Band_-_Fatshe_leno_la_rona.ogg) |
| BRA | Brazil | 1:53 | Commons MP3 | [Recording page](https://commons.wikimedia.org/wiki/File:Hino_Nacional_Brasileiro_instrumental.ogg) |
| BRN | Bahrain | 0:49 | Commons MP3 | [Recording page](https://commons.wikimedia.org/wiki/File:Bahraini_Anthem.ogg) |
| BRU | Brunei | 1:03 | Commons MP3 | [Recording page](https://commons.wikimedia.org/wiki/File:Brunei_anthem.ogg) |
| BUL | Bulgaria | 2:01 | Commons MP3 | [Recording page](https://commons.wikimedia.org/wiki/File:Mila_Rodino_instrumental.ogg) |
| BUR | Burkina Faso | 1:47 | Commons MP3 | [Recording page](https://commons.wikimedia.org/wiki/File:National_anthem_of_Burkina_Faso.oga) |
| CAN | Canada | 1:19 | Commons MP3 | [Recording page](https://commons.wikimedia.org/wiki/File:United_States_Navy_Band_-_O_Canada.ogg) |
| CGO | Congo | 1:15 | Commons MP3 | [Recording page](https://commons.wikimedia.org/wiki/File:National_anthem_of_the_Republic_of_the_Congo.oga) |
| CHA | Chad | 1:01 | Commons MP3 | [Recording page](https://commons.wikimedia.org/wiki/File:Chadian_national_anthem,_performed_by_the_United_States_Navy_Band.flac) |
| CHI | Chile | 2:02 | Commons MP3 | [Recording page](https://commons.wikimedia.org/wiki/File:United_States_Navy_Band_-_National_Anthem_of_Chile.ogg) |
| CHN | China (People's Republic of China) | 0:44 | Commons MP3 | [Recording page](https://commons.wikimedia.org/wiki/File:March_of_the_Volunteers_instrumental.ogg) |
| COK | Cook Islands | 1:06 | Commons MP3 | [Recording page](https://commons.wikimedia.org/wiki/File:National_Anthem_of_the_Cook_Islands.ogg) |
| COL | Colombia | 2:41 | Commons MP3 | [Recording page](https://commons.wikimedia.org/wiki/File:United_States_Navy_Band_-_%C2%A1Oh,_gloria_inmarcesible!.ogg) |
| COM | Comoros | 1:37 | Commons MP3 | [Recording page](https://commons.wikimedia.org/wiki/File:National_anthem_of_the_Comoros,_performed_by_the_U.S._Navy_Band.oga) |
| CPV | Cape Verde | 1:11 | Commons MP3 | [Recording page](https://commons.wikimedia.org/wiki/File:C%C3%A2ntico_da_Liberdade_%28instrumental%29.ogg) |
| CRC | Costa Rica | 1:50 | Commons MP3 | [Recording page](https://commons.wikimedia.org/wiki/File:Costa_Rica_National_Anthem.ogg) |
| CRO | Croatia | 1:57 | Commons MP3 | [Recording page](https://commons.wikimedia.org/wiki/File:Lijepa_nasa_domovino_instrumental_cijeli.ogg) |
| CUB | Cuba | 1:10 | Commons MP3 | [Recording page](https://commons.wikimedia.org/wiki/File:United_States_Navy_Band_-_La_Bayamesa.ogg) |
| CZE | Czechia | 1:05 | Commons MP3 | [Recording page](https://commons.wikimedia.org/wiki/File:Kde_domov_m%C5%AFj.ogg) |
| DEN | Denmark | 1:19 | Commons MP3 | [Recording page](https://commons.wikimedia.org/wiki/File:United_States_Navy_Band_-_Der_er_et_yndigt_land.ogg) |
| DJI | Djibouti | 0:48 | Commons MP3 | [Recording page](https://commons.wikimedia.org/wiki/File:The_Djiboutian_anthem.ogg) |
| DMA | Dominica | 0:49 | Commons MP3 | [Recording page](https://commons.wikimedia.org/wiki/File:National_Anthem_of_Dominica_by_US_Navy_Band.ogg) |
| DOM | Dominican Republic | 1:37 | Commons MP3 | [Recording page](https://commons.wikimedia.org/wiki/File:Dominican_Republic_National_Anthem.ogg) |
| ECU | Ecuador | 3:19 | Commons MP3 | [Recording page](https://commons.wikimedia.org/wiki/File:Anthem_of_Ecuador.ogg) |
| EGY | Egypt | 1:26 | Commons MP3 | [Recording page](https://commons.wikimedia.org/wiki/File:Bilady,_Bilady,_Bilady.ogg) |
| ERI | Eritrea | 1:59 | Commons MP3 | [Recording page](https://commons.wikimedia.org/wiki/File:Eritrean_national_anthem,_performed_by_the_U.S._Navy_Band.wav) |
| ESA | El Salvador | 4:14 | Source-matched mirror | [Recording page](https://commons.wikimedia.org/wiki/File:El_Salvador_National_Anthem.ogg) |
| ESP | Spain | 1:02 | Original converted locally | [Recording page](https://commons.wikimedia.org/wiki/File:Marcha_Real-Royal_March_by_US_Navy_Band.ogg) |
| EST | Estonia | 0:32 | Source-matched mirror | [Recording page](https://commons.wikimedia.org/wiki/File:US_Navy_band_-_National_anthem_of_Estonia.ogg) |
| FIJ | Fiji | 1:26 | Source-matched mirror | [Recording page](https://commons.wikimedia.org/wiki/File:Fiji_National_Anthem.ogg) |
| FRA | France | 1:19 | Original converted locally | [Recording page](https://commons.wikimedia.org/wiki/File:La_Marseillaise.ogg) |
| FSM | Micronesia | 1:59 | Source-matched mirror | [Recording page](https://commons.wikimedia.org/wiki/File:Full_performance_of_the_Micronesian_national_anthem_by_the_U.S._Navy_Band.flac) |
| GAB | Gabon | 1:39 | Source-matched mirror | [Recording page](https://commons.wikimedia.org/wiki/File:La_Concorde.ogg) |
| GAM | Gambia | 1:15 | Source-matched mirror | [Recording page](https://commons.wikimedia.org/wiki/File:For_The_Gambia_Our_Homeland_%28instrumental%29.ogg) |
| GBR | Great Britain | 0:50 | Source-matched mirror | [Recording page](https://commons.wikimedia.org/wiki/File:U.S._Navy_Band_-_God_Save_the_King.oga) |
| GEO | Georgia | 1:26 | Original converted locally | [Recording page](https://commons.wikimedia.org/wiki/File:Georgian_national_anthem.oga) |
| GEQ | Equatorial Guinea | 1:52 | Source-matched mirror | [Recording page](https://commons.wikimedia.org/wiki/File:Equatorial_Guinea%27s_national_anthem,_performed_by_the_United_States_Navy_Band.oga) |
| GER | Germany | 1:14 | Original converted locally | [Recording page](https://commons.wikimedia.org/wiki/File:German_national_anthem_performed_by_the_US_Navy_Band.ogg) |
| GHA | Ghana | 0:52 | Source-matched mirror | [Recording page](https://commons.wikimedia.org/wiki/File:National_Anthem_of_Ghana.ogg) |
| GRE | Greece | 0:45 | Source-matched mirror | [Recording page](https://commons.wikimedia.org/wiki/File:Hymn_to_liberty_instrumental.oga) |
| GUI | Guinea | 1:12 | Source-matched mirror | [Recording page](https://commons.wikimedia.org/wiki/File:Libert%C3%A9.oga) |
| GUY | Guyana | 0:53 | Source-matched mirror | [Recording page](https://commons.wikimedia.org/wiki/File:National_Anthem_of_Guyana.ogg) |
| HAI | Haiti | 0:37 | Source-matched mirror | [Recording page](https://commons.wikimedia.org/wiki/File:Haiti_National_Anthem.ogg) |
| HON | Honduras | 2:46 | Source-matched mirror | [Recording page](https://commons.wikimedia.org/wiki/File:Honduras_National_Anthem.ogg) |
| HUN | Hungary | 1:33 | Source-matched mirror | [Recording page](https://commons.wikimedia.org/wiki/File:Hu-magyarhimnusz.ogg) |
| INA | Indonesia | 1:49 | Source-matched mirror | [Recording page](https://commons.wikimedia.org/wiki/File:Indonesia_Raya_instrumental.ogg) |
| IND | India | 1:03 | Source-matched mirror | [Recording page](https://commons.wikimedia.org/wiki/File:Jana_Gana_Mana_instrumental.ogg) |
| IRL | Ireland | 0:58 | Source-matched mirror | [Recording page](https://commons.wikimedia.org/wiki/File:Irish_national_anthem,_performed_by_the_United_States_Navy_Band.wav) |
| IRQ | Iraq | 1:43 | Source-matched mirror | [Recording page](https://commons.wikimedia.org/wiki/File:Iraqi_national_anthem,_performed_by_the_U.S._Navy_Band.wav) |
| ISL | Iceland | 1:39 | Source-matched mirror | [Recording page](https://commons.wikimedia.org/wiki/File:Lofs%C3%B6ngur.ogg) |
| ISR | Israel | 1:14 | Source-matched mirror | [Recording page](https://commons.wikimedia.org/wiki/File:Hatikvah_instrumental.ogg) |
| ITA | Italy | 1:39 | Source-matched mirror | [Recording page](https://commons.wikimedia.org/wiki/File:National_anthem_of_Italy_-_U.S._Navy_Band_%28long_version%29.ogg) |
| JAM | Jamaica | 1:19 | Source-matched mirror | [Recording page](https://commons.wikimedia.org/wiki/File:%22Jamaica,_Land_We_Love%22,_performed_by_the_United_States_Navy_Band.oga) |
| JOR | Jordan | 0:36 | Source-matched mirror | [Recording page](https://commons.wikimedia.org/wiki/File:National_anthem_of_Jordan_instrumental.ogg) |
| JPN | Japan | 0:59 | Original converted locally | [Recording page](https://commons.wikimedia.org/wiki/File:Kimi_ga_Yo_instrumental.ogg) |
| KAZ | Kazakhstan | 1:39 | Source-matched mirror | [Recording page](https://commons.wikimedia.org/wiki/File:National_anthem_of_Kazakhstan,_performed_by_the_United_States_Navy_Band.wav) |
| KEN | Kenya | 1:52 | Source-matched mirror | [Recording page](https://commons.wikimedia.org/wiki/File:National_anthem_of_Kenya,_performed_by_the_United_States_Navy_Band.flac) |
| KGZ | Kyrgyzstan | 2:03 | Original converted locally | [Recording page](https://commons.wikimedia.org/wiki/File:National_Anthem_of_Kyrgyzstan.ogg) |
| KOR | South Korea | 0:57 | Source-matched mirror | [Recording page](https://commons.wikimedia.org/wiki/File:National_anthem_of_South_Korea,_performed_by_the_United_States_Navy_Band.wav) |
| KOS | Kosovo | 0:56 | Source-matched mirror | [Recording page](https://commons.wikimedia.org/wiki/File:National_Anthem_of_the_Republic_of_Kosovo.ogg) |
| KSA | Saudi Arabia | 0:50 | Source-matched mirror | [Recording page](https://commons.wikimedia.org/wiki/File:Saudi_Arabian_national_anthem,_performed_by_the_United_States_Navy_Band.wav) |
| KUW | Kuwait | 0:34 | Source-matched mirror | [Recording page](https://commons.wikimedia.org/wiki/File:National_anthem_of_Kuwait_%28instrumental%29.ogg) |
| LAO | Laos | 0:50 | Source-matched mirror | [Recording page](https://commons.wikimedia.org/wiki/File:National_Anthem_of_Laos.ogg) |
| LBA | Libya | 1:07 | Source-matched mirror | [Recording page](https://commons.wikimedia.org/wiki/File:Libya,_Libya,_Libya_instrumental.ogg) |
| LBN | Lebanon | 0:50 | Source-matched mirror | [Recording page](https://commons.wikimedia.org/wiki/File:Lebanese_national_anthem.ogg) |
| LBR | Liberia | 1:20 | Source-matched mirror | [Recording page](https://commons.wikimedia.org/wiki/File:Liberia_National_Anthem.ogg) |
| LCA | Saint Lucia | 0:41 | Source-matched mirror | [Recording page](https://commons.wikimedia.org/wiki/File:National_Anthem_of_Saint_Lucia.ogg) |
| LES | Lesotho | 0:42 | Source-matched mirror | [Recording page](https://commons.wikimedia.org/wiki/File:National_anthem_of_Lesotho,_performed_by_the_U.S._Navy_Band.flac) |
| LIE | Liechtenstein | 1:24 | Source-matched mirror | [Recording page](https://commons.wikimedia.org/wiki/File:Oben_am_jungen_Rhein,_by_the_U.S._Navy_Band.ogg) |
| LUX | Luxembourg | 1:23 | Source-matched mirror | [Recording page](https://commons.wikimedia.org/wiki/File:Luxembourg_National_Anthem.ogg) |
| MAD | Madagascar | 1:02 | Source-matched mirror | [Recording page](https://commons.wikimedia.org/wiki/File:Ry_Tanindrazanay_malala_%C3%B4!_%28instrumental%29.ogg) |
| MAR | Morocco | 1:00 | Source-matched mirror | [Recording page](https://commons.wikimedia.org/wiki/File:National_Anthem_of_Morocco.ogg) |
| MAS | Malaysia | 0:59 | Source-matched mirror | [Recording page](https://commons.wikimedia.org/wiki/File:Negaraku_instrumental.ogg) |
| MAW | Malawi | 0:51 | Source-matched mirror | [Recording page](https://commons.wikimedia.org/wiki/File:Malawian_national_anthem.oga) |
| MDA | Moldova | 1:10 | Source-matched mirror | [Recording page](https://commons.wikimedia.org/wiki/File:Imnul_Republicii_Moldova_US_NAVY.ogg) |
| MDV | Maldives | 1:08 | Source-matched mirror | [Recording page](https://commons.wikimedia.org/wiki/File:Gaumii_salaam.ogg) |
| MEX | Mexico | 1:41 | Source-matched mirror | [Recording page](https://commons.wikimedia.org/wiki/File:Himno_Nacional_Mexicano_instrumental.ogg) |
| MHL | Marshall Islands | 2:17 | Source-matched mirror | [Recording page](https://commons.wikimedia.org/wiki/File:National_anthem_of_Marshall_Islands.wav) |
| MLI | Mali | 1:18 | Source-matched mirror | [Recording page](https://commons.wikimedia.org/wiki/File:Malian_national_anthem,_performed_by_the_United_States_Navy_Band.wav) |
| MLT | Malta | 0:49 | Source-matched mirror | [Recording page](https://commons.wikimedia.org/wiki/File:Malta_National_Anthem.ogg) |
| MNE | Montenegro | 2:04 | Source-matched mirror | [Recording page](https://commons.wikimedia.org/wiki/File:National_Anthem_of_Montenegro.ogg) |
| MON | Monaco | 1:18 | Source-matched mirror | [Recording page](https://commons.wikimedia.org/wiki/File:Monaco_National_Anthem.ogg) |
| MYA | Myanmar | 0:39 | Source-matched mirror | [Recording page](https://commons.wikimedia.org/wiki/File:U.S._Navy_Band_-_Kaba_Ma_Kyei.oga) |
| NCA | Nicaragua | 0:55 | Source-matched mirror | [Recording page](https://commons.wikimedia.org/wiki/File:National_Anthem_of_Nicaragua_by_US_Navy_Band.ogg) |
| NED | Netherlands | 0:48 | Source-matched mirror | [Recording page](https://commons.wikimedia.org/wiki/File:United_States_Navy_Band_-_%22Het_Wilhelmus%22.wav) |
| NEP | Nepal | 1:09 | Source-matched mirror | [Recording page](https://commons.wikimedia.org/wiki/File:Sayaun_Thunga_Phool_Ka_%28instrumental%29.ogg) |
| NOR | Norway | 1:01 | Source-matched mirror | [Recording page](https://commons.wikimedia.org/wiki/File:Norway_%28National_Anthem%29.ogg) |
| NZL | New Zealand | 1:03 | Source-matched mirror | [Recording page](https://commons.wikimedia.org/wiki/File:New_Zealand_national_anthem,_performed_by_the_United_States_Navy_Band.wav) |
| PAK | Pakistan | 1:22 | Source-matched mirror | [Recording page](https://commons.wikimedia.org/wiki/File:Pakistani_national_anthem,_performed_by_the_U.S._Navy_Band.wav) |
| PAN | Panama | 1:50 | Source-matched mirror | [Recording page](https://commons.wikimedia.org/wiki/File:Panama_National_Anthem.ogg) |
| PAR | Paraguay | 3:11 | Source-matched mirror | [Recording page](https://commons.wikimedia.org/wiki/File:Paraguayan_National_Anthem.oga) |
| PER | Peru | 3:09 | Source-matched mirror | [Recording page](https://commons.wikimedia.org/wiki/File:United_States_Navy_Band_-_Marcha_Nacional_del_Per%C3%BA_B%E2%99%AD_major_bpm_90.ogg) |
| PHI | Philippines | 1:01 | Source-matched mirror | [Recording page](https://commons.wikimedia.org/wiki/File:Lupang_Hinirang_instrumental.ogg) |
| PLW | Palau | 0:51 | Source-matched mirror | [Recording page](https://commons.wikimedia.org/wiki/File:Belau_rekid_%28instrumental%29.oga) |
| PNG | Papua New Guinea | 0:51 | Source-matched mirror | [Recording page](https://commons.wikimedia.org/wiki/File:O_Arise,_All_You_Sons_%28instrumental%29.ogg) |
| POL | Poland | 0:42 | Source-matched mirror | [Recording page](https://commons.wikimedia.org/wiki/File:Mazurek_Dabrowskiego.ogg) |
| POR | Portugal | 1:09 | Source-matched mirror | [Recording page](https://commons.wikimedia.org/wiki/File:A_Portuguesa.ogg) |
| QAT | Qatar | 1:26 | Source-matched mirror | [Recording page](https://commons.wikimedia.org/wiki/File:National_anthem_of_Qatar.ogg) |
| ROU | Romania | 2:18 | Source-matched mirror | [Recording page](https://commons.wikimedia.org/wiki/File:Desteapta-te,_romane!.ogg) |
| RSA | South Africa | 2:02 | Source-matched mirror | [Recording page](https://commons.wikimedia.org/wiki/File:South_African_national_anthem.oga) |
| RUS | Russia | 1:08 | Commons MP3 | [Recording page](https://commons.wikimedia.org/wiki/File:National_anthem_of_Russia,_performed_by_the_United_States_Navy_Band.wav) |
| RWA | Rwanda | 2:18 | Source-matched mirror | [Recording page](https://commons.wikimedia.org/wiki/File:Hymne_National_du_Rwanda.ogg) |
| SEN | Senegal | 0:56 | Source-matched mirror | [Recording page](https://commons.wikimedia.org/wiki/File:National_Anthem_of_Senegal.ogg) |
| SEY | Seychelles | 1:06 | Source-matched mirror | [Recording page](https://commons.wikimedia.org/wiki/File:National_anthem_of_Seychelles.wav) |
| SIN | Singapore | 1:18 | Source-matched mirror | [Recording page](https://commons.wikimedia.org/wiki/File:Majulah_Singapura.ogg) |
| SLO | Slovenia | 0:56 | Source-matched mirror | [Recording page](https://commons.wikimedia.org/wiki/File:Slovenia%27s_national_anthem,_performed_by_the_United_States_Navy_Band.oga) |
| SOM | Somalia | 1:05 | Source-matched mirror | [Recording page](https://commons.wikimedia.org/wiki/File:Somali_national_anthem,_performed_by_the_United_States_Navy_Band.oga) |
| SRB | Serbia | 1:44 | Source-matched mirror | [Recording page](https://commons.wikimedia.org/wiki/File:National_anthem_of_Serbia,_performed_by_the_United_States_Navy_Band.wav) |
| SSD | South Sudan | 1:15 | Source-matched mirror | [Recording page](https://commons.wikimedia.org/wiki/File:South_Sudan_Oyee!_%28instrumental%29.ogg) |
| SUD | Sudan | 0:46 | Source-matched mirror | [Recording page](https://commons.wikimedia.org/wiki/File:Sudanese_national_anthem,_performed_by_the_U.S._Navy_Band.oga) |
| SUI | Switzerland | 1:24 | Source-matched mirror | [Recording page](https://commons.wikimedia.org/wiki/File:Swiss_Psalm.ogg) |
| SUR | Suriname | 0:52 | Source-matched mirror | [Recording page](https://commons.wikimedia.org/wiki/File:Surinamese_national_anthem,_performed_by_the_U.S._Navy_Band.ogg) |
| SWE | Sweden | 1:27 | Source-matched mirror | [Recording page](https://commons.wikimedia.org/wiki/File:United_States_Navy_Band_-_Sweden.ogg) |
| SWZ | Kingdom of Eswatini | 1:08 | Source-matched mirror | [Recording page](https://commons.wikimedia.org/wiki/File:Nkulunkulu_Mnikati_wetibusiso_temaSwati_%28instrumental%29.ogg) |
| TAN | Tanzania | 0:51 | Source-matched mirror | [Recording page](https://commons.wikimedia.org/wiki/File:Tanzanian_national_anthem,_performed_by_the_United_States_Navy_Band.oga) |
| THA | Thailand | 0:44 | Source-matched mirror | [Recording page](https://commons.wikimedia.org/wiki/File:Thai_National_Anthem_-_US_Navy_Band.ogg) |
| TJK | Tajikistan | 1:50 | Commons MP3 | [Recording page](https://commons.wikimedia.org/wiki/File:National_anthem_of_Tajikistan,_performed_by_the_U.S._Navy_Band.flac) |
| TKM | Turkmenistan | 1:58 | Source-matched mirror | [Recording page](https://commons.wikimedia.org/wiki/File:National_anthem_of_Turkmenistan,_performed_by_the_United_States_Navy_Band.wav) |
| TLS | Timor-Leste | 2:08 | Source-matched mirror | [Recording page](https://commons.wikimedia.org/wiki/File:East_Timorese_national_anthem.wav) |
| TTO | Trinidad and Tobago | 1:13 | Source-matched mirror | [Recording page](https://commons.wikimedia.org/wiki/File:Forged_from_the_Love_of_Liberty_%28instrumental%29.ogg) |
| TUR | Türkiye | 1:16 | Source-matched mirror | [Recording page](https://commons.wikimedia.org/wiki/File:Istikl%C3%A2l_Marsi_instrumetal.ogg) |
| UAE | United Arab Emirates | 1:26 | Source-matched mirror | [Recording page](https://commons.wikimedia.org/wiki/File:As_Salam_Al_Amiri_instrumental.ogg) |
| UGA | Uganda | 0:43 | Source-matched mirror | [Recording page](https://commons.wikimedia.org/wiki/File:Ugandan_national_anthem,_performed_by_the_U.S._Navy_Band.flac) |
| UKR | Ukraine | 1:19 | Source-matched mirror | [Recording page](https://commons.wikimedia.org/wiki/File:National_anthem_of_Ukraine,_instrumental.oga) |
| URU | Uruguay | 4:30 | Source-matched mirror | [Recording page](https://commons.wikimedia.org/wiki/File:United_States_Navy_Band_-_National_Anthem_of_Uruguay_%28complete%29.ogg) |
| USA | United States | 1:18 | Archived Navy original | [Recording page](https://commons.wikimedia.org/wiki/File%3A%22The_Star-Spangled_Banner%22_performed_by_the_United_States_Navy_Band.mp3) |
| VEN | Venezuela | 1:30 | Source-matched mirror | [Recording page](https://commons.wikimedia.org/wiki/File:United_States_Navy_Band_-_Gloria_al_Bravo_Pueblo.ogg) |
| VIN | Saint Vincent and the Grenadines | 0:51 | Source-matched mirror | [Recording page](https://commons.wikimedia.org/wiki/File:National_anthem_of_Saint_Vincent_and_the_Grenadines,_performed_by_the_United_States_Navy_Band.oga) |

## Entries without a bundled recording

These are gaps in this release's library, not a judgment about event eligibility or whether a national anthem exists. Import a preferred recording for a selected code.

| Code | Catalog name |
| --- | --- |
| AFG | Afghanistan |
| AHO | Caribbean Netherlands |
| AIA | Anguilla |
| ALA | Åland Islands |
| AND | Andorra |
| ASA | American Samoa |
| ATA | Antarctica |
| ATF | French Southern Territories |
| BDI | Burundi |
| BER | Bermuda |
| BHU | Bhutan |
| BIH | Bosnia and Herzegovina |
| BLM | Saint Barthélemy |
| BVT | Bouvet Island |
| CAF | Central African Republic |
| CAM | Cambodia |
| CAY | Cayman Islands |
| CCK | Cocos (Keeling) Islands |
| CIV | Côte d'Ivoire |
| CMR | Cameroon |
| COD | DR Congo |
| CUW | Curaçao |
| CXR | Christmas Island |
| CYP | Cyprus |
| ENG | England |
| ESH | Western Sahara |
| ETH | Ethiopia |
| EUR | Europe |
| FGU | French Guiana |
| FIN | Finland |
| FLK | Falkland Islands (Malvinas) |
| FRO | Faroe Islands |
| GBS | Guinea-Bissau |
| GGY | Guernsey |
| GIB | Gibraltar |
| GLP | Guadeloupe |
| GRL | Greenland |
| GRN | Grenada |
| GUA | Guatemala |
| GUM | Guam |
| HEL | Saint Helena, Ascension and Tristan da Cunha |
| HKG | Hong Kong |
| HMD | Heard Island and McDonald Islands |
| IMN | Isle of Man |
| IOT | British Indian Ocean Territory |
| IRI | Iran |
| ISV | Virgin Islands, U.S. |
| IVB | Virgin Islands, British |
| JEY | Jersey |
| KIR | Kiribati |
| LAT | Latvia |
| LTU | Lithuania |
| MAC | Macao |
| MAF | Saint Martin |
| MAY | Mayotte |
| MGL | Mongolia |
| MKD | North Macedonia |
| MNT | Montserrat |
| MOZ | Mozambique |
| MRI | Mauritius |
| MRT | Martinique |
| MTN | Mauritania |
| NAM | Namibia |
| NCL | New Caledonia |
| NFK | Norfolk Island |
| NGR | Nigeria |
| NIG | Niger |
| NIR | Northern Ireland |
| NIU | Niue |
| NMI | Northern Mariana Islands |
| NRU | Nauru |
| OMA | Oman |
| PCN | Pitcairn |
| PLE | Palestine |
| PRK | North Korea |
| PUR | Puerto Rico |
| PYF | French Polynesia |
| REU | Réunion |
| SAM | Samoa |
| SCO | Scotland |
| SGS | South Georgia and the South Sandwich Islands |
| SJM | Svalbard and Jan Mayen Islands |
| SKN | Saint Kitts and Nevis |
| SLE | Sierra Leone |
| SMR | San Marino |
| SOL | Solomon Islands |
| SPM | Saint Pierre and Miquelon |
| SRI | Sri Lanka |
| STP | Sao Tome and Principe |
| SVK | Slovakia |
| SXM | Sint Maarten (Dutch part) |
| SYR | Syria |
| TGA | Tonga |
| TKL | Tokelau |
| TKS | Turks and Caicos Islands |
| TOG | Togo |
| TPE | Chinese Taipei |
| TUN | Tunisia |
| TUV | Tuvalu |
| UMI | US Minor Outlying Islands |
| UZB | Uzbekistan |
| VAN | Vanuatu |
| VAT | Holy See (Vatican City State) |
| VIE | Vietnam |
| WAF | Wallis and Futuna Islands |
| WAL | Wales |
| YEM | Yemen |
| ZAM | Zambia |
| ZIM | Zimbabwe |

## Updating the library

The reviewed mapping lives in `scripts/anthem-sources.json`. `scripts/import-anthems.py` reads original Commons file metadata and rejects sources without the selected public-domain Navy provenance. `--originals` uses a development-only FFmpeg converter in `.tools/anthem-converter`; `--mirror` uses the cached source metadata and discovery index in `artifacts/anthem-research` and requires an exact original-file identity match. Archive URLs are explicit in the reviewed mapping. These tools do not run in the application. Native tests and full-stream checks must be rerun after replacing audio.
