# test

# one time password

## Execution
```bash
# Enter python virtual environment
python3 -m venv env
source env/bin/activate
# Install requirements
python -m pip install --upgrade pip
python -m pip install -r requirements.txt
# Execution
python submission.py --generate-qr
python submission.py --get-otp
# Exit python virtual environment
deactivate
```

## Implementation
Secret key is randomly generated and stored in local text file in order to preserve secret key between separate commands. In such small scale project, storing secret key in local text file is reasonable in order to preserve secret key. To generate QR code, secret key is read from local file which is used to generate QR code. To print relevant OTPs, secret key is read from local file which is used to print relevant OTPs.
