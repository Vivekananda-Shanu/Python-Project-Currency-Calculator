# Python-Project-Currency-Calculator
This is a currency calculator that can convert any amount given in INR and turn it into any currency of your choice 

Main Code -
with open('CurrencyDATA.txt') as f:
	lines = f.readlines()

currencyDict = {}
for line in lines:
	parsed = line.split("\t")
	currencyDict[parsed[0]] = parsed[-1]

amount = int(input("Enter amount:\n"))
print("Enter the name of the currency you want to convert this amount to? Available Options:\n")
[print(item) for item in currencyDict.keys()]
currency = input("Please enter one of these values: \n")


Currency File -
Argentine Peso	1.115338	0.896589
Australian Dollar	0.017966	55.660476
Bahraini Dinar	0.005109	195.726140
Botswana Pula	0.149039	6.709659
Brazilian Real	0.068308	14.639623
British Pound	0.010200	98.042160
Bruneian Dollar	0.018113	55.210090
Bulgarian Lev	0.021856	45.754931
Canadian Dollar	0.017286	57.849228
Chilean Peso	9.984351	0.100157
Chinese Yuan Renminbi	0.088853	11.254577
Colombian Peso	46.472740	0.021518
Croatian Kuna	0.084281	11.865041
Czech Koruna	0.294208	3.398959
Danish Krone	0.083171	12.023476
Emirati Dirham	0.049903	20.038946
Euro	0.011175	89.488866
Hong Kong Dollar	0.105329	9.494061
Hungarian Forint	3.954032	0.252906
Icelandic Krona	1.728425	0.578561
Indonesian Rupiah	191.655288	0.005218
Iranian Rial	568.665341	0.001759
Israeli Shekel	0.044178	22.635679
Japanese Yen	1.413723	0.707352
Kazakhstani Tenge	5.696617	0.175543
Kuwaiti Dinar	0.004145	241.232117
Libyan Dinar	0.018288	54.679837
Malaysian Ringgit	0.054995	18.183521
Mauritian Rupee	0.537754	1.859587
Mexican Peso	0.271623	3.681572
Nepalese Rupee	1.607500	0.622084
New Zealand Dollar	0.019132	52.267460
Norwegian Krone	0.118981	8.404735
Omani Rial	0.005225	191.399294
Pakistani Rupee	2.173161	0.460159
Philippine Peso	0.653161	1.531016
Polish Zloty	0.049474	20.212818
Qatari Riyal	0.049461	20.217865
Romanian New Leu	0.054403	18.381264
Russian Ruble	0.993034	1.007015
Saudi Arabian Riyal	0.050956	19.624808
Singapore Dollar	0.018113	55.210090
South African Rand	0.204165	4.897995
South Korean Won	14.810964	0.067518
Sri Lankan Rupee	2.529038	0.395407
Swedish Krona	0.114455	8.737087
Swiss Franc	0.012034	83.097635
Taiwan New Dollar	0.382560	2.613972
Thai Baht	0.407954	2.451255
Trinidadian Dollar	0.092336	10.830042
Turkish Lira	0.107358	9.314632
US Dollar	0.013588	73.593029
Venezuelan Bolivar	0.135713	7.368513
