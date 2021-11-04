# test

# one time password

## Run Code
```bash
# Enter python virtual environment
python3 -m venv env
source env/bin/activate
# Install requirements
python -m pip install --upgrade pip
python -m pip install -r requirements.txt
# Run code
python submission.py --generate-qr
python submission.py --get-otp
# Exit python virtual environment
deactivate
```

## Implementation
Secret key is randomly generated and stored in local text file in order to generate QR code and print relevant OTPs in separate commands. Storing secret key in local text file is reasonable to preserve secret key in such small scale project. To generate QR code, secret key is read which is used to generate QR code. To print relevant OTPs, secret key is read which is used to print relevant OTPs.
