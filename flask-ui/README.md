# JLU Tag Flask UI

#### Clone

```sh
git clone --recurse-submodules --remote-submodule https://github.com/KDI-2023/flask-ui.git
```

#### Run

```sh
cd flask-ui
py -m pip install -r requirements.txt
flask -A webui run --debug --port 23648
```

#### How to use

##### Search

`http://ip:port/search/<str>` like `http://127.0.0.1:23648/search/柯南`.

##### UID

`http://ip:port/uid/<uid>` like `http://127.0.0.1:23648/uid/eb58eb0963c64062b5030663e77b49df`.

##### API/Search

`http://ip:port/api/search/<str>` like `http://127.0.0.1:23648/api/search/柯南`.

Return a JSON.

##### API/UID

`http://ip:port/api/uid/<uid>` like `http://127.0.0.1:23648/api/uid/eb58eb0963c64062b5030663e77b49df`.

Return a JSON.
