# DataBase Export

DataBase Export is simple python application example to export the content of a database

    For this project PostgreSQL DB is used with two tables Product and review.


## Usage

Download or clone the [DatabaseExportPython](https://github.com/DILMADALE/DatabaseExportPython) project

From the dbexport folder run the following command
```bash
pip install dbexport
```

Activate the pipenv
```bash
pipenv shell
```

Setup DB url
```bash
(dbexport) $ DB_URL="postgres://db_username:db_password@db_public_ip:db_port/db_name" PYTHONPATH=. python
```

To export the DB content in CSV format - {file name - product_rating.csv}
```bash
python product_csv.py
```

To export the DB content in json format - {file name - product_rating.json}
```bash
python product_json.py
```

### How to use for different db
    - Update the models.py to map to columns of the DB.
    - Update the product_{csv/json}.py to reflect the changes made to models.py and what value needs to printed on the output file.

## Contributing
Pull requests are welcome. For major changes, please open an issue first to discuss what you would like to change.

###### Shoutout to Linux Academy
    To use the application as it is, you can use the DB setup script to setup a PostgreSQL server with the tables.
    [DB Setup Script](https://raw.githubusercontent.com/linuxacademy/content-python-use-cases/master/helpers/db_setup.sh)