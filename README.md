# appsec101-dast
appsec101


## Start and stop zap and juiceshop
```bash
# start
docker-compose up -d
# stop
docker-compose down
```

## Scan and get report
- After running the python script, a HTML file will be generated in your working directory.
- 
```bash
# Init and install requirement
python3 -m venv venv
source venv/bin/activate
pip install -r requirements.txt
# run and get report
python basic-spider-scan.py
```

## Notice
- API key are hardcode in `docker-compose.yml` and `basic-spider-scan.py` file.
- Only listen on localhost.
- The target `http://web:3000` is from juiceshop container name.


## Reference
- https://github.com/zaproxy/zap-api-python
- https://github.com/zaproxy/zaproxy/blob/develop/docker/zap-baseline.py