
## Demo
A online demo is avaiable at [isi.sorz.org](https://isi.sorz.org/).

## Install

0. Download repository
  ```
  git clone https://github.com/sorz/isi.git
  ```

1. Install [Python](https://www.python.org/) 3.4 or above
  ```
  apt-get install python3 python3-virtualenv
  ```
  
2. Install [Bower](http://bower.io/)
   ```
   apt-get isntall nodejs npm
   npm install -g bower
   ```

3. (optional) Create virtual environment
  ```
  virtualenv env
  . env/bin/activate
  ```

4. Install Python modules
  ```
  pip install -r requirements.txt
  ```

5. Copy a config file and edit it
  ```
  cd store/store/settings
  cp config.sample.py config.py
  vim config.py
  ```

6. Install JavaScript libraries
  ```
  python manage.py bower_install
  ```

7. Migrate database
  ```
  python manage.py migrate
  ```

8. (optional) Load demo data
  ```
  python manage.py loaddata /path/to/data.json
  ```

9. Run
  ```
  python manage.py runserver
  ```

