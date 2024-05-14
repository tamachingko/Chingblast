requirement
Flask==2.0.3
SQLAlchemy==1.4.31

how to run project
pip install -r requirements.txt
python -c 'from database import init_db; init_db()'
python app.py

how to run pip
url_shortener/
├── url_shortener/
│   ├── __init__.py
│   ├── app.py
│   ├── database.py
│   ├── models.py
│   └── templates/
│       └── index.html
├── tests/
│   └── test_app.py
├── setup.py
├── README.md
├── MANIFEST.in
└── requirements.txt

from setuptools import setup, find_packages

setup(
    name='url_shortener',
    version='0.1.0',
    packages=find_packages(),
    include_package_data=True,
    install_requires=[
        'Flask>=2.0.3',
        'SQLAlchemy>=1.4.31'
    ],
    entry_points={
        'console_scripts': [
            'url_shortener=url_shortener.app:main'
        ]
    },
    package_data={
        'url_shortener': ['templates/*.html'],
    },
)
# This file can be left empty or you can add package-level docstrings and imports
