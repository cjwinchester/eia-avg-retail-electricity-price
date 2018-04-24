# EIA state-level average retail electricity prices

A Jupyter notebook with some Python to hit the EIA's API for state-level data on monthly average retail electricity prices (all sectors) -- a piece of [Table 5.6.A](https://www.eia.gov/electricity/monthly/epm_table_grapher.php?t=epmt_5_06_a) of the agency's [Electric Power Monthly report](https://www.eia.gov/electricity/monthly/) going back to 2001. (I am 97% it's easier to get this specific data via API than by using one of [the agency's bulk download files](https://www.eia.gov/opendata/bulkfiles.php), but I could be wrong.)

The notebook also adjusts the price data for inflation, as EIA data [are given in nominal dollars](https://www.eia.gov/tools/faqs/faq.php?id=13&t=5).

### Running this notebook

- Get [pipenv](https://docs.pipenv.org) if you don't have it already
- Clone this repo and `cd` into the directory
- Install the dependencies: `pipenv install`
- [Get your EIA API key here](https://www.eia.gov/developer/) and save it as an environmental variable called `EIA_API_KEY`
- [Get your BLS API key here](https://data.bls.gov/registrationEngine/) and save it as an environmental variable called `BLS_API_KEY`
- Run the notebook: `pipenv run jupyter notebook`
