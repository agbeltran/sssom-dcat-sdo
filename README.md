# sssom-dcat-sdo
A repository for the [SSSOM](https://mapping-commons.github.io/sssom/spec/) mapping between [DCAT](https://w3c.github.io/dxwg/dcat/) and SDO


# installation

SSSOM works for Python >=3.8, <3.12 (I couldn't get it working with Python 3.12).

These steps install the required library (sssom) in a virtual environment:
```
python3 -m virtualenv venv
source venv/bin/activate
python3 -m pip install -r requirements.txt 
```

To parse the mapping use:
```
sssom parse dcat-sdo-sssom.tsv -m dcat-sdo-sssom.yml 
sssom parse dcat-sdo-owl-sssom.tsv -m dcat-sdo-owl-sssom.yml 
```

To convert the mappings into OWL
```
sssom convert dcat-sdo-sssom.tsv --output dcat-sdo-sssom.owl --output-format owl
```


To deactivate the virtual environment:
```
deactivate
```
