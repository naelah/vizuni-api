# vizuni-api
python api for vizuni data-driven dashboard

## Resources
- https://towardsdatascience.com/working-with-apis-using-flask-flask-restplus-and-swagger-ui-7cf447deda7f

#### Testing
```
$env:FLASK_APP = ".\test.py"
flask run
```

App available on [http://127.0.0.1:5000/]

#### Notes
- werkzeug import caused fail thus adding ` from werkzeug.utils import cached_property ` to the script as well as downgrading werzeug to a version 0.16.1 solves the issue `pip install --upgrade Werkzeug==0.16.1`
- flask-restplus is no longer maintained and should be replaced with flask-restx