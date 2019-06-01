# Calendar Effects Scores (CES)

The Calendar Effects Scores (CES) are three measures for the presence and severity of calendar effects - market anomalies linked to calendar time - in stock markets.


## Context

The measures were developed for the Master's Dissertation in Finance, _"The Impact of Financial Development on Stock Market Calendar Effects"_ (Gaspar & Macedo, 2019).


## Methodology

The database contains observations for 46 country stock indices, between 1992 and 2016. The following indices are used for each country:

| Country        	| Index                                   	|
|:----------------|:-----------------------------------------	|
| Argentina      	| MERVAL Index                            	|
| Australia      	| S&P/ASX 300                             	|
| Austria        	| Wiener Börse Index                      	|
| Belgium        	| BEL 20                                  	|
| Brazil         	| Bovespa Index                           	|
| Bulgaria       	| SOFIX                                   	|
| Canada         	| S&P/TSX Composite Index                 	|
| Chile          	| IPSA                                    	|
| China          	| SSE Composite Index                     	|
| Croatia        	| CROBEX                                  	|
| Czech Republic 	| PX-GLOB                                 	|
| Denmark        	| OMX Copenhagen 20                       	|
| Finland        	| OMX Helsinki All-Share Index            	|
| France         	| CAC 40                                  	|
| Germany        	| DAX Composite Index                     	|
| Greece         	| Athens Stock Exchange General Index     	|
| Hong Kong      	| Hang Seng Index                         	|
| India          	| BSE SENSEX                              	|
| Indonesia      	| Jakarta Composite Index                 	|
| Ireland        	| ISEQ All-Share Index                    	|
| Italy          	| FTSE MIB                                	|
| Japan          	| Nikkei 225                              	|
| Lithuania      	| OMX Vilnius                             	|
| Mexico         	| S&P/BMV IPC                             	|
| Morocco        	| Moroccan All-Shares Index               	|
| Netherlands    	| AEX All-Share Index                     	|
| New Zealand    	| NZX 50 Index                            	|
| Nigeria        	| Nigerian Stock Exchange All-Share Index 	|
| Norway         	| Olso Børs All-Share Index               	|
| Peru           	| S&amp;P/BVL Peru General Index          	|
| Philippines    	| PSE Composite Index                     	|
| Poland         	| WIG                                     	|
| Portugal       	| PSI All-Share Index                     	|
| Romania        	| Bucharest Exchange Trading Index        	|
| Russia         	| MOEX Russia Index                       	|
| Singapore      	| FTSE Straits Times Index                	|
| South Africa   	| FTSE/JSE Africa All-Share Index         	|
| South Korea    	| Korea Composite Stock Price Index       	|
| Spain          	| IBEX 35                                 	|
| Sweden         	| OMX Stockholm 30                        	|
| Switzerland    	| Swiss All-Share Index                   	|
| Thailand       	| SET Index                               	|
| Tunisia        	| Tunindex                                	|
| Ukraine        	| PFTS Index                              	|
| United Kingdom 	| FTSE All-Share Index                    	|


### Linear regressions

From the daily returns for each index between the sample period, the coefficients for the following models are estimated, through an OLS regression, per each country and year:

#### Day of the Week effects:
<img src="/Images/dotw.gif" alt="DOTW" height="25"/>
where the coefficients represent, respectively, the Monday and the Friday effects;

#### Month of the Year effects:
<img src="/Images/moty.gif" alt="MOTY" height="25"/>
where the coefficients represent, respectively, the January, April, and December effects;

#### Halloween effect:
<img src="/Images/halloween.gif" alt="Halloween" height="25"/>
where the coefficient represents the Halloween effect.


### CES scores
* CES<sub>A</sub> represents the count of calendar effects for a given country and year that are significant at the 5% level.

* CES<sub>B</sub> represents the average daily absolute anomalous return of calendar effects that are significant at the 5% level for a given country and year.
<p align="center">
<img src="/Images/cesb.gif" alt="CES B" height="50"/>
</p>

* CES<sub>C</sub> represents the average daily absolute anomalous return of all potential calendar effects for a given country and year.
<p align="center">
<img src="/Images/cesc.gif" alt="CES C" height="50"/>
</p>

## Summary statistics

|              	| CES<sub>A</sub> 	| CES<sub>B</sub> 	| CES<sub>C</sub> 	|
|--------------	|----------------:	|----------------:	|----------------:	|
| Min          	| 0               	| 0.00             	| 0.00             	|
| Median       	| 0               	| 0.00             	| 0.00             	|
| Mean         	| 0.42            	| 0.20            	| 0.04            	|
| Max          	| 4               	| 2.70            	| 0.91            	|

<img src="/Images/ces_histogram.png" alt="CES A" height="400"/><img src="/Images/ces_density.png" alt="CES B & CES C" height="400"/>
