# Air Quality Index (AQI) Data collection, analysation and visualisation

Pollution is now a major problem, this project focuses on providing AQI data and visualisations for very precise locations so as to pinpoint the actual sources of pollution instead of providing data for large chunks of areas.

## Getting Started

These instructions will get you a copy of the project up and running on your local machine for development and testing purposes. See deployment for notes on how to deploy the project on a live system.

The heart of this app is in ``Flask_Server.py`` which runs on the machine ip on which the this py file is running.
The data visualisation part is done by another stand-alone Dash app named ``Dash_plotting_real_time.py`` which connects to the sqlite DB which stores the AQI data recived by various sensors across the nation. The visualisations provided by this app are included as an ``iframe`` on the main web app so, easy integration.

To install the requires modeules to run this, you need to ``pip install`` the following

- flask
- Dash and its components
- flask-sqlalchemy
- python-aqi
- pandas

You also need an arduino to get real-time data. The code to be uploaded to arduino is included in the Hardware folder.
You just need the to change the ``ip`` address to your server on which you are running this app, also, the location, latitude and the longitude.

## Incase you don't have a real arduino to test 

Don't worry, we have got you covered. In this case, you can run the ``Dash_plotting_server.py`` instead of ``Dash_plotting_real_time.py`` which connects to the DB containing Dummy AQI data for various locaions.

## Contributing

Please feel free to contribute. We would love to see pull requests from you guys.


## Versioning

We use [SemVer](http://semver.org/) for versioning.

## Authors

* **Mankaran Singh** - *Initial work* - [MankaranSingh](https://github.com/MankaranSingh)
* **Prakhar Singh** - *Initial work* - [prakharsingh1312](https://github.com/prakharsingh1312)
* **Prakhar Singh** - *Initial work* - [uchauhan2022](https://github.com/uchauhan2022)

## Acknowledgments

* Special thanks Dash/Plotly team for providing such a great visualisation tool
* The Creative Computing Society (CCS) team who always inspires and motivates to push ourselves beyond limits.
* Hats-off to all those people who built the other dependencies used in this project  
