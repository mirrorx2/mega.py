# Mega.py

Python library for the Mega.co.nz API, currently supporting login, uploading, downloading & deleting of files.

This is a work in progress, further functionality coming shortly.

## How To Use

### Create an instance of Mega.py

    mega = Mega()

### Login to Mega

    m = mega.login(email, password)

### Get user details

    details = m.get_user()

### Get account files

    files = m.get_files()

### Upload a file

    m.upload('myfile.doc')

### Download a file from URL or it's ID,key combo
    m.download('utYjgSTQ','OM4U3V5v_W4N5edSo0wolg1D5H0fwSrLD3oLnLuS9pc')
    m.download_url('https://mega.co.nz/#!utYjgSTQ!OM4U3V5v_W4N5edSo0wolg1D5H0fwSrLD3oLnLuS9pc')

### Get a public link for a file
    m.get_link('utYjgSTQ','OM4U3V5v_W4N5edSo0wolg1D5H0fwSrLD3oLnLuS9pc')

### Search for a file
    m.find('myfile.doc')

### Trash a file from URL or it's ID

    m.delete('utYjgSTQ')
    m.delete_url('https://mega.co.nz/#!utYjgSTQ!OM4U3V5v_W4N5edSo0wolg1D5H0fwSrLD3oLnLuS9pc')

## Requirements

    1. Python2.7+
    2. Python requests - python-requests.org
    3. PyCrypto - dlitz.net/software/pycrypto/

## Tests

    Test .py files can be found in /tests, run these to ensure Mega.py is working 100%.

## Contribute

    Feel free to pull the source and make changes and additions.

    Learn about the API at Mega.co.nz
    - https://mega.co.nz/#developers

