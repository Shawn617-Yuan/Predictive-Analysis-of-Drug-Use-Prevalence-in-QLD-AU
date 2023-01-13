Ive just uploaded some sample data to look at. Feel free to add more data from each data source (especially as it becomes relevant)

For the crime data, we can have it broken down into either
- District
- Division
- State
- Region
- LGA (local government area)

For the census data, we can have it broken down into 
- All geographies
- Aus
- State/territory
- Statistical areas
- Greater capital city statistical areas
- LGA
- Suburbs
- Postal Area
- Electoral Division
- Section of state
- etc

Click [here](https://www.abs.gov.au/websitedbs/D3310114.nsf/Home/2016%20DataPacks) to go to a page with explanations on Datapacks from the Bureau of Statistics. This is where we get the census data

Click [here](https://www.police.qld.gov.au/maps-and-statistics) for the crime data

Click [here](https://data.gov.au/dataset/ds-dga-16803f0b-6934-41ae-bf82-d16265784c7f/details?q=QLD%20Boundaries%20-%20Geoscape) for the location data for queensland LGAs


# Structure of the crime data
Described in this document: [Queensland Police Service Annual Statistics Review 2016-17](https://www.police.qld.gov.au/sites/default/files/2019-01/AnnualStatisticalReview_2016-17.pdf)

Exists as
- Category (total)
    - sub-category (count)
    - sub-category (count)

	Department of Industry, Science, Energy and Resources

- 'Division',
- 'Month Year',
- 'Offences Against the Person',
	- 'Homicide (Murder)',
	- 'Other Homicide',
		- 'Attempted Murder',
		- 'Conspiracy to Murder',
		- 'Manslaughter (excl. by driving)',
		- 'Manslaughter Unlawful Striking Causing Death',
		- 'Driving Causing Death',
	- 'Assault',
		- 'Grievous Assault',
		- 'Serious Assault',
		- 'Serious Assault (Other)',
		- 'Common Assault'',
	- 'Sexual Offences',
		- 'Rape and Attempted Rape',
		- 'Other Sexual Offences',
	- 'Robbery',
		- 'Armed Robbery',
		- 'Unarmed Robbery',
	- 'Other Offences Against the Person',
		- 'Kidnapping & Abduction etc.',
		- 'Extortion',
		- 'Stalking',
		- 'Life Endangering Acts',
- 'Offences Against Property',
	- 'Unlawful Entry',
		- 'Unlawful Entry With Intent - Dwelling',
		- 'Unlawful Entry Without Violence - Dwelling',
		- 'Unlawful Entry With Violence - Dwelling',
		- 'Unlawful Entry With Intent - Shop',
		- 'Unlawful Entry With Intent - Other',
	- 'Arson',
	- 'Other Property Damage',
	- 'Unlawful Use of Motor Vehicle',
	- 'Other Theft (excl. Unlawful Entry)',
		- 'Stealing from Dwellings',
		- 'Shop Stealing',
		- 'Vehicles (steal from/enter with intent)',
		- 'Other Stealing',
	- 'Fraud',
		- 'Fraud by Computer',
		- 'Fraud by Cheque',
		- 'Fraud by Credit Card',
		- 'Identity Fraud',
		- 'Other Fraud',
	- 'Handling Stolen Goods',
		- 'Possess Property Suspected Stolen',
		- 'Receiving Stolen Property',
		- 'Possess etc. Tainted Property',
		- 'Other Handling Stolen Goods',
- 'Other Offences''
	- 'Drug Offences',
		- 'Trafficking Drugs',
		- 'Possess Drugs',
		- 'Produce Drugs',
		- 'Sell Supply Drugs',
		- 'Other Drug Offences',
	- 'Prostitution Offences',
		- 'Found in Places Used for Purpose of Prostitution Offences',
		- 'Have Interest in Premises Used for Prostitution Offences',
		- 'Knowingly Participate in Provision Prostitution Offences',
		- 'Public Soliciting',
		- 'Procuring Prostitution',
		- 'Permit Minor to be at a Place Used for Prostitution Offences',
		- 'Advertising Prostitution',
		- 'Other Prostitution Offences',
	- 'Liquor (excl. Drunkenness)',
	- 'Gaming Racing & Betting Offences',
	- 'Breach Domestic Violence Protection Order',
	- 'Trespassing and Vagrancy',
	- 'Weapons Act Offences',
		- 'Unlawful Possess Concealable Firearm',
		- 'Unlawful Possess Firearm - Other',
		- 'Bomb Possess and/or use of',
		- 'Possess and/or use other weapons; restricted items',
		- 'Weapons Act Offences - Other',
	- 'Good Order Offences',
		- 'Disobey Move-on Direction',
		- 'Resist Incite Hinder Obstruct Police',
		- 'Fare Evasion',
		- 'Public Nuisance',
	- 'Stock Related Offences',
	- 'Traffic and Related Offences',
		- 'Dangerous Operation of a Vehicle',
		- 'Drink Driving',
		- 'Disqualified Driving',
		- 'Interfere with Mechanism of Motor Vehicle',
	- 'Miscellaneous Offences',
