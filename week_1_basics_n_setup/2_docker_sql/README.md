### backup of bash commands:
- <history -w ~/061123_history.txt>
C:\Users\charl\061123_history.txt



## issues with volume mapping, use //c/ instead of /c/
winpty docker run -it \
  -e POSTGRES_USER="root" \
  -e POSTGRES_PASSWORD="root" \
  -e POSTGRES_DB="ny_taxi" \
  -v //c/Users/charl/Documents/repo/data-engineering-zoomcamp/week_1_basics_n_setup/2_docker_sql/ny_taxi_postgres_data:/var/lib/postgresql/data \
  -p 5432:5432 \
  postgres:13

