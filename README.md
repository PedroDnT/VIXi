# VIXi (work in progress)
Notebook Study on trying to replicate the VIX Index methodology for B3(rip BVSP)

## Obs: 
- If you have problem downloading the raw files contact me and I'll send you
- Feel free to reach me if you have any ideas/coments
- Something broke the original VIX file and I am writing it again

## Downloading and parsing data
F+iles Download: [BMFBOV - COTACOES HISTORICAS](http://www.bmfbovespa.com.br/pt_br/servicos/market-data/historico/mercado-a-vista/cotacoes-historicas/)
Historical txt series with all transactions on B3. 

## B3_Reader.py 
Contais functions to parse txt files into more human friendly tables: 

```
x = parse_dataset( filepath )  # Loads dataset into pandas dataframe
translate_bdi(x)  # Translates BDI Codes and returns pandas df mofied
market_type(x)  # Translates market_types Codes and returns pandas df mofied
price_mod(x)  # Returns price fields formated as currency
```
More detailed explanation on the other [repository](https://github.com/PedroDnT/B3)  

### Usage
The notebook cruncher.ipynb uses the above functions to group tables and select only info relevant to calculate the VIX. 
The actual VIX function is still under development. 

*is us who fly dog*

## Authors
* **Pedro Todescan** - *GitHub Profile* - [PedroDnT](https://github.com/PedroDnT)

## License
This project is licensed under the Apache License 2.0 - see the [LICENSE.md](LICENSE.md) file for details
