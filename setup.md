### Python and Database Requirements
`Python 3.9`

`PostgreSQL database`

Required Python libraries (listed in requirements.txt)

run `pip install -r requirements.txt` - run in a virtualenv (recommended)

### R Requirements
Some of the processes and dependencies in the OHDSI environment may require specific R packages to interact with the OHDSI CDM and tools. Ensure the following R packages are installed:

```bash
install.packages("devtools")
install.packages("DatabaseConnector")
install.packages("SqlRender")
devtools::install_github("OHDSI/CommonDataModel")  # For working with CDM-related functionality
install.packages("arrow")
```

Have you postgresql server downloaded, or you could spin up a docker container or connect to an external host.

### Make sure this is done.
set both R and Java Home
example for windows terminal
```bash
setx R_HOME "C:\Program Files\R\xxx"
setx JAVA_HOME "C:\Program Files\Java\xxx"
setx PATH "%PATH%;%JAVA_HOME%\bin;%R_HOME%\bin\x64"
```

### create an environment variable file
file name should be `.env`
copy what is stored in `.env.example` into `.env`

### check out to run ATLAS - a little spin for you.
https://github.com/eHealthHub4Cancer/SPIN_WEB_API_ATLAS/blob/main/README.md


### spin all at once- still trying for other architectures - you might be lucky anyways
https://github.com/eHealthHub4Cancer/ohdsi_cdm_loader


### some scripts
https://github.com/eHealthHub4Cancer/ETL_script 
https://github.com/OHDSI/ETL-Synthea
https://github.com/OHDSI/dbt-synthea


#### Keep it going!
