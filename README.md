# Example Package

Полезный документ: [Creating the package files](https://packaging.python.org/en/latest/tutorials/packaging-projects/)

Важна структура каталогов проекта.

```bash
packaging_tutorial/
├── LICENSE
├── pyproject.toml
├── README.md
├── src/
│   └── example_package_YOUR_USERNAME_HERE/
│       ├── __init__.py
│       └── example.py
└── tests/
```

Если добавить `__main__.py` то у проекта будет точка входа и его можно будет запускать в командной строке.



Нужные команды для построения пакета

1. обновить pip


```bash
python -m pip install --upgrade build
```


2. создать пакет

```bash
python -m build
```

3. запустить пакет с точки входа `__main__.py`

```bash
 python .\dist\my_package-0.0.1-py3-none-any.whl\my_package
```